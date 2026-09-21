# AggregateEntities200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | [**[]AggregateEntitiesGroup**](AggregateEntitiesGroup.md) |  | 
**Limit** | **int32** | The group cap that was applied | 
**Truncated** | **bool** | True when more groups exist than were returned | 

## Methods

### NewAggregateEntities200Response

`func NewAggregateEntities200Response(data []AggregateEntitiesGroup, limit int32, truncated bool, ) *AggregateEntities200Response`

NewAggregateEntities200Response instantiates a new AggregateEntities200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAggregateEntities200ResponseWithDefaults

`func NewAggregateEntities200ResponseWithDefaults() *AggregateEntities200Response`

NewAggregateEntities200ResponseWithDefaults instantiates a new AggregateEntities200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *AggregateEntities200Response) GetData() []AggregateEntitiesGroup`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *AggregateEntities200Response) GetDataOk() (*[]AggregateEntitiesGroup, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *AggregateEntities200Response) SetData(v []AggregateEntitiesGroup)`

SetData sets Data field to given value.


### GetLimit

`func (o *AggregateEntities200Response) GetLimit() int32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *AggregateEntities200Response) GetLimitOk() (*int32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *AggregateEntities200Response) SetLimit(v int32)`

SetLimit sets Limit field to given value.


### GetTruncated

`func (o *AggregateEntities200Response) GetTruncated() bool`

GetTruncated returns the Truncated field if non-nil, zero value otherwise.

### GetTruncatedOk

`func (o *AggregateEntities200Response) GetTruncatedOk() (*bool, bool)`

GetTruncatedOk returns a tuple with the Truncated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTruncated

`func (o *AggregateEntities200Response) SetTruncated(v bool)`

SetTruncated sets Truncated field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


