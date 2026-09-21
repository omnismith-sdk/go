# AutomationResponseTrigger

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | Pointer to **string** | Trigger event type. &#x60;on_action_executed&#x60; fires when the named entity action runs on a record, whether or not the write changed anything. | [optional] 
**TemplateId** | Pointer to **NullableString** | Target template UUID | [optional] 
**AttributeId** | Pointer to **NullableString** | Target attribute UUID for attribute change triggers | [optional] 
**ActionId** | Pointer to **NullableString** | Entity action UUID; required for &#x60;on_action_executed&#x60;, must be null otherwise | [optional] 

## Methods

### NewAutomationResponseTrigger

`func NewAutomationResponseTrigger() *AutomationResponseTrigger`

NewAutomationResponseTrigger instantiates a new AutomationResponseTrigger object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAutomationResponseTriggerWithDefaults

`func NewAutomationResponseTriggerWithDefaults() *AutomationResponseTrigger`

NewAutomationResponseTriggerWithDefaults instantiates a new AutomationResponseTrigger object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *AutomationResponseTrigger) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *AutomationResponseTrigger) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *AutomationResponseTrigger) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *AutomationResponseTrigger) HasType() bool`

HasType returns a boolean if a field has been set.

### GetTemplateId

`func (o *AutomationResponseTrigger) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *AutomationResponseTrigger) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *AutomationResponseTrigger) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *AutomationResponseTrigger) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### SetTemplateIdNil

`func (o *AutomationResponseTrigger) SetTemplateIdNil(b bool)`

 SetTemplateIdNil sets the value for TemplateId to be an explicit nil

### UnsetTemplateId
`func (o *AutomationResponseTrigger) UnsetTemplateId()`

UnsetTemplateId ensures that no value is present for TemplateId, not even an explicit nil
### GetAttributeId

`func (o *AutomationResponseTrigger) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *AutomationResponseTrigger) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *AutomationResponseTrigger) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.

### HasAttributeId

`func (o *AutomationResponseTrigger) HasAttributeId() bool`

HasAttributeId returns a boolean if a field has been set.

### SetAttributeIdNil

`func (o *AutomationResponseTrigger) SetAttributeIdNil(b bool)`

 SetAttributeIdNil sets the value for AttributeId to be an explicit nil

### UnsetAttributeId
`func (o *AutomationResponseTrigger) UnsetAttributeId()`

UnsetAttributeId ensures that no value is present for AttributeId, not even an explicit nil
### GetActionId

`func (o *AutomationResponseTrigger) GetActionId() string`

GetActionId returns the ActionId field if non-nil, zero value otherwise.

### GetActionIdOk

`func (o *AutomationResponseTrigger) GetActionIdOk() (*string, bool)`

GetActionIdOk returns a tuple with the ActionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionId

`func (o *AutomationResponseTrigger) SetActionId(v string)`

SetActionId sets ActionId field to given value.

### HasActionId

`func (o *AutomationResponseTrigger) HasActionId() bool`

HasActionId returns a boolean if a field has been set.

### SetActionIdNil

`func (o *AutomationResponseTrigger) SetActionIdNil(b bool)`

 SetActionIdNil sets the value for ActionId to be an explicit nil

### UnsetActionId
`func (o *AutomationResponseTrigger) UnsetActionId()`

UnsetActionId ensures that no value is present for ActionId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


