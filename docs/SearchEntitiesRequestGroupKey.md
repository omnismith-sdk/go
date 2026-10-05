# SearchEntitiesRequestGroupKey

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Field** | **string** | Attribute slug or UUID | 
**Value** | [**NullableSearchEntitiesRequestGroupKeyValue**](SearchEntitiesRequestGroupKeyValue.md) |  | 

## Methods

### NewSearchEntitiesRequestGroupKey

`func NewSearchEntitiesRequestGroupKey(field string, value NullableSearchEntitiesRequestGroupKeyValue, ) *SearchEntitiesRequestGroupKey`

NewSearchEntitiesRequestGroupKey instantiates a new SearchEntitiesRequestGroupKey object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSearchEntitiesRequestGroupKeyWithDefaults

`func NewSearchEntitiesRequestGroupKeyWithDefaults() *SearchEntitiesRequestGroupKey`

NewSearchEntitiesRequestGroupKeyWithDefaults instantiates a new SearchEntitiesRequestGroupKey object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetField

`func (o *SearchEntitiesRequestGroupKey) GetField() string`

GetField returns the Field field if non-nil, zero value otherwise.

### GetFieldOk

`func (o *SearchEntitiesRequestGroupKey) GetFieldOk() (*string, bool)`

GetFieldOk returns a tuple with the Field field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetField

`func (o *SearchEntitiesRequestGroupKey) SetField(v string)`

SetField sets Field field to given value.


### GetValue

`func (o *SearchEntitiesRequestGroupKey) GetValue() SearchEntitiesRequestGroupKeyValue`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *SearchEntitiesRequestGroupKey) GetValueOk() (*SearchEntitiesRequestGroupKeyValue, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *SearchEntitiesRequestGroupKey) SetValue(v SearchEntitiesRequestGroupKeyValue)`

SetValue sets Value field to given value.


### SetValueNil

`func (o *SearchEntitiesRequestGroupKey) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *SearchEntitiesRequestGroupKey) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


