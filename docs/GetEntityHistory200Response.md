# GetEntityHistory200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Items** | Pointer to [**[]GetEntityHistory200ResponseItemsInner**](GetEntityHistory200ResponseItemsInner.md) |  | [optional] 
**Total** | Pointer to **int32** |  | [optional] 

## Methods

### NewGetEntityHistory200Response

`func NewGetEntityHistory200Response() *GetEntityHistory200Response`

NewGetEntityHistory200Response instantiates a new GetEntityHistory200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetEntityHistory200ResponseWithDefaults

`func NewGetEntityHistory200ResponseWithDefaults() *GetEntityHistory200Response`

NewGetEntityHistory200ResponseWithDefaults instantiates a new GetEntityHistory200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItems

`func (o *GetEntityHistory200Response) GetItems() []GetEntityHistory200ResponseItemsInner`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *GetEntityHistory200Response) GetItemsOk() (*[]GetEntityHistory200ResponseItemsInner, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *GetEntityHistory200Response) SetItems(v []GetEntityHistory200ResponseItemsInner)`

SetItems sets Items field to given value.

### HasItems

`func (o *GetEntityHistory200Response) HasItems() bool`

HasItems returns a boolean if a field has been set.

### GetTotal

`func (o *GetEntityHistory200Response) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *GetEntityHistory200Response) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *GetEntityHistory200Response) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *GetEntityHistory200Response) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


