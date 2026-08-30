# CreateAutomationRequestConditionsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | **string** | Attribute UUID to evaluate | 
**Operator** | **string** | Comparison operator | 
**Value** | Pointer to **interface{}** | Expected comparison value | [optional] 
**Mode** | **string** | Evaluation mode: current value, absolute numeric change, or percentage change | 

## Methods

### NewCreateAutomationRequestConditionsInner

`func NewCreateAutomationRequestConditionsInner(attributeId string, operator string, mode string, ) *CreateAutomationRequestConditionsInner`

NewCreateAutomationRequestConditionsInner instantiates a new CreateAutomationRequestConditionsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateAutomationRequestConditionsInnerWithDefaults

`func NewCreateAutomationRequestConditionsInnerWithDefaults() *CreateAutomationRequestConditionsInner`

NewCreateAutomationRequestConditionsInnerWithDefaults instantiates a new CreateAutomationRequestConditionsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeId

`func (o *CreateAutomationRequestConditionsInner) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *CreateAutomationRequestConditionsInner) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *CreateAutomationRequestConditionsInner) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.


### GetOperator

`func (o *CreateAutomationRequestConditionsInner) GetOperator() string`

GetOperator returns the Operator field if non-nil, zero value otherwise.

### GetOperatorOk

`func (o *CreateAutomationRequestConditionsInner) GetOperatorOk() (*string, bool)`

GetOperatorOk returns a tuple with the Operator field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperator

`func (o *CreateAutomationRequestConditionsInner) SetOperator(v string)`

SetOperator sets Operator field to given value.


### GetValue

`func (o *CreateAutomationRequestConditionsInner) GetValue() interface{}`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *CreateAutomationRequestConditionsInner) GetValueOk() (*interface{}, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *CreateAutomationRequestConditionsInner) SetValue(v interface{})`

SetValue sets Value field to given value.

### HasValue

`func (o *CreateAutomationRequestConditionsInner) HasValue() bool`

HasValue returns a boolean if a field has been set.

### SetValueNil

`func (o *CreateAutomationRequestConditionsInner) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *CreateAutomationRequestConditionsInner) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil
### GetMode

`func (o *CreateAutomationRequestConditionsInner) GetMode() string`

GetMode returns the Mode field if non-nil, zero value otherwise.

### GetModeOk

`func (o *CreateAutomationRequestConditionsInner) GetModeOk() (*string, bool)`

GetModeOk returns a tuple with the Mode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMode

`func (o *CreateAutomationRequestConditionsInner) SetMode(v string)`

SetMode sets Mode field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


