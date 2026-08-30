# CreateDashboardBlockRequestConfigFiltersInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Field** | **string** |  | 
**Operator** | **string** |  | 
**Value** | Pointer to **NullableString** |  | [optional] 
**IsActive** | Pointer to **bool** |  | [optional] [default to true]

## Methods

### NewCreateDashboardBlockRequestConfigFiltersInner

`func NewCreateDashboardBlockRequestConfigFiltersInner(field string, operator string, ) *CreateDashboardBlockRequestConfigFiltersInner`

NewCreateDashboardBlockRequestConfigFiltersInner instantiates a new CreateDashboardBlockRequestConfigFiltersInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateDashboardBlockRequestConfigFiltersInnerWithDefaults

`func NewCreateDashboardBlockRequestConfigFiltersInnerWithDefaults() *CreateDashboardBlockRequestConfigFiltersInner`

NewCreateDashboardBlockRequestConfigFiltersInnerWithDefaults instantiates a new CreateDashboardBlockRequestConfigFiltersInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetField

`func (o *CreateDashboardBlockRequestConfigFiltersInner) GetField() string`

GetField returns the Field field if non-nil, zero value otherwise.

### GetFieldOk

`func (o *CreateDashboardBlockRequestConfigFiltersInner) GetFieldOk() (*string, bool)`

GetFieldOk returns a tuple with the Field field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetField

`func (o *CreateDashboardBlockRequestConfigFiltersInner) SetField(v string)`

SetField sets Field field to given value.


### GetOperator

`func (o *CreateDashboardBlockRequestConfigFiltersInner) GetOperator() string`

GetOperator returns the Operator field if non-nil, zero value otherwise.

### GetOperatorOk

`func (o *CreateDashboardBlockRequestConfigFiltersInner) GetOperatorOk() (*string, bool)`

GetOperatorOk returns a tuple with the Operator field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperator

`func (o *CreateDashboardBlockRequestConfigFiltersInner) SetOperator(v string)`

SetOperator sets Operator field to given value.


### GetValue

`func (o *CreateDashboardBlockRequestConfigFiltersInner) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *CreateDashboardBlockRequestConfigFiltersInner) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *CreateDashboardBlockRequestConfigFiltersInner) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *CreateDashboardBlockRequestConfigFiltersInner) HasValue() bool`

HasValue returns a boolean if a field has been set.

### SetValueNil

`func (o *CreateDashboardBlockRequestConfigFiltersInner) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *CreateDashboardBlockRequestConfigFiltersInner) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil
### GetIsActive

`func (o *CreateDashboardBlockRequestConfigFiltersInner) GetIsActive() bool`

GetIsActive returns the IsActive field if non-nil, zero value otherwise.

### GetIsActiveOk

`func (o *CreateDashboardBlockRequestConfigFiltersInner) GetIsActiveOk() (*bool, bool)`

GetIsActiveOk returns a tuple with the IsActive field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsActive

`func (o *CreateDashboardBlockRequestConfigFiltersInner) SetIsActive(v bool)`

SetIsActive sets IsActive field to given value.

### HasIsActive

`func (o *CreateDashboardBlockRequestConfigFiltersInner) HasIsActive() bool`

HasIsActive returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


