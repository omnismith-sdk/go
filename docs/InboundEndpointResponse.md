# InboundEndpointResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**TemplateId** | **string** |  | 
**Name** | **string** |  | 
**Enabled** | **bool** | A disabled endpoint answers every delivery with 404. | 
**Url** | **string** | The receive URL to configure in the sender. It is not a secret: the signature authenticates each delivery. | 
**Signature** | **map[string]interface{}** | How deliveries are authenticated: &#x60;preset&#x60;, plus the effective parameters for &#x60;custom_hmac&#x60; and &#x60;shared_secret_header&#x60;. | 
**Mapping** | **map[string]interface{}** | How a payload becomes records, with every default filled in (&#x60;on_null&#x60;, &#x60;key.prefix&#x60;, &#x60;timestamp.format&#x60;). | 
**DeliveryIdSource** | [**NullableInboundDeliveryIdSource**](InboundDeliveryIdSource.md) |  | 
**Secrets** | [**[]InboundSecret**](InboundSecret.md) | The secrets deliveries are verified with: one, or two while a rotation is under way. Only a hint of each is shown. | 
**LastSignatureFailureAt** | **NullableTime** | When a delivery last failed signature verification. A time newer than the last processed delivery usually means the sender uses the wrong secret. | 
**CreatedBy** | **string** | Email of the user who created the endpoint | 
**CreatedAt** | **time.Time** |  | 
**UpdatedAt** | **time.Time** |  | 

## Methods

### NewInboundEndpointResponse

`func NewInboundEndpointResponse(id string, templateId string, name string, enabled bool, url string, signature map[string]interface{}, mapping map[string]interface{}, deliveryIdSource NullableInboundDeliveryIdSource, secrets []InboundSecret, lastSignatureFailureAt NullableTime, createdBy string, createdAt time.Time, updatedAt time.Time, ) *InboundEndpointResponse`

NewInboundEndpointResponse instantiates a new InboundEndpointResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInboundEndpointResponseWithDefaults

`func NewInboundEndpointResponseWithDefaults() *InboundEndpointResponse`

NewInboundEndpointResponseWithDefaults instantiates a new InboundEndpointResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *InboundEndpointResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *InboundEndpointResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *InboundEndpointResponse) SetId(v string)`

SetId sets Id field to given value.


### GetTemplateId

`func (o *InboundEndpointResponse) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *InboundEndpointResponse) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *InboundEndpointResponse) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.


### GetName

`func (o *InboundEndpointResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *InboundEndpointResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *InboundEndpointResponse) SetName(v string)`

SetName sets Name field to given value.


### GetEnabled

`func (o *InboundEndpointResponse) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *InboundEndpointResponse) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *InboundEndpointResponse) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.


### GetUrl

`func (o *InboundEndpointResponse) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *InboundEndpointResponse) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *InboundEndpointResponse) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetSignature

`func (o *InboundEndpointResponse) GetSignature() map[string]interface{}`

GetSignature returns the Signature field if non-nil, zero value otherwise.

### GetSignatureOk

`func (o *InboundEndpointResponse) GetSignatureOk() (*map[string]interface{}, bool)`

GetSignatureOk returns a tuple with the Signature field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSignature

`func (o *InboundEndpointResponse) SetSignature(v map[string]interface{})`

SetSignature sets Signature field to given value.


### GetMapping

`func (o *InboundEndpointResponse) GetMapping() map[string]interface{}`

GetMapping returns the Mapping field if non-nil, zero value otherwise.

### GetMappingOk

`func (o *InboundEndpointResponse) GetMappingOk() (*map[string]interface{}, bool)`

GetMappingOk returns a tuple with the Mapping field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMapping

`func (o *InboundEndpointResponse) SetMapping(v map[string]interface{})`

SetMapping sets Mapping field to given value.


### GetDeliveryIdSource

`func (o *InboundEndpointResponse) GetDeliveryIdSource() InboundDeliveryIdSource`

GetDeliveryIdSource returns the DeliveryIdSource field if non-nil, zero value otherwise.

### GetDeliveryIdSourceOk

`func (o *InboundEndpointResponse) GetDeliveryIdSourceOk() (*InboundDeliveryIdSource, bool)`

GetDeliveryIdSourceOk returns a tuple with the DeliveryIdSource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveryIdSource

`func (o *InboundEndpointResponse) SetDeliveryIdSource(v InboundDeliveryIdSource)`

SetDeliveryIdSource sets DeliveryIdSource field to given value.


### SetDeliveryIdSourceNil

`func (o *InboundEndpointResponse) SetDeliveryIdSourceNil(b bool)`

 SetDeliveryIdSourceNil sets the value for DeliveryIdSource to be an explicit nil

### UnsetDeliveryIdSource
`func (o *InboundEndpointResponse) UnsetDeliveryIdSource()`

UnsetDeliveryIdSource ensures that no value is present for DeliveryIdSource, not even an explicit nil
### GetSecrets

`func (o *InboundEndpointResponse) GetSecrets() []InboundSecret`

GetSecrets returns the Secrets field if non-nil, zero value otherwise.

### GetSecretsOk

`func (o *InboundEndpointResponse) GetSecretsOk() (*[]InboundSecret, bool)`

GetSecretsOk returns a tuple with the Secrets field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecrets

`func (o *InboundEndpointResponse) SetSecrets(v []InboundSecret)`

SetSecrets sets Secrets field to given value.


### GetLastSignatureFailureAt

`func (o *InboundEndpointResponse) GetLastSignatureFailureAt() time.Time`

GetLastSignatureFailureAt returns the LastSignatureFailureAt field if non-nil, zero value otherwise.

### GetLastSignatureFailureAtOk

`func (o *InboundEndpointResponse) GetLastSignatureFailureAtOk() (*time.Time, bool)`

GetLastSignatureFailureAtOk returns a tuple with the LastSignatureFailureAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSignatureFailureAt

`func (o *InboundEndpointResponse) SetLastSignatureFailureAt(v time.Time)`

SetLastSignatureFailureAt sets LastSignatureFailureAt field to given value.


### SetLastSignatureFailureAtNil

`func (o *InboundEndpointResponse) SetLastSignatureFailureAtNil(b bool)`

 SetLastSignatureFailureAtNil sets the value for LastSignatureFailureAt to be an explicit nil

### UnsetLastSignatureFailureAt
`func (o *InboundEndpointResponse) UnsetLastSignatureFailureAt()`

UnsetLastSignatureFailureAt ensures that no value is present for LastSignatureFailureAt, not even an explicit nil
### GetCreatedBy

`func (o *InboundEndpointResponse) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *InboundEndpointResponse) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *InboundEndpointResponse) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.


### GetCreatedAt

`func (o *InboundEndpointResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *InboundEndpointResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *InboundEndpointResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *InboundEndpointResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *InboundEndpointResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *InboundEndpointResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


