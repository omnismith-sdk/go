# ListAutomationExecutions200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | Pointer to [**[]AutomationExecutionResponse**](AutomationExecutionResponse.md) |  | [optional] 
**Total** | Pointer to **int32** |  | [optional] 

## Methods

### NewListAutomationExecutions200Response

`func NewListAutomationExecutions200Response() *ListAutomationExecutions200Response`

NewListAutomationExecutions200Response instantiates a new ListAutomationExecutions200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListAutomationExecutions200ResponseWithDefaults

`func NewListAutomationExecutions200ResponseWithDefaults() *ListAutomationExecutions200Response`

NewListAutomationExecutions200ResponseWithDefaults instantiates a new ListAutomationExecutions200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *ListAutomationExecutions200Response) GetData() []AutomationExecutionResponse`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ListAutomationExecutions200Response) GetDataOk() (*[]AutomationExecutionResponse, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ListAutomationExecutions200Response) SetData(v []AutomationExecutionResponse)`

SetData sets Data field to given value.

### HasData

`func (o *ListAutomationExecutions200Response) HasData() bool`

HasData returns a boolean if a field has been set.

### GetTotal

`func (o *ListAutomationExecutions200Response) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ListAutomationExecutions200Response) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ListAutomationExecutions200Response) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *ListAutomationExecutions200Response) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


