# AddListItemRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Value** | **string** | Display value / label for the new choice option. | 
**SortOrder** | Pointer to **int32** | Sorting rank for display ordering (lower numbers appear first). | [optional] [default to 0]
**Id** | Pointer to **NullableString** | Optional explicit UUID for the item. Generated automatically if omitted. | [optional] 

## Methods

### NewAddListItemRequest

`func NewAddListItemRequest(value string, ) *AddListItemRequest`

NewAddListItemRequest instantiates a new AddListItemRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAddListItemRequestWithDefaults

`func NewAddListItemRequestWithDefaults() *AddListItemRequest`

NewAddListItemRequestWithDefaults instantiates a new AddListItemRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValue

`func (o *AddListItemRequest) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *AddListItemRequest) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *AddListItemRequest) SetValue(v string)`

SetValue sets Value field to given value.


### GetSortOrder

`func (o *AddListItemRequest) GetSortOrder() int32`

GetSortOrder returns the SortOrder field if non-nil, zero value otherwise.

### GetSortOrderOk

`func (o *AddListItemRequest) GetSortOrderOk() (*int32, bool)`

GetSortOrderOk returns a tuple with the SortOrder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortOrder

`func (o *AddListItemRequest) SetSortOrder(v int32)`

SetSortOrder sets SortOrder field to given value.

### HasSortOrder

`func (o *AddListItemRequest) HasSortOrder() bool`

HasSortOrder returns a boolean if a field has been set.

### GetId

`func (o *AddListItemRequest) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AddListItemRequest) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AddListItemRequest) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *AddListItemRequest) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *AddListItemRequest) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *AddListItemRequest) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


