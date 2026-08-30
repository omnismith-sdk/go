# UpdateAutomationRequestConditionsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | Pointer to **string** | Attribute UUID to evaluate | [optional] 
**Operator** | Pointer to **string** | Comparison operator | [optional] 
**Value** | Pointer to **interface{}** | Expected comparison value | [optional] 
**Mode** | Pointer to **string** | Evaluation mode: current value, absolute numeric change, or percentage change | [optional] 

## Methods

### NewUpdateAutomationRequestConditionsInner

`func NewUpdateAutomationRequestConditionsInner() *UpdateAutomationRequestConditionsInner`

NewUpdateAutomationRequestConditionsInner instantiates a new UpdateAutomationRequestConditionsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateAutomationRequestConditionsInnerWithDefaults

`func NewUpdateAutomationRequestConditionsInnerWithDefaults() *UpdateAutomationRequestConditionsInner`

NewUpdateAutomationRequestConditionsInnerWithDefaults instantiates a new UpdateAutomationRequestConditionsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeId

`func (o *UpdateAutomationRequestConditionsInner) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *UpdateAutomationRequestConditionsInner) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *UpdateAutomationRequestConditionsInner) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.

### HasAttributeId

`func (o *UpdateAutomationRequestConditionsInner) HasAttributeId() bool`

HasAttributeId returns a boolean if a field has been set.

### GetOperator

`func (o *UpdateAutomationRequestConditionsInner) GetOperator() string`

GetOperator returns the Operator field if non-nil, zero value otherwise.

### GetOperatorOk

`func (o *UpdateAutomationRequestConditionsInner) GetOperatorOk() (*string, bool)`

GetOperatorOk returns a tuple with the Operator field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperator

`func (o *UpdateAutomationRequestConditionsInner) SetOperator(v string)`

SetOperator sets Operator field to given value.

### HasOperator

`func (o *UpdateAutomationRequestConditionsInner) HasOperator() bool`

HasOperator returns a boolean if a field has been set.

### GetValue

`func (o *UpdateAutomationRequestConditionsInner) GetValue() interface{}`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *UpdateAutomationRequestConditionsInner) GetValueOk() (*interface{}, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *UpdateAutomationRequestConditionsInner) SetValue(v interface{})`

SetValue sets Value field to given value.

### HasValue

`func (o *UpdateAutomationRequestConditionsInner) HasValue() bool`

HasValue returns a boolean if a field has been set.

### SetValueNil

`func (o *UpdateAutomationRequestConditionsInner) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *UpdateAutomationRequestConditionsInner) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil
### GetMode

`func (o *UpdateAutomationRequestConditionsInner) GetMode() string`

GetMode returns the Mode field if non-nil, zero value otherwise.

### GetModeOk

`func (o *UpdateAutomationRequestConditionsInner) GetModeOk() (*string, bool)`

GetModeOk returns a tuple with the Mode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMode

`func (o *UpdateAutomationRequestConditionsInner) SetMode(v string)`

SetMode sets Mode field to given value.

### HasMode

`func (o *UpdateAutomationRequestConditionsInner) HasMode() bool`

HasMode returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


