# ListItemLayoutResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ListItemId** | **string** | List item UUID | 
**AttributeId** | **string** | Parent attribute UUID | 
**SortOrder** | **int32** | Display sorting rank in selection menus | 

## Methods

### NewListItemLayoutResponse

`func NewListItemLayoutResponse(listItemId string, attributeId string, sortOrder int32, ) *ListItemLayoutResponse`

NewListItemLayoutResponse instantiates a new ListItemLayoutResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListItemLayoutResponseWithDefaults

`func NewListItemLayoutResponseWithDefaults() *ListItemLayoutResponse`

NewListItemLayoutResponseWithDefaults instantiates a new ListItemLayoutResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetListItemId

`func (o *ListItemLayoutResponse) GetListItemId() string`

GetListItemId returns the ListItemId field if non-nil, zero value otherwise.

### GetListItemIdOk

`func (o *ListItemLayoutResponse) GetListItemIdOk() (*string, bool)`

GetListItemIdOk returns a tuple with the ListItemId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListItemId

`func (o *ListItemLayoutResponse) SetListItemId(v string)`

SetListItemId sets ListItemId field to given value.


### GetAttributeId

`func (o *ListItemLayoutResponse) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *ListItemLayoutResponse) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *ListItemLayoutResponse) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.


### GetSortOrder

`func (o *ListItemLayoutResponse) GetSortOrder() int32`

GetSortOrder returns the SortOrder field if non-nil, zero value otherwise.

### GetSortOrderOk

`func (o *ListItemLayoutResponse) GetSortOrderOk() (*int32, bool)`

GetSortOrderOk returns a tuple with the SortOrder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortOrder

`func (o *ListItemLayoutResponse) SetSortOrder(v int32)`

SetSortOrder sets SortOrder field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


