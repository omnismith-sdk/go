# CreateInboundEndpointRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Name shown in the template editor and in record history | 
**Signature** | **map[string]interface{}** | How deliveries are authenticated. Every delivery must pass; a failure is answered with 401 and a &#x60;reason&#x60; (&#x60;missing_signature&#x60;, &#x60;malformed_signature&#x60;, &#x60;mismatch&#x60;, &#x60;stale_timestamp&#x60;).  Name the sender&#39;s preset: &#x60;{\&quot;preset\&quot;: \&quot;github\&quot;}&#x60;, &#x60;stripe&#x60;, &#x60;shopify&#x60;, &#x60;standard_webhooks&#x60; (symmetric &#x60;v1&#x60; only) or &#x60;lemonsqueezy&#x60;. Presets take no other members and also set &#x60;delivery_id_source&#x60; when the sender has an id.  For senders that cannot sign (Zapier, Make, n8n, scripts, devices): &#x60;{\&quot;preset\&quot;: \&quot;shared_secret_header\&quot;, \&quot;header\&quot;: \&quot;X-Omnismith-Secret\&quot;, \&quot;prefix\&quot;: \&quot;\&quot;}&#x60;. The sender sends the secret in &#x60;header&#x60;, after &#x60;prefix&#x60; (for example &#x60;Authorization&#x60; with &#x60;Bearer &#x60;). Both members are optional; those are the defaults.  For any other HMAC sender: &#x60;{\&quot;preset\&quot;: \&quot;custom_hmac\&quot;, ...}&#x60; with &#x60;header&#x60; (required), &#x60;algorithm&#x60; (&#x60;sha1&#x60;, &#x60;sha256&#x60;, &#x60;sha512&#x60;; default &#x60;sha256&#x60;), &#x60;format&#x60; (&#x60;plain&#x60; with an optional literal &#x60;prefix&#x60;; &#x60;kv_list&#x60; of comma-separated &#x60;key&#x3D;value&#x60; pairs with &#x60;signature_key&#x60; and optional &#x60;timestamp_key&#x60;; or &#x60;versioned_list&#x60; of space-separated &#x60;version,signature&#x60; entries with &#x60;version&#x60;), &#x60;encoding&#x60; (&#x60;hex&#x60; or &#x60;base64&#x60;; default &#x60;hex&#x60;), &#x60;signed_content&#x60; (a template over &#x60;{body}&#x60;, &#x60;{timestamp}&#x60; and &#x60;{id}&#x60;; default &#x60;{body}&#x60;), &#x60;timestamp_header&#x60;, &#x60;id_header&#x60;, &#x60;tolerance_seconds&#x60; (the replay window for timestamped signatures; default 300), &#x60;secret_encoding&#x60; (&#x60;raw&#x60; or &#x60;base64&#x60;; default &#x60;raw&#x60;) and &#x60;secret_prefix&#x60; (stripped before decoding a &#x60;base64&#x60; secret, for example &#x60;whsec_&#x60;).  An update may switch presets only when both store secrets the same way. | 
**Mapping** | **map[string]interface{}** | How a delivery&#39;s JSON payload becomes records of the template. Validated against the template on every save; check it on a sample payload with &#x60;previewInboundMapping&#x60; before saving.  Members: - &#x60;mode&#x60; (required): &#x60;create&#x60;, &#x60;update&#x60; (an unknown key is an item error) or &#x60;upsert&#x60;. &#x60;update&#x60; and &#x60;upsert&#x60; require &#x60;key&#x60;. - &#x60;key&#x60;: &#x60;{\&quot;path\&quot;: \&quot;$.data.object.id\&quot;, \&quot;prefix\&quot;: \&quot;stripe:\&quot;}&#x60;. The record&#39;s external key: the value at &#x60;path&#x60; (a string or number) after the literal &#x60;prefix&#x60;, which namespaces keys when several senders feed one template. - &#x60;items&#x60;: a path to a list; each element becomes one record (at most 100) and &#x60;$&#x60; then means the element, &#x60;$root&#x60; the whole body. Without it the whole body is one record. - &#x60;match&#x60;: conditions on the whole body that must all hold, or the delivery is acknowledged and skipped: &#x60;{\&quot;path\&quot;: \&quot;$.type\&quot;, \&quot;operator\&quot;: \&quot;eq\&quot;, \&quot;value\&quot;: \&quot;customer.created\&quot;}&#x60;. Operators: &#x60;eq&#x60;, &#x60;neq&#x60;, &#x60;in&#x60; (a list &#x60;value&#x60;), &#x60;exists&#x60;, &#x60;not_exists&#x60; (no &#x60;value&#x60;). Values compare strictly: &#x60;\&quot;1\&quot;&#x60; is not &#x60;1&#x60;. - &#x60;attributes&#x60; (required, 1 to 100): keyed by attribute slug or UUID of the template. Each entry has either &#x60;path&#x60; or a constant &#x60;value&#x60;, plus optionally: &#x60;default&#x60; (used when the path is absent or null), &#x60;on_null&#x60; (&#x60;skip&#x60;, the default, leaves the attribute as it is; &#x60;clear&#x60; clears it; not on metrics), &#x60;prefix&#x60; (reference attributes: the value after the prefix is an external key of the referenced template), &#x60;format&#x60; (date and datetime attributes: &#x60;iso8601&#x60;, &#x60;epoch_s&#x60; or &#x60;epoch_ms&#x60;), and &#x60;timestamp&#x60; (&#x60;{\&quot;path\&quot;: \&quot;$.ts\&quot;, \&quot;format\&quot;: \&quot;epoch_ms\&quot;}&#x60;: the observation time of a metric reading, or the backfill time of a value; &#x60;format&#x60; defaults to &#x60;iso8601&#x60;).  Paths support &#x60;$&#x60;, &#x60;.name&#x60;, &#x60;[&#39;name&#39;]&#x60; and &#x60;[index]&#x60; only. List values resolve by option label (case-insensitive) or id; options are never created. Metric attributes take numbers and append a reading. Values are type-checked and the template&#39;s rules are enforced as on any write. | 
**Enabled** | Pointer to **bool** | Whether the endpoint accepts deliveries. A disabled endpoint answers 404. | [optional] [default to true]
**Secret** | Pointer to **string** | The secret the sender signs with, when the sender issued it (Stripe and Shopify do). Omit it to have one generated, which suits GitHub, custom senders and &#x60;shared_secret_header&#x60; (always generated). The secret is returned once, in this response, and never again. | [optional] 
**DeliveryIdSource** | Pointer to [**NullableInboundDeliveryIdSource**](InboundDeliveryIdSource.md) |  | [optional] 

