# InboundEndpointCreatedResponse

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
**Secret** | [**InboundSecretRevealed**](InboundSecretRevealed.md) |  | 

## Methods

### NewInboundEndpointCreatedResponse

`func NewInboundEndpointCreatedResponse(id string, templateId string, name string, enabled bool, url string, signature map[string]interface{}, mapping map[string]interface{}, deliveryIdSource NullableInboundDeliveryIdSource, secrets []InboundSecret, lastSignatureFailureAt NullableTime, createdBy string, createdAt time.Time, updatedAt time.Time, secret InboundSecretRevealed, ) *InboundEndpointCreatedResponse`

NewInboundEndpointCreatedResponse instantiates a new InboundEndpointCreatedResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInboundEndpointCreatedResponseWithDefaults

`func NewInboundEndpointCreatedResponseWithDefaults() *InboundEndpointCreatedResponse`

NewInboundEndpointCreatedResponseWithDefaults instantiates a new InboundEndpointCreatedResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *InboundEndpointCreatedResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *InboundEndpointCreatedResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *InboundEndpointCreatedResponse) SetId(v string)`

SetId sets Id field to given value.


### GetTemplateId

`func (o *InboundEndpointCreatedResponse) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *InboundEndpointCreatedResponse) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *InboundEndpointCreatedResponse) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.


### GetName

`func (o *InboundEndpointCreatedResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *InboundEndpointCreatedResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *InboundEndpointCreatedResponse) SetName(v string)`

SetName sets Name field to given value.


### GetEnabled

`func (o *InboundEndpointCreatedResponse) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *InboundEndpointCreatedResponse) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *InboundEndpointCreatedResponse) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.


### GetUrl

`func (o *InboundEndpointCreatedResponse) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *InboundEndpointCreatedResponse) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *InboundEndpointCreatedResponse) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetSignature

`func (o *InboundEndpointCreatedResponse) GetSignature() map[string]interface{}`

GetSignature returns the Signature field if non-nil, zero value otherwise.

### GetSignatureOk

`func (o *InboundEndpointCreatedResponse) GetSignatureOk() (*map[string]interface{}, bool)`

GetSignatureOk returns a tuple with the Signature field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSignature

`func (o *InboundEndpointCreatedResponse) SetSignature(v map[string]interface{})`

SetSignature sets Signature field to given value.


### GetMapping

`func (o *InboundEndpointCreatedResponse) GetMapping() map[string]interface{}`

GetMapping returns the Mapping field if non-nil, zero value otherwise.

### GetMappingOk

`func (o *InboundEndpointCreatedResponse) GetMappingOk() (*map[string]interface{}, bool)`

GetMappingOk returns a tuple with the Mapping field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMapping

`func (o *InboundEndpointCreatedResponse) SetMapping(v map[string]interface{})`

SetMapping sets Mapping field to given value.


### GetDeliveryIdSource

`func (o *InboundEndpointCreatedResponse) GetDeliveryIdSource() InboundDeliveryIdSource`

GetDeliveryIdSource returns the DeliveryIdSource field if non-nil, zero value otherwise.

### GetDeliveryIdSourceOk

`func (o *InboundEndpointCreatedResponse) GetDeliveryIdSourceOk() (*InboundDeliveryIdSource, bool)`

GetDeliveryIdSourceOk returns a tuple with the DeliveryIdSource field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveryIdSource

`func (o *InboundEndpointCreatedResponse) SetDeliveryIdSource(v InboundDeliveryIdSource)`

SetDeliveryIdSource sets DeliveryIdSource field to given value.


### SetDeliveryIdSourceNil

`func (o *InboundEndpointCreatedResponse) SetDeliveryIdSourceNil(b bool)`

 SetDeliveryIdSourceNil sets the value for DeliveryIdSource to be an explicit nil

### UnsetDeliveryIdSource
`func (o *InboundEndpointCreatedResponse) UnsetDeliveryIdSource()`

UnsetDeliveryIdSource ensures that no value is present for DeliveryIdSource, not even an explicit nil
### GetSecrets

`func (o *InboundEndpointCreatedResponse) GetSecrets() []InboundSecret`

GetSecrets returns the Secrets field if non-nil, zero value otherwise.

### GetSecretsOk

`func (o *InboundEndpointCreatedResponse) GetSecretsOk() (*[]InboundSecret, bool)`

GetSecretsOk returns a tuple with the Secrets field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecrets

`func (o *InboundEndpointCreatedResponse) SetSecrets(v []InboundSecret)`

SetSecrets sets Secrets field to given value.


### GetLastSignatureFailureAt

`func (o *InboundEndpointCreatedResponse) GetLastSignatureFailureAt() time.Time`

GetLastSignatureFailureAt returns the LastSignatureFailureAt field if non-nil, zero value otherwise.

### GetLastSignatureFailureAtOk

`func (o *InboundEndpointCreatedResponse) GetLastSignatureFailureAtOk() (*time.Time, bool)`

GetLastSignatureFailureAtOk returns a tuple with the LastSignatureFailureAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastSignatureFailureAt

`func (o *InboundEndpointCreatedResponse) SetLastSignatureFailureAt(v time.Time)`

SetLastSignatureFailureAt sets LastSignatureFailureAt field to given value.


### SetLastSignatureFailureAtNil

`func (o *InboundEndpointCreatedResponse) SetLastSignatureFailureAtNil(b bool)`

 SetLastSignatureFailureAtNil sets the value for LastSignatureFailureAt to be an explicit nil

### UnsetLastSignatureFailureAt
`func (o *InboundEndpointCreatedResponse) UnsetLastSignatureFailureAt()`

UnsetLastSignatureFailureAt ensures that no value is present for LastSignatureFailureAt, not even an explicit nil
### GetCreatedBy

`func (o *InboundEndpointCreatedResponse) GetCreatedBy() string`

GetCreatedBy returns the CreatedBy field if non-nil, zero value otherwise.

### GetCreatedByOk

`func (o *InboundEndpointCreatedResponse) GetCreatedByOk() (*string, bool)`

GetCreatedByOk returns a tuple with the CreatedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedBy

`func (o *InboundEndpointCreatedResponse) SetCreatedBy(v string)`

SetCreatedBy sets CreatedBy field to given value.


### GetCreatedAt

`func (o *InboundEndpointCreatedResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *InboundEndpointCreatedResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *InboundEndpointCreatedResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetUpdatedAt

`func (o *InboundEndpointCreatedResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *InboundEndpointCreatedResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *InboundEndpointCreatedResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.


### GetSecret

`func (o *InboundEndpointCreatedResponse) GetSecret() InboundSecretRevealed`

GetSecret returns the Secret field if non-nil, zero value otherwise.

### GetSecretOk

`func (o *InboundEndpointCreatedResponse) GetSecretOk() (*InboundSecretRevealed, bool)`

GetSecretOk returns a tuple with the Secret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecret

`func (o *InboundEndpointCreatedResponse) SetSecret(v InboundSecretRevealed)`

SetSecret sets Secret field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


