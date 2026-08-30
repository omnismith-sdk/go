# RoleEntityScopeConditionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Field** | Pointer to **string** | Attribute UUID or standard entity field (e.g. id, created_at) | [optional] 
**Operator** | Pointer to **string** | Comparison operator | [optional] 
**Value** | Pointer to **NullableString** | Comparison value | [optional] 

## Methods

### NewRoleEntityScopeConditionResponse

`func NewRoleEntityScopeConditionResponse() *RoleEntityScopeConditionResponse`

NewRoleEntityScopeConditionResponse instantiates a new RoleEntityScopeConditionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRoleEntityScopeConditionResponseWithDefaults

`func NewRoleEntityScopeConditionResponseWithDefaults() *RoleEntityScopeConditionResponse`

NewRoleEntityScopeConditionResponseWithDefaults instantiates a new RoleEntityScopeConditionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetField

`func (o *RoleEntityScopeConditionResponse) GetField() string`

GetField returns the Field field if non-nil, zero value otherwise.

### GetFieldOk

`func (o *RoleEntityScopeConditionResponse) GetFieldOk() (*string, bool)`

GetFieldOk returns a tuple with the Field field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetField

`func (o *RoleEntityScopeConditionResponse) SetField(v string)`

SetField sets Field field to given value.

### HasField

`func (o *RoleEntityScopeConditionResponse) HasField() bool`

HasField returns a boolean if a field has been set.

### GetOperator

`func (o *RoleEntityScopeConditionResponse) GetOperator() string`

GetOperator returns the Operator field if non-nil, zero value otherwise.

### GetOperatorOk

`func (o *RoleEntityScopeConditionResponse) GetOperatorOk() (*string, bool)`

GetOperatorOk returns a tuple with the Operator field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperator

`func (o *RoleEntityScopeConditionResponse) SetOperator(v string)`

SetOperator sets Operator field to given value.

### HasOperator

`func (o *RoleEntityScopeConditionResponse) HasOperator() bool`

HasOperator returns a boolean if a field has been set.

### GetValue

`func (o *RoleEntityScopeConditionResponse) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *RoleEntityScopeConditionResponse) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *RoleEntityScopeConditionResponse) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *RoleEntityScopeConditionResponse) HasValue() bool`

HasValue returns a boolean if a field has been set.

### SetValueNil

`func (o *RoleEntityScopeConditionResponse) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *RoleEntityScopeConditionResponse) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


