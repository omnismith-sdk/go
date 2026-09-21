# ReorderEntityActionsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Ids** | **[]string** | Every action UUID of the template, first to last. Omitting or repeating one is rejected with 422. | 

## Methods

### NewReorderEntityActionsRequest

`func NewReorderEntityActionsRequest(ids []string, ) *ReorderEntityActionsRequest`

NewReorderEntityActionsRequest instantiates a new ReorderEntityActionsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReorderEntityActionsRequestWithDefaults

`func NewReorderEntityActionsRequestWithDefaults() *ReorderEntityActionsRequest`

NewReorderEntityActionsRequestWithDefaults instantiates a new ReorderEntityActionsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIds

`func (o *ReorderEntityActionsRequest) GetIds() []string`

GetIds returns the Ids field if non-nil, zero value otherwise.

### GetIdsOk

`func (o *ReorderEntityActionsRequest) GetIdsOk() (*[]string, bool)`

GetIdsOk returns a tuple with the Ids field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIds

`func (o *ReorderEntityActionsRequest) SetIds(v []string)`

SetIds sets Ids field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


