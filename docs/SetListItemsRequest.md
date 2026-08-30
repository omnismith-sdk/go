# SetListItemsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Items** | [**[]ListItemInput**](ListItemInput.md) | Array of list item specifications to set. | 

## Methods

### NewSetListItemsRequest

`func NewSetListItemsRequest(items []ListItemInput, ) *SetListItemsRequest`

NewSetListItemsRequest instantiates a new SetListItemsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSetListItemsRequestWithDefaults

`func NewSetListItemsRequestWithDefaults() *SetListItemsRequest`

NewSetListItemsRequestWithDefaults instantiates a new SetListItemsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItems

`func (o *SetListItemsRequest) GetItems() []ListItemInput`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *SetListItemsRequest) GetItemsOk() (*[]ListItemInput, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *SetListItemsRequest) SetItems(v []ListItemInput)`

SetItems sets Items field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


