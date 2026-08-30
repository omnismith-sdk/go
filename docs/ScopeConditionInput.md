# ScopeConditionInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Field** | **string** | Attribute id or a standard entity field (id, created_at, updated_at) | 
**Operator** | **string** |  | 
**Value** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewScopeConditionInput

`func NewScopeConditionInput(field string, operator string, ) *ScopeConditionInput`

NewScopeConditionInput instantiates a new ScopeConditionInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScopeConditionInputWithDefaults

`func NewScopeConditionInputWithDefaults() *ScopeConditionInput`

NewScopeConditionInputWithDefaults instantiates a new ScopeConditionInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetField

`func (o *ScopeConditionInput) GetField() string`

GetField returns the Field field if non-nil, zero value otherwise.

### GetFieldOk

`func (o *ScopeConditionInput) GetFieldOk() (*string, bool)`

GetFieldOk returns a tuple with the Field field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetField

`func (o *ScopeConditionInput) SetField(v string)`

SetField sets Field field to given value.


### GetOperator

`func (o *ScopeConditionInput) GetOperator() string`

GetOperator returns the Operator field if non-nil, zero value otherwise.

### GetOperatorOk

`func (o *ScopeConditionInput) GetOperatorOk() (*string, bool)`

GetOperatorOk returns a tuple with the Operator field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperator

`func (o *ScopeConditionInput) SetOperator(v string)`

SetOperator sets Operator field to given value.


### GetValue

`func (o *ScopeConditionInput) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *ScopeConditionInput) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *ScopeConditionInput) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *ScopeConditionInput) HasValue() bool`

HasValue returns a boolean if a field has been set.

### SetValueNil

`func (o *ScopeConditionInput) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *ScopeConditionInput) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


