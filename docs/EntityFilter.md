# EntityFilter

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Field** | **string** | Attribute slug or UUID, a standard field (&#x60;id&#x60;, &#x60;created_at&#x60;, &#x60;updated_at&#x60;, &#x60;external_key&#x60;), or a one-hop path through a reference attribute: &#x60;&lt;reference&gt;.&lt;attribute of its target template&gt;&#x60; (e.g. &#x60;customer.tier&#x60;). | 
**Operator** | **string** | eq, neq, gt, lt, like (case-insensitive substring), not-like, empty, not-empty, in, not-in, between | 
**Value** | Pointer to [**NullableEntityFilterValue**](EntityFilterValue.md) |  | [optional] 

## Methods

### NewEntityFilter

`func NewEntityFilter(field string, operator string, ) *EntityFilter`

NewEntityFilter instantiates a new EntityFilter object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityFilterWithDefaults

`func NewEntityFilterWithDefaults() *EntityFilter`

NewEntityFilterWithDefaults instantiates a new EntityFilter object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetField

`func (o *EntityFilter) GetField() string`

GetField returns the Field field if non-nil, zero value otherwise.

### GetFieldOk

`func (o *EntityFilter) GetFieldOk() (*string, bool)`

GetFieldOk returns a tuple with the Field field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetField

`func (o *EntityFilter) SetField(v string)`

SetField sets Field field to given value.


### GetOperator

`func (o *EntityFilter) GetOperator() string`

GetOperator returns the Operator field if non-nil, zero value otherwise.

### GetOperatorOk

`func (o *EntityFilter) GetOperatorOk() (*string, bool)`

GetOperatorOk returns a tuple with the Operator field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperator

`func (o *EntityFilter) SetOperator(v string)`

SetOperator sets Operator field to given value.


### GetValue

`func (o *EntityFilter) GetValue() EntityFilterValue`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *EntityFilter) GetValueOk() (*EntityFilterValue, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *EntityFilter) SetValue(v EntityFilterValue)`

SetValue sets Value field to given value.

### HasValue

`func (o *EntityFilter) HasValue() bool`

HasValue returns a boolean if a field has been set.

### SetValueNil

`func (o *EntityFilter) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *EntityFilter) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


