# ResolvedChartBlockResponseSeriesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EntityId** | Pointer to **string** | Entity unique identifier | [optional] 
**EntityName** | Pointer to **NullableString** | Resolved display name of the entity | [optional] 
**DataPoints** | Pointer to [**[]ResolvedChartBlockResponseSeriesInnerDataPointsInner**](ResolvedChartBlockResponseSeriesInnerDataPointsInner.md) | Ordered array of time-bucketed metric points | [optional] 

## Methods

### NewResolvedChartBlockResponseSeriesInner

`func NewResolvedChartBlockResponseSeriesInner() *ResolvedChartBlockResponseSeriesInner`

NewResolvedChartBlockResponseSeriesInner instantiates a new ResolvedChartBlockResponseSeriesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResolvedChartBlockResponseSeriesInnerWithDefaults

`func NewResolvedChartBlockResponseSeriesInnerWithDefaults() *ResolvedChartBlockResponseSeriesInner`

NewResolvedChartBlockResponseSeriesInnerWithDefaults instantiates a new ResolvedChartBlockResponseSeriesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEntityId

`func (o *ResolvedChartBlockResponseSeriesInner) GetEntityId() string`

GetEntityId returns the EntityId field if non-nil, zero value otherwise.

### GetEntityIdOk

`func (o *ResolvedChartBlockResponseSeriesInner) GetEntityIdOk() (*string, bool)`

GetEntityIdOk returns a tuple with the EntityId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityId

`func (o *ResolvedChartBlockResponseSeriesInner) SetEntityId(v string)`

SetEntityId sets EntityId field to given value.

### HasEntityId

`func (o *ResolvedChartBlockResponseSeriesInner) HasEntityId() bool`

HasEntityId returns a boolean if a field has been set.

### GetEntityName

`func (o *ResolvedChartBlockResponseSeriesInner) GetEntityName() string`

GetEntityName returns the EntityName field if non-nil, zero value otherwise.

### GetEntityNameOk

`func (o *ResolvedChartBlockResponseSeriesInner) GetEntityNameOk() (*string, bool)`

GetEntityNameOk returns a tuple with the EntityName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityName

`func (o *ResolvedChartBlockResponseSeriesInner) SetEntityName(v string)`

SetEntityName sets EntityName field to given value.

### HasEntityName

`func (o *ResolvedChartBlockResponseSeriesInner) HasEntityName() bool`

HasEntityName returns a boolean if a field has been set.

### SetEntityNameNil

`func (o *ResolvedChartBlockResponseSeriesInner) SetEntityNameNil(b bool)`

 SetEntityNameNil sets the value for EntityName to be an explicit nil

### UnsetEntityName
`func (o *ResolvedChartBlockResponseSeriesInner) UnsetEntityName()`

UnsetEntityName ensures that no value is present for EntityName, not even an explicit nil
### GetDataPoints

`func (o *ResolvedChartBlockResponseSeriesInner) GetDataPoints() []ResolvedChartBlockResponseSeriesInnerDataPointsInner`

GetDataPoints returns the DataPoints field if non-nil, zero value otherwise.

### GetDataPointsOk

`func (o *ResolvedChartBlockResponseSeriesInner) GetDataPointsOk() (*[]ResolvedChartBlockResponseSeriesInnerDataPointsInner, bool)`

GetDataPointsOk returns a tuple with the DataPoints field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataPoints

`func (o *ResolvedChartBlockResponseSeriesInner) SetDataPoints(v []ResolvedChartBlockResponseSeriesInnerDataPointsInner)`

SetDataPoints sets DataPoints field to given value.

### HasDataPoints

`func (o *ResolvedChartBlockResponseSeriesInner) HasDataPoints() bool`

HasDataPoints returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


