# AggregateEntitiesGroup

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Key** | [**[]AggregateEntitiesGroupKeyInner**](AggregateEntitiesGroupKeyInner.md) |  | 
**Aggregates** | [**[]AggregateEntitiesGroupAggregatesInner**](AggregateEntitiesGroupAggregatesInner.md) |  | 

## Methods

### NewAggregateEntitiesGroup

`func NewAggregateEntitiesGroup(key []AggregateEntitiesGroupKeyInner, aggregates []AggregateEntitiesGroupAggregatesInner, ) *AggregateEntitiesGroup`

NewAggregateEntitiesGroup instantiates a new AggregateEntitiesGroup object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAggregateEntitiesGroupWithDefaults

`func NewAggregateEntitiesGroupWithDefaults() *AggregateEntitiesGroup`

NewAggregateEntitiesGroupWithDefaults instantiates a new AggregateEntitiesGroup object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKey

`func (o *AggregateEntitiesGroup) GetKey() []AggregateEntitiesGroupKeyInner`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *AggregateEntitiesGroup) GetKeyOk() (*[]AggregateEntitiesGroupKeyInner, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *AggregateEntitiesGroup) SetKey(v []AggregateEntitiesGroupKeyInner)`

SetKey sets Key field to given value.


### GetAggregates

`func (o *AggregateEntitiesGroup) GetAggregates() []AggregateEntitiesGroupAggregatesInner`

GetAggregates returns the Aggregates field if non-nil, zero value otherwise.

### GetAggregatesOk

`func (o *AggregateEntitiesGroup) GetAggregatesOk() (*[]AggregateEntitiesGroupAggregatesInner, bool)`

GetAggregatesOk returns a tuple with the Aggregates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAggregates

`func (o *AggregateEntitiesGroup) SetAggregates(v []AggregateEntitiesGroupAggregatesInner)`

SetAggregates sets Aggregates field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