## Methods

### NewCreateInboundEndpointRequest

`func NewCreateInboundEndpointRequest(name string, signature map[string]interface{}, mapping map[string]interface{}, ) *CreateInboundEndpointRequest`

NewCreateInboundEndpointRequest instantiates a new CreateInboundEndpointRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateInboundEndpointRequestWithDefaults

`func NewCreateInboundEndpointRequestWithDefaults() *CreateInboundEndpointRequest`

NewCreateInboundEndpointRequestWithDefaults instantiates a new CreateInboundEndpointRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreateInboundEndpointRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateInboundEndpointRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateInboundEndpointRequest) SetName(v string)`

SetName sets Name field to given value.


### GetSignature

`func (o *CreateInboundEndpointRequest) GetSignature() map[string]interface{}`

GetSignature returns the Signature field if non-nil, zero value otherwise.

### GetSignatureOk

`func (o *CreateInboundEndpointRequest) GetSignatureOk() (*map[string]interface{}, bool)`

GetSignatureOk returns a tuple with the Signature field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSignature

`func (o *CreateInboundEndpointRequest) SetSignature(v map[string]interface{})`

SetSignature sets Signature field to given value.


### GetMapping

`func (o *CreateInboundEndpointRequest) GetMapping() map[string]interface{}`

GetMapping returns the Mapping field if non-nil, zero value otherwise.

### GetMappingOk

`func (o *CreateInboundEndpointRequest) GetMappingOk() (*map[string]interface{}, bool)`

GetMappingOk returns a tuple with the Mapping field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMapping

`func (o *CreateInboundEndpointRequest) SetMapping(v map[string]interface{})`

SetMapping sets Mapping field to given value.


### GetEnabled

`func (o *CreateInboundEndpointRequest) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *CreateInboundEndpointRequest) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *CreateInboundEndpointRequest) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *CreateInboundEndpointRequest) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetSecret

`func (o *CreateInboundEndpointRequest) GetSecret() string`

GetSecret returns the Secret field if non-nil, zero value otherwise.

### GetSecretOk

`func (o *CreateInboundEndpointRequest) GetSecretOk() (*string, bool)`

GetSecretOk returns a tuple with the Secret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecret

`func (o *CreateInboundEndpointRequest) SetSecret(v string)`

SetSecret sets Secret field to given value.

### HasSecret

`func (o *CreateInboundEndpointRequest) HasSecret() bool`

HasSecret returns a boolean if a field has been set.

### GetDeliveryIdSource

`func (o *CreateInboundEndpointRequest) GetDeliveryIdSource() InboundDeliveryIdSource`

GetDeliveryIdSource returns the DeliveryIdSource field if non-nil, zero value otherwise.

### GetDeliveryIdSourceOk

`func (o *CreateInboundEndpointRequest) GetDeliveryIdSourceOk() (*InboundDeliveryIdSource, bool)`

GetDeliveryIdSourceOk returns a tuple with the DeliveryIdSource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveryIdSource

`func (o *CreateInboundEndpointRequest) SetDeliveryIdSource(v InboundDeliveryIdSource)`

SetDeliveryIdSource sets DeliveryIdSource field to given value.

### HasDeliveryIdSource

`func (o *CreateInboundEndpointRequest) HasDeliveryIdSource() bool`

HasDeliveryIdSource returns a boolean if a field has been set.

### SetDeliveryIdSourceNil

`func (o *CreateInboundEndpointRequest) SetDeliveryIdSourceNil(b bool)`

 SetDeliveryIdSourceNil sets the value for DeliveryIdSource to be an explicit nil

### UnsetDeliveryIdSource
`func (o *CreateInboundEndpointRequest) UnsetDeliveryIdSource()`

UnsetDeliveryIdSource ensures that no value is present for DeliveryIdSource, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


