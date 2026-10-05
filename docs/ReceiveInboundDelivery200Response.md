# ReceiveInboundDelivery200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Status** | **string** |  | 
**LogId** | **string** | The delivery log row | 
**EntityIds** | **[]string** | Records created or updated | 
**Reason** | Pointer to **string** | Why a delivery was skipped | [optional] 
**Items** | Pointer to **[]map[string]interface{}** | One result per record: &#x60;index&#x60; in the payload, &#x60;entity_id&#x60;, &#x60;created&#x60;, and the &#x60;error&#x60; body of a record that failed | [optional] 
**Errors** | Pointer to **map[string]interface{}** | Record errors of a partial delivery, &#x60;items[i].attributes.&lt;slug&gt;&#x60; &#x3D;&gt; messages | [optional] 

## Methods

### NewReceiveInboundDelivery200Response

`func NewReceiveInboundDelivery200Response(status string, logId string, entityIds []string, ) *ReceiveInboundDelivery200Response`

NewReceiveInboundDelivery200Response instantiates a new ReceiveInboundDelivery200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReceiveInboundDelivery200ResponseWithDefaults

`func NewReceiveInboundDelivery200ResponseWithDefaults() *ReceiveInboundDelivery200Response`

NewReceiveInboundDelivery200ResponseWithDefaults instantiates a new ReceiveInboundDelivery200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetStatus

`func (o *ReceiveInboundDelivery200Response) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *ReceiveInboundDelivery200Response) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *ReceiveInboundDelivery200Response) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetLogId

`func (o *ReceiveInboundDelivery200Response) GetLogId() string`

GetLogId returns the LogId field if non-nil, zero value otherwise.

### GetLogIdOk

`func (o *ReceiveInboundDelivery200Response) GetLogIdOk() (*string, bool)`

GetLogIdOk returns a tuple with the LogId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogId

`func (o *ReceiveInboundDelivery200Response) SetLogId(v string)`

SetLogId sets LogId field to given value.


### GetEntityIds

`func (o *ReceiveInboundDelivery200Response) GetEntityIds() []string`

GetEntityIds returns the EntityIds field if non-nil, zero value otherwise.

### GetEntityIdsOk

`func (o *ReceiveInboundDelivery200Response) GetEntityIdsOk() (*[]string, bool)`

GetEntityIdsOk returns a tuple with the EntityIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityIds

`func (o *ReceiveInboundDelivery200Response) SetEntityIds(v []string)`

SetEntityIds sets EntityIds field to given value.


### GetReason

`func (o *ReceiveInboundDelivery200Response) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *ReceiveInboundDelivery200Response) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *ReceiveInboundDelivery200Response) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *ReceiveInboundDelivery200Response) HasReason() bool`

HasReason returns a boolean if a field has been set.

### GetItems

`func (o *ReceiveInboundDelivery200Response) GetItems() []map[string]interface{}`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *ReceiveInboundDelivery200Response) GetItemsOk() (*[]map[string]interface{}, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *ReceiveInboundDelivery200Response) SetItems(v []map[string]interface{})`

SetItems sets Items field to given value.

### HasItems

`func (o *ReceiveInboundDelivery200Response) HasItems() bool`

HasItems returns a boolean if a field has been set.

### GetErrors

`func (o *ReceiveInboundDelivery200Response) GetErrors() map[string]interface{}`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *ReceiveInboundDelivery200Response) GetErrorsOk() (*map[string]interface{}, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *ReceiveInboundDelivery200Response) SetErrors(v map[string]interface{})`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *ReceiveInboundDelivery200Response) HasErrors() bool`

HasErrors returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


