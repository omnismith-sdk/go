# ResolvedAggregateBlockResponseGroupsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Key** | Pointer to [**[]ResolvedAggregateBlockResponseGroupsInnerKeyInner**](ResolvedAggregateBlockResponseGroupsInnerKeyInner.md) | The group_by fields and their values, in configured order | [optional] 
**Aggregates** | Pointer to [**[]ResolvedAggregateBlockResponseGroupsInnerAggregatesInner**](ResolvedAggregateBlockResponseGroupsInnerAggregatesInner.md) | The configured reduces for this group, in configured order | [optional] 

## Methods

### NewResolvedAggregateBlockResponseGroupsInner

`func NewResolvedAggregateBlockResponseGroupsInner() *ResolvedAggregateBlockResponseGroupsInner`

NewResolvedAggregateBlockResponseGroupsInner instantiates a new ResolvedAggregateBlockResponseGroupsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResolvedAggregateBlockResponseGroupsInnerWithDefaults

`func NewResolvedAggregateBlockResponseGroupsInnerWithDefaults() *ResolvedAggregateBlockResponseGroupsInner`

NewResolvedAggregateBlockResponseGroupsInnerWithDefaults instantiates a new ResolvedAggregateBlockResponseGroupsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKey

`func (o *ResolvedAggregateBlockResponseGroupsInner) GetKey() []ResolvedAggregateBlockResponseGroupsInnerKeyInner`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *ResolvedAggregateBlockResponseGroupsInner) GetKeyOk() (*[]ResolvedAggregateBlockResponseGroupsInnerKeyInner, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *ResolvedAggregateBlockResponseGroupsInner) SetKey(v []ResolvedAggregateBlockResponseGroupsInnerKeyInner)`

SetKey sets Key field to given value.

### HasKey

`func (o *ResolvedAggregateBlockResponseGroupsInner) HasKey() bool`

HasKey returns a boolean if a field has been set.

### GetAggregates

`func (o *ResolvedAggregateBlockResponseGroupsInner) GetAggregates() []ResolvedAggregateBlockResponseGroupsInnerAggregatesInner`

GetAggregates returns the Aggregates field if non-nil, zero value otherwise.

### GetAggregatesOk

`func (o *ResolvedAggregateBlockResponseGroupsInner) GetAggregatesOk() (*[]ResolvedAggregateBlockResponseGroupsInnerAggregatesInner, bool)`

GetAggregatesOk returns a tuple with the Aggregates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAggregates

`func (o *ResolvedAggregateBlockResponseGroupsInner) SetAggregates(v []ResolvedAggregateBlockResponseGroupsInnerAggregatesInner)`

SetAggregates sets Aggregates field to given value.

### HasAggregates

`func (o *ResolvedAggregateBlockResponseGroupsInner) HasAggregates() bool`

HasAggregates returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


