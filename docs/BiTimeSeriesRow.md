# BiTimeSeriesRow

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | Pointer to **string** | Template UUID | [optional] 
**EntityId** | Pointer to **string** | Entity UUID | [optional] 
**AttributeId** | Pointer to **string** | Metric attribute UUID | [optional] 
**AttributeName** | Pointer to **NullableString** | Metric attribute display name | [optional] 
**BucketTime** | Pointer to **time.Time** | Bucket start timestamp in ISO 8601 format | [optional] 
**Value** | Pointer to **float32** | Aggregated metric value for the time bucket | [optional] 

## Methods

### NewBiTimeSeriesRow

`func NewBiTimeSeriesRow() *BiTimeSeriesRow`

NewBiTimeSeriesRow instantiates a new BiTimeSeriesRow object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBiTimeSeriesRowWithDefaults

`func NewBiTimeSeriesRowWithDefaults() *BiTimeSeriesRow`

NewBiTimeSeriesRowWithDefaults instantiates a new BiTimeSeriesRow object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *BiTimeSeriesRow) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *BiTimeSeriesRow) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *BiTimeSeriesRow) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *BiTimeSeriesRow) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetEntityId

`func (o *BiTimeSeriesRow) GetEntityId() string`

GetEntityId returns the EntityId field if non-nil, zero value otherwise.

### GetEntityIdOk

`func (o *BiTimeSeriesRow) GetEntityIdOk() (*string, bool)`

GetEntityIdOk returns a tuple with the EntityId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityId

`func (o *BiTimeSeriesRow) SetEntityId(v string)`

SetEntityId sets EntityId field to given value.

### HasEntityId

`func (o *BiTimeSeriesRow) HasEntityId() bool`

HasEntityId returns a boolean if a field has been set.

### GetAttributeId

`func (o *BiTimeSeriesRow) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *BiTimeSeriesRow) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *BiTimeSeriesRow) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.

### HasAttributeId

`func (o *BiTimeSeriesRow) HasAttributeId() bool`

HasAttributeId returns a boolean if a field has been set.

### GetAttributeName

`func (o *BiTimeSeriesRow) GetAttributeName() string`

GetAttributeName returns the AttributeName field if non-nil, zero value otherwise.

### GetAttributeNameOk

`func (o *BiTimeSeriesRow) GetAttributeNameOk() (*string, bool)`

GetAttributeNameOk returns a tuple with the AttributeName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeName

`func (o *BiTimeSeriesRow) SetAttributeName(v string)`

SetAttributeName sets AttributeName field to given value.

### HasAttributeName

`func (o *BiTimeSeriesRow) HasAttributeName() bool`

HasAttributeName returns a boolean if a field has been set.

### SetAttributeNameNil

`func (o *BiTimeSeriesRow) SetAttributeNameNil(b bool)`

 SetAttributeNameNil sets the value for AttributeName to be an explicit nil

### UnsetAttributeName
`func (o *BiTimeSeriesRow) UnsetAttributeName()`

UnsetAttributeName ensures that no value is present for AttributeName, not even an explicit nil
### GetBucketTime

`func (o *BiTimeSeriesRow) GetBucketTime() time.Time`

GetBucketTime returns the BucketTime field if non-nil, zero value otherwise.

### GetBucketTimeOk

`func (o *BiTimeSeriesRow) GetBucketTimeOk() (*time.Time, bool)`

GetBucketTimeOk returns a tuple with the BucketTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBucketTime

`func (o *BiTimeSeriesRow) SetBucketTime(v time.Time)`

SetBucketTime sets BucketTime field to given value.

### HasBucketTime

`func (o *BiTimeSeriesRow) HasBucketTime() bool`

HasBucketTime returns a boolean if a field has been set.

### GetValue

`func (o *BiTimeSeriesRow) GetValue() float32`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *BiTimeSeriesRow) GetValueOk() (*float32, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *BiTimeSeriesRow) SetValue(v float32)`

SetValue sets Value field to given value.

### HasValue

`func (o *BiTimeSeriesRow) HasValue() bool`

HasValue returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


