# UpdateAutomationRequestTrigger

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | Pointer to **string** | Trigger event type. &#x60;on_action_executed&#x60; fires when the named entity action runs on a record, whether or not the write changed anything. | [optional] 
**TemplateId** | Pointer to **NullableString** | Template UUID | [optional] 
**AttributeId** | Pointer to **NullableString** | Attribute UUID for attribute change triggers | [optional] 
**ActionId** | Pointer to **NullableString** | Entity action UUID; required for &#x60;on_action_executed&#x60;, must be null otherwise | [optional] 

## Methods

### NewUpdateAutomationRequestTrigger

`func NewUpdateAutomationRequestTrigger() *UpdateAutomationRequestTrigger`

NewUpdateAutomationRequestTrigger instantiates a new UpdateAutomationRequestTrigger object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateAutomationRequestTriggerWithDefaults

`func NewUpdateAutomationRequestTriggerWithDefaults() *UpdateAutomationRequestTrigger`

NewUpdateAutomationRequestTriggerWithDefaults instantiates a new UpdateAutomationRequestTrigger object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *UpdateAutomationRequestTrigger) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *UpdateAutomationRequestTrigger) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *UpdateAutomationRequestTrigger) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *UpdateAutomationRequestTrigger) HasType() bool`

HasType returns a boolean if a field has been set.

### GetTemplateId

`func (o *UpdateAutomationRequestTrigger) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *UpdateAutomationRequestTrigger) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *UpdateAutomationRequestTrigger) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *UpdateAutomationRequestTrigger) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### SetTemplateIdNil

`func (o *UpdateAutomationRequestTrigger) SetTemplateIdNil(b bool)`

 SetTemplateIdNil sets the value for TemplateId to be an explicit nil

### UnsetTemplateId
`func (o *UpdateAutomationRequestTrigger) UnsetTemplateId()`

UnsetTemplateId ensures that no value is present for TemplateId, not even an explicit nil
### GetAttributeId

`func (o *UpdateAutomationRequestTrigger) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *UpdateAutomationRequestTrigger) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *UpdateAutomationRequestTrigger) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.

### HasAttributeId

`func (o *UpdateAutomationRequestTrigger) HasAttributeId() bool`

HasAttributeId returns a boolean if a field has been set.

### SetAttributeIdNil

`func (o *UpdateAutomationRequestTrigger) SetAttributeIdNil(b bool)`

 SetAttributeIdNil sets the value for AttributeId to be an explicit nil

### UnsetAttributeId
`func (o *UpdateAutomationRequestTrigger) UnsetAttributeId()`

UnsetAttributeId ensures that no value is present for AttributeId, not even an explicit nil
### GetActionId

`func (o *UpdateAutomationRequestTrigger) GetActionId() string`

GetActionId returns the ActionId field if non-nil, zero value otherwise.

### GetActionIdOk

`func (o *UpdateAutomationRequestTrigger) GetActionIdOk() (*string, bool)`

GetActionIdOk returns a tuple with the ActionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionId

`func (o *UpdateAutomationRequestTrigger) SetActionId(v string)`

SetActionId sets ActionId field to given value.

### HasActionId

`func (o *UpdateAutomationRequestTrigger) HasActionId() bool`

HasActionId returns a boolean if a field has been set.

### SetActionIdNil

`func (o *UpdateAutomationRequestTrigger) SetActionIdNil(b bool)`

 SetActionIdNil sets the value for ActionId to be an explicit nil

### UnsetActionId
`func (o *UpdateAutomationRequestTrigger) UnsetActionId()`

UnsetActionId ensures that no value is present for ActionId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


