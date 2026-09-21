# ResolvedAggregateBlockResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BlockId** | Pointer to **string** | Dashboard block unique identifier | [optional] 
**Title** | Pointer to **string** | Block header title | [optional] 
**Type** | Pointer to **string** | Block type discriminator | [optional] 
**Limit** | Pointer to **int32** | Maximum number of groups returned, as configured on the block | [optional] 
**Truncated** | Pointer to **bool** | Whether more groups exist beyond &#x60;limit&#x60; | [optional] 
**Groups** | Pointer to [**[]ResolvedAggregateBlockResponseGroupsInner**](ResolvedAggregateBlockResponseGroupsInner.md) | One row per group, in the order configured on the block | [optional] 

## Methods

### NewResolvedAggregateBlockResponse

`func NewResolvedAggregateBlockResponse() *ResolvedAggregateBlockResponse`

NewResolvedAggregateBlockResponse instantiates a new ResolvedAggregateBlockResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResolvedAggregateBlockResponseWithDefaults

`func NewResolvedAggregateBlockResponseWithDefaults() *ResolvedAggregateBlockResponse`

NewResolvedAggregateBlockResponseWithDefaults instantiates a new ResolvedAggregateBlockResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBlockId

`func (o *ResolvedAggregateBlockResponse) GetBlockId() string`

GetBlockId returns the BlockId field if non-nil, zero value otherwise.

### GetBlockIdOk

`func (o *ResolvedAggregateBlockResponse) GetBlockIdOk() (*string, bool)`

GetBlockIdOk returns a tuple with the BlockId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlockId

`func (o *ResolvedAggregateBlockResponse) SetBlockId(v string)`

SetBlockId sets BlockId field to given value.

### HasBlockId

`func (o *ResolvedAggregateBlockResponse) HasBlockId() bool`

HasBlockId returns a boolean if a field has been set.

### GetTitle

`func (o *ResolvedAggregateBlockResponse) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ResolvedAggregateBlockResponse) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ResolvedAggregateBlockResponse) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ResolvedAggregateBlockResponse) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetType

`func (o *ResolvedAggregateBlockResponse) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ResolvedAggregateBlockResponse) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ResolvedAggregateBlockResponse) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ResolvedAggregateBlockResponse) HasType() bool`

HasType returns a boolean if a field has been set.

### GetLimit

`func (o *ResolvedAggregateBlockResponse) GetLimit() int32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *ResolvedAggregateBlockResponse) GetLimitOk() (*int32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *ResolvedAggregateBlockResponse) SetLimit(v int32)`

SetLimit sets Limit field to given value.

### HasLimit

`func (o *ResolvedAggregateBlockResponse) HasLimit() bool`

HasLimit returns a boolean if a field has been set.

### GetTruncated

`func (o *ResolvedAggregateBlockResponse) GetTruncated() bool`

GetTruncated returns the Truncated field if non-nil, zero value otherwise.

### GetTruncatedOk

`func (o *ResolvedAggregateBlockResponse) GetTruncatedOk() (*bool, bool)`

GetTruncatedOk returns a tuple with the Truncated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTruncated

`func (o *ResolvedAggregateBlockResponse) SetTruncated(v bool)`

SetTruncated sets Truncated field to given value.

### HasTruncated

`func (o *ResolvedAggregateBlockResponse) HasTruncated() bool`

HasTruncated returns a boolean if a field has been set.

### GetGroups

`func (o *ResolvedAggregateBlockResponse) GetGroups() []ResolvedAggregateBlockResponseGroupsInner`

GetGroups returns the Groups field if non-nil, zero value otherwise.

### GetGroupsOk

`func (o *ResolvedAggregateBlockResponse) GetGroupsOk() (*[]ResolvedAggregateBlockResponseGroupsInner, bool)`

GetGroupsOk returns a tuple with the Groups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroups

`func (o *ResolvedAggregateBlockResponse) SetGroups(v []ResolvedAggregateBlockResponseGroupsInner)`

SetGroups sets Groups field to given value.

### HasGroups

`func (o *ResolvedAggregateBlockResponse) HasGroups() bool`

HasGroups returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


