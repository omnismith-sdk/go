# AggregateEntitiesGroupKeyInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Field** | **string** | The group_by entry as sent | 
**Value** | [**NullableAggregateEntitiesGroupKeyInnerValue**](AggregateEntitiesGroupKeyInnerValue.md) |  | 
**CustomValue** | **NullableString** | The list item label or the referenced record&#39;s display value; null for other types | 

## Methods

### NewAggregateEntitiesGroupKeyInner

`func NewAggregateEntitiesGroupKeyInner(field string, value NullableAggregateEntitiesGroupKeyInnerValue, customValue NullableString, ) *AggregateEntitiesGroupKeyInner`

NewAggregateEntitiesGroupKeyInner instantiates a new AggregateEntitiesGroupKeyInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAggregateEntitiesGroupKeyInnerWithDefaults

`func NewAggregateEntitiesGroupKeyInnerWithDefaults() *AggregateEntitiesGroupKeyInner`

NewAggregateEntitiesGroupKeyInnerWithDefaults instantiates a new AggregateEntitiesGroupKeyInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetField

`func (o *AggregateEntitiesGroupKeyInner) GetField() string`

GetField returns the Field field if non-nil, zero value otherwise.

### GetFieldOk

`func (o *AggregateEntitiesGroupKeyInner) GetFieldOk() (*string, bool)`

GetFieldOk returns a tuple with the Field field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetField

`func (o *AggregateEntitiesGroupKeyInner) SetField(v string)`

SetField sets Field field to given value.


### GetValue

`func (o *AggregateEntitiesGroupKeyInner) GetValue() AggregateEntitiesGroupKeyInnerValue`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *AggregateEntitiesGroupKeyInner) GetValueOk() (*AggregateEntitiesGroupKeyInnerValue, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *AggregateEntitiesGroupKeyInner) SetValue(v AggregateEntitiesGroupKeyInnerValue)`

SetValue sets Value field to given value.


### SetValueNil

`func (o *AggregateEntitiesGroupKeyInner) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *AggregateEntitiesGroupKeyInner) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil
### GetCustomValue

`func (o *AggregateEntitiesGroupKeyInner) GetCustomValue() string`

GetCustomValue returns the CustomValue field if non-nil, zero value otherwise.

### GetCustomValueOk

`func (o *AggregateEntitiesGroupKeyInner) GetCustomValueOk() (*string, bool)`

GetCustomValueOk returns a tuple with the CustomValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomValue

`func (o *AggregateEntitiesGroupKeyInner) SetCustomValue(v string)`

SetCustomValue sets CustomValue field to given value.


### SetCustomValueNil

`func (o *AggregateEntitiesGroupKeyInner) SetCustomValueNil(b bool)`

 SetCustomValueNil sets the value for CustomValue to be an explicit nil

### UnsetCustomValue
`func (o *AggregateEntitiesGroupKeyInner) UnsetCustomValue()`

UnsetCustomValue ensures that no value is present for CustomValue, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


