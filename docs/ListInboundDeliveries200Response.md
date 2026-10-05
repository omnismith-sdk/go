# ListInboundDeliveries200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]InboundDeliverySummary**](InboundDeliverySummary.md) |  | 
**Total** | **int32** | Deliveries matching the filters | 

## Methods

### NewListInboundDeliveries200Response

`func NewListInboundDeliveries200Response(data []InboundDeliverySummary, total int32, ) *ListInboundDeliveries200Response`

NewListInboundDeliveries200Response instantiates a new ListInboundDeliveries200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListInboundDeliveries200ResponseWithDefaults

`func NewListInboundDeliveries200ResponseWithDefaults() *ListInboundDeliveries200Response`

NewListInboundDeliveries200ResponseWithDefaults instantiates a new ListInboundDeliveries200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *ListInboundDeliveries200Response) GetData() []InboundDeliverySummary`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ListInboundDeliveries200Response) GetDataOk() (*[]InboundDeliverySummary, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ListInboundDeliveries200Response) SetData(v []InboundDeliverySummary)`

SetData sets Data field to given value.


### GetTotal

`func (o *ListInboundDeliveries200Response) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ListInboundDeliveries200Response) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ListInboundDeliveries200Response) SetTotal(v int32)`

SetTotal sets Total field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


