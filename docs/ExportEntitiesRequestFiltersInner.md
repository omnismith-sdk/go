# ExportEntitiesRequestFiltersInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Field** | Pointer to **string** | Attribute UUID, attribute slug, or standard field (id, created_at, updated_at) | [optional] 
**Operator** | Pointer to **string** | Filter comparison operator: eq, neq, gt, lt, like, not-like, empty, not-empty | [optional] 
**Value** | Pointer to **NullableString** | Comparison value serialized as string | [optional] 

## Methods

### NewExportEntitiesRequestFiltersInner

`func NewExportEntitiesRequestFiltersInner() *ExportEntitiesRequestFiltersInner`

NewExportEntitiesRequestFiltersInner instantiates a new ExportEntitiesRequestFiltersInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExportEntitiesRequestFiltersInnerWithDefaults

`func NewExportEntitiesRequestFiltersInnerWithDefaults() *ExportEntitiesRequestFiltersInner`

NewExportEntitiesRequestFiltersInnerWithDefaults instantiates a new ExportEntitiesRequestFiltersInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetField

`func (o *ExportEntitiesRequestFiltersInner) GetField() string`

GetField returns the Field field if non-nil, zero value otherwise.

### GetFieldOk

`func (o *ExportEntitiesRequestFiltersInner) GetFieldOk() (*string, bool)`

GetFieldOk returns a tuple with the Field field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetField

`func (o *ExportEntitiesRequestFiltersInner) SetField(v string)`

SetField sets Field field to given value.

### HasField

`func (o *ExportEntitiesRequestFiltersInner) HasField() bool`

HasField returns a boolean if a field has been set.

### GetOperator

`func (o *ExportEntitiesRequestFiltersInner) GetOperator() string`

GetOperator returns the Operator field if non-nil, zero value otherwise.

### GetOperatorOk

`func (o *ExportEntitiesRequestFiltersInner) GetOperatorOk() (*string, bool)`

GetOperatorOk returns a tuple with the Operator field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperator

`func (o *ExportEntitiesRequestFiltersInner) SetOperator(v string)`

SetOperator sets Operator field to given value.

### HasOperator

`func (o *ExportEntitiesRequestFiltersInner) HasOperator() bool`

HasOperator returns a boolean if a field has been set.

### GetValue

`func (o *ExportEntitiesRequestFiltersInner) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *ExportEntitiesRequestFiltersInner) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *ExportEntitiesRequestFiltersInner) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *ExportEntitiesRequestFiltersInner) HasValue() bool`

HasValue returns a boolean if a field has been set.

### SetValueNil

`func (o *ExportEntitiesRequestFiltersInner) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *ExportEntitiesRequestFiltersInner) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


