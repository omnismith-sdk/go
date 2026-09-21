# AggregateEntitiesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**FilterGroups** | Pointer to [**[][]EntityFilter**]([]EntityFilter.md) | Narrows the records before grouping. Same grammar as the search endpoint: Filter groups: clauses inside a group are AND-ed, groups are OR-ed. &#x60;[]&#x60; applies no filter, &#x60;[[a, b]]&#x60; is &#x60;a AND b&#x60;, &#x60;[[a], [b, c]]&#x60; is &#x60;a OR (b AND c)&#x60;. | [optional] 
**GroupBy** | Pointer to **[]string** | Attribute slugs or UUIDs to group by, at most 3. Lists, references, strings, numbers, booleans and dates can be keys; metrics, markdown, files and images cannot. Empty groups the whole filtered set into one row. | [optional] 
**Aggregations** | [**[]AggregateEntitiesRequestAggregationsInner**](AggregateEntitiesRequestAggregationsInner.md) | Reduces computed for every group, reported back in this order. &#x60;count&#x60; takes no field; &#x60;sum&#x60; and &#x60;avg&#x60; need a number attribute; &#x60;min&#x60; and &#x60;max&#x60; accept number, date and datetime attributes. | 
**Limit** | Pointer to **int32** | Maximum number of groups returned (1-100). The response says whether more groups exist. | [optional] [default to 50]

## Methods

### NewAggregateEntitiesRequest

`func NewAggregateEntitiesRequest(aggregations []AggregateEntitiesRequestAggregationsInner, ) *AggregateEntitiesRequest`

NewAggregateEntitiesRequest instantiates a new AggregateEntitiesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAggregateEntitiesRequestWithDefaults

`func NewAggregateEntitiesRequestWithDefaults() *AggregateEntitiesRequest`

NewAggregateEntitiesRequestWithDefaults instantiates a new AggregateEntitiesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetFilterGroups

`func (o *AggregateEntitiesRequest) GetFilterGroups() [][]EntityFilter`

GetFilterGroups returns the FilterGroups field if non-nil, zero value otherwise.

### GetFilterGroupsOk

`func (o *AggregateEntitiesRequest) GetFilterGroupsOk() (*[][]EntityFilter, bool)`

GetFilterGroupsOk returns a tuple with the FilterGroups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilterGroups

`func (o *AggregateEntitiesRequest) SetFilterGroups(v [][]EntityFilter)`

SetFilterGroups sets FilterGroups field to given value.

### HasFilterGroups

`func (o *AggregateEntitiesRequest) HasFilterGroups() bool`

HasFilterGroups returns a boolean if a field has been set.

### GetGroupBy

`func (o *AggregateEntitiesRequest) GetGroupBy() []string`

GetGroupBy returns the GroupBy field if non-nil, zero value otherwise.

### GetGroupByOk

`func (o *AggregateEntitiesRequest) GetGroupByOk() (*[]string, bool)`

GetGroupByOk returns a tuple with the GroupBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroupBy

`func (o *AggregateEntitiesRequest) SetGroupBy(v []string)`

SetGroupBy sets GroupBy field to given value.

### HasGroupBy

`func (o *AggregateEntitiesRequest) HasGroupBy() bool`

HasGroupBy returns a boolean if a field has been set.

### GetAggregations

`func (o *AggregateEntitiesRequest) GetAggregations() []AggregateEntitiesRequestAggregationsInner`

GetAggregations returns the Aggregations field if non-nil, zero value otherwise.

### GetAggregationsOk

`func (o *AggregateEntitiesRequest) GetAggregationsOk() (*[]AggregateEntitiesRequestAggregationsInner, bool)`

GetAggregationsOk returns a tuple with the Aggregations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAggregations

`func (o *AggregateEntitiesRequest) SetAggregations(v []AggregateEntitiesRequestAggregationsInner)`

SetAggregations sets Aggregations field to given value.


### GetLimit

`func (o *AggregateEntitiesRequest) GetLimit() int32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *AggregateEntitiesRequest) GetLimitOk() (*int32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *AggregateEntitiesRequest) SetLimit(v int32)`

SetLimit sets Limit field to given value.

### HasLimit

`func (o *AggregateEntitiesRequest) HasLimit() bool`

HasLimit returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


