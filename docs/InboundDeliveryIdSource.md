# InboundDeliveryIdSource

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**From** | **string** | &#x60;header&#x60; or &#x60;body&#x60; | 
**Path** | **string** | A header name (&#x60;X-GitHub-Delivery&#x60;) for &#x60;header&#x60;; a JSON path for &#x60;body&#x60;: &#x60;$&#x60;, &#x60;.name&#x60;, &#x60;[&#39;name&#39;]&#x60; and &#x60;[index]&#x60;, e.g. &#x60;$.id&#x60;. | 

## Methods

### NewInboundDeliveryIdSource

`func NewInboundDeliveryIdSource(from string, path string, ) *InboundDeliveryIdSource`

NewInboundDeliveryIdSource instantiates a new InboundDeliveryIdSource object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInboundDeliveryIdSourceWithDefaults

`func NewInboundDeliveryIdSourceWithDefaults() *InboundDeliveryIdSource`

NewInboundDeliveryIdSourceWithDefaults instantiates a new InboundDeliveryIdSource object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFrom

`func (o *InboundDeliveryIdSource) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *InboundDeliveryIdSource) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *InboundDeliveryIdSource) SetFrom(v string)`

SetFrom sets From field to given value.


### GetPath

`func (o *InboundDeliveryIdSource) GetPath() string`

GetPath returns the Path field if non-nil, zero value otherwise.

### GetPathOk

`func (o *InboundDeliveryIdSource) GetPathOk() (*string, bool)`

GetPathOk returns a tuple with the Path field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPath

`func (o *InboundDeliveryIdSource) SetPath(v string)`

SetPath sets Path field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


