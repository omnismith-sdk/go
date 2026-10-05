# PreviewInboundMappingRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Body** | Pointer to **map[string]interface{}** | A sample payload, as the sender would post it: for example the sample event in the sender&#39;s webhook documentation. | [optional] 
**DeliveryId** | Pointer to **string** | A delivery from the endpoint&#39;s log to use as the sample instead: the &#x60;log_id&#x60; the sender was answered with. | [optional] 
**Mapping** | Pointer to **map[string]interface{}** | A mapping to try instead of the saved one, in the same shape as the endpoint&#39;s &#x60;mapping&#x60;. It is not saved. | [optional] 

## Methods

### NewPreviewInboundMappingRequest

`func NewPreviewInboundMappingRequest() *PreviewInboundMappingRequest`

NewPreviewInboundMappingRequest instantiates a new PreviewInboundMappingRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPreviewInboundMappingRequestWithDefaults

`func NewPreviewInboundMappingRequestWithDefaults() *PreviewInboundMappingRequest`

NewPreviewInboundMappingRequestWithDefaults instantiates a new PreviewInboundMappingRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBody

`func (o *PreviewInboundMappingRequest) GetBody() map[string]interface{}`

GetBody returns the Body field if non-nil, zero value otherwise.

### GetBodyOk

`func (o *PreviewInboundMappingRequest) GetBodyOk() (*map[string]interface{}, bool)`

GetBodyOk returns a tuple with the Body field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBody

`func (o *PreviewInboundMappingRequest) SetBody(v map[string]interface{})`

SetBody sets Body field to given value.

### HasBody

`func (o *PreviewInboundMappingRequest) HasBody() bool`

HasBody returns a boolean if a field has been set.

### GetDeliveryId

`func (o *PreviewInboundMappingRequest) GetDeliveryId() string`

GetDeliveryId returns the DeliveryId field if non-nil, zero value otherwise.

### GetDeliveryIdOk

`func (o *PreviewInboundMappingRequest) GetDeliveryIdOk() (*string, bool)`

GetDeliveryIdOk returns a tuple with the DeliveryId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveryId

`func (o *PreviewInboundMappingRequest) SetDeliveryId(v string)`

SetDeliveryId sets DeliveryId field to given value.

### HasDeliveryId

`func (o *PreviewInboundMappingRequest) HasDeliveryId() bool`

HasDeliveryId returns a boolean if a field has been set.

### GetMapping

`func (o *PreviewInboundMappingRequest) GetMapping() map[string]interface{}`

GetMapping returns the Mapping field if non-nil, zero value otherwise.

### GetMappingOk

`func (o *PreviewInboundMappingRequest) GetMappingOk() (*map[string]interface{}, bool)`

GetMappingOk returns a tuple with the Mapping field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMapping

`func (o *PreviewInboundMappingRequest) SetMapping(v map[string]interface{})`

SetMapping sets Mapping field to given value.

### HasMapping

`func (o *PreviewInboundMappingRequest) HasMapping() bool`

HasMapping returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


