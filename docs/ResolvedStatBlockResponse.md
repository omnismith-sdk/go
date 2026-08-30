# ResolvedStatBlockResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BlockId** | Pointer to **string** | Dashboard block unique identifier | [optional] 
**Title** | Pointer to **string** | Block header title | [optional] 
**Type** | Pointer to **string** | Block type discriminator | [optional] 
**Count** | Pointer to **int32** | Total count of entities matching template and active filter rules | [optional] 

## Methods

### NewResolvedStatBlockResponse

`func NewResolvedStatBlockResponse() *ResolvedStatBlockResponse`

NewResolvedStatBlockResponse instantiates a new ResolvedStatBlockResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResolvedStatBlockResponseWithDefaults

`func NewResolvedStatBlockResponseWithDefaults() *ResolvedStatBlockResponse`

NewResolvedStatBlockResponseWithDefaults instantiates a new ResolvedStatBlockResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBlockId

`func (o *ResolvedStatBlockResponse) GetBlockId() string`

GetBlockId returns the BlockId field if non-nil, zero value otherwise.

### GetBlockIdOk

`func (o *ResolvedStatBlockResponse) GetBlockIdOk() (*string, bool)`

GetBlockIdOk returns a tuple with the BlockId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlockId

`func (o *ResolvedStatBlockResponse) SetBlockId(v string)`

SetBlockId sets BlockId field to given value.

### HasBlockId

`func (o *ResolvedStatBlockResponse) HasBlockId() bool`

HasBlockId returns a boolean if a field has been set.

### GetTitle

`func (o *ResolvedStatBlockResponse) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ResolvedStatBlockResponse) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ResolvedStatBlockResponse) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ResolvedStatBlockResponse) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetType

`func (o *ResolvedStatBlockResponse) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ResolvedStatBlockResponse) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ResolvedStatBlockResponse) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ResolvedStatBlockResponse) HasType() bool`

HasType returns a boolean if a field has been set.

### GetCount

`func (o *ResolvedStatBlockResponse) GetCount() int32`

GetCount returns the Count field if non-nil, zero value otherwise.

### GetCountOk

`func (o *ResolvedStatBlockResponse) GetCountOk() (*int32, bool)`

GetCountOk returns a tuple with the Count field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCount

`func (o *ResolvedStatBlockResponse) SetCount(v int32)`

SetCount sets Count field to given value.

### HasCount

`func (o *ResolvedStatBlockResponse) HasCount() bool`

HasCount returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


