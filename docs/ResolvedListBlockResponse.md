# ResolvedListBlockResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BlockId** | Pointer to **string** | Dashboard block unique identifier | [optional] 
**Title** | Pointer to **string** | Block header title | [optional] 
**Type** | Pointer to **string** | Block type discriminator | [optional] 
**Items** | Pointer to [**[]ResolvedListBlockResponseItemsInner**](ResolvedListBlockResponseItemsInner.md) | List of matching entity records with hydrated attributes | [optional] 
**TotalCount** | Pointer to **int32** | Total number of items matching filters | [optional] 

## Methods

### NewResolvedListBlockResponse

`func NewResolvedListBlockResponse() *ResolvedListBlockResponse`

NewResolvedListBlockResponse instantiates a new ResolvedListBlockResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResolvedListBlockResponseWithDefaults

`func NewResolvedListBlockResponseWithDefaults() *ResolvedListBlockResponse`

NewResolvedListBlockResponseWithDefaults instantiates a new ResolvedListBlockResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBlockId

`func (o *ResolvedListBlockResponse) GetBlockId() string`

GetBlockId returns the BlockId field if non-nil, zero value otherwise.

### GetBlockIdOk

`func (o *ResolvedListBlockResponse) GetBlockIdOk() (*string, bool)`

GetBlockIdOk returns a tuple with the BlockId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlockId

`func (o *ResolvedListBlockResponse) SetBlockId(v string)`

SetBlockId sets BlockId field to given value.

### HasBlockId

`func (o *ResolvedListBlockResponse) HasBlockId() bool`

HasBlockId returns a boolean if a field has been set.

### GetTitle

`func (o *ResolvedListBlockResponse) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ResolvedListBlockResponse) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ResolvedListBlockResponse) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ResolvedListBlockResponse) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetType

`func (o *ResolvedListBlockResponse) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ResolvedListBlockResponse) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ResolvedListBlockResponse) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ResolvedListBlockResponse) HasType() bool`

HasType returns a boolean if a field has been set.

### GetItems

`func (o *ResolvedListBlockResponse) GetItems() []ResolvedListBlockResponseItemsInner`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *ResolvedListBlockResponse) GetItemsOk() (*[]ResolvedListBlockResponseItemsInner, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *ResolvedListBlockResponse) SetItems(v []ResolvedListBlockResponseItemsInner)`

SetItems sets Items field to given value.

### HasItems

`func (o *ResolvedListBlockResponse) HasItems() bool`

HasItems returns a boolean if a field has been set.

### GetTotalCount

`func (o *ResolvedListBlockResponse) GetTotalCount() int32`

GetTotalCount returns the TotalCount field if non-nil, zero value otherwise.

### GetTotalCountOk

`func (o *ResolvedListBlockResponse) GetTotalCountOk() (*int32, bool)`

GetTotalCountOk returns a tuple with the TotalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCount

`func (o *ResolvedListBlockResponse) SetTotalCount(v int32)`

SetTotalCount sets TotalCount field to given value.

### HasTotalCount

`func (o *ResolvedListBlockResponse) HasTotalCount() bool`

HasTotalCount returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


