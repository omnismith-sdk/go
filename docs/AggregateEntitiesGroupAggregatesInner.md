# AggregateEntitiesGroupAggregatesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Op** | **string** |  | 
**Field** | **NullableString** | The aggregation field as sent; null for count | 
**Value** | [**NullableAggregateEntitiesGroupAggregatesInnerValue**](AggregateEntitiesGroupAggregatesInnerValue.md) |  | 

## Methods

### NewAggregateEntitiesGroupAggregatesInner

`func NewAggregateEntitiesGroupAggregatesInner(op string, field NullableString, value NullableAggregateEntitiesGroupAggregatesInnerValue, ) *AggregateEntitiesGroupAggregatesInner`

NewAggregateEntitiesGroupAggregatesInner instantiates a new AggregateEntitiesGroupAggregatesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAggregateEntitiesGroupAggregatesInnerWithDefaults

`func NewAggregateEntitiesGroupAggregatesInnerWithDefaults() *AggregateEntitiesGroupAggregatesInner`

NewAggregateEntitiesGroupAggregatesInnerWithDefaults instantiates a new AggregateEntitiesGroupAggregatesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOp

`func (o *AggregateEntitiesGroupAggregatesInner) GetOp() string`

GetOp returns the Op field if non-nil, zero value otherwise.

### GetOpOk

`func (o *AggregateEntitiesGroupAggregatesInner) GetOpOk() (*string, bool)`

GetOpOk returns a tuple with the Op field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOp

`func (o *AggregateEntitiesGroupAggregatesInner) SetOp(v string)`

SetOp sets Op field to given value.


### GetField

`func (o *AggregateEntitiesGroupAggregatesInner) GetField() string`

GetField returns the Field field if non-nil, zero value otherwise.

### GetFieldOk

`func (o *AggregateEntitiesGroupAggregatesInner) GetFieldOk() (*string, bool)`

GetFieldOk returns a tuple with the Field field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetField

`func (o *AggregateEntitiesGroupAggregatesInner) SetField(v string)`

SetField sets Field field to given value.


### SetFieldNil

`func (o *AggregateEntitiesGroupAggregatesInner) SetFieldNil(b bool)`

 SetFieldNil sets the value for Field to be an explicit nil

### UnsetField
`func (o *AggregateEntitiesGroupAggregatesInner) UnsetField()`

UnsetField ensures that no value is present for Field, not even an explicit nil
### GetValue

`func (o *AggregateEntitiesGroupAggregatesInner) GetValue() AggregateEntitiesGroupAggregatesInnerValue`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *AggregateEntitiesGroupAggregatesInner) GetValueOk() (*AggregateEntitiesGroupAggregatesInnerValue, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *AggregateEntitiesGroupAggregatesInner) SetValue(v AggregateEntitiesGroupAggregatesInnerValue)`

SetValue sets Value field to given value.


### SetValueNil

`func (o *AggregateEntitiesGroupAggregatesInner) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *AggregateEntitiesGroupAggregatesInner) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


