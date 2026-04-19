# UpdateAutomationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **NullableString** |  | [optional] 
**Description** | Pointer to **NullableString** |  | [optional] 
**Trigger** | Pointer to [**NullableUpdateAutomationRequestTrigger**](UpdateAutomationRequestTrigger.md) |  | [optional] 
**Conditions** | Pointer to [**[]AutomationResponseConditionsInner**](AutomationResponseConditionsInner.md) |  | [optional] 
**Actions** | Pointer to [**[]AutomationResponseActionsInner**](AutomationResponseActionsInner.md) |  | [optional] 
**CooldownSeconds** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewUpdateAutomationRequest

`func NewUpdateAutomationRequest() *UpdateAutomationRequest`

NewUpdateAutomationRequest instantiates a new UpdateAutomationRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateAutomationRequestWithDefaults

`func NewUpdateAutomationRequestWithDefaults() *UpdateAutomationRequest`

NewUpdateAutomationRequestWithDefaults instantiates a new UpdateAutomationRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *UpdateAutomationRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateAutomationRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateAutomationRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *UpdateAutomationRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *UpdateAutomationRequest) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *UpdateAutomationRequest) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetDescription

`func (o *UpdateAutomationRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *UpdateAutomationRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *UpdateAutomationRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *UpdateAutomationRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *UpdateAutomationRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *UpdateAutomationRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetTrigger

`func (o *UpdateAutomationRequest) GetTrigger() UpdateAutomationRequestTrigger`

GetTrigger returns the Trigger field if non-nil, zero value otherwise.

### GetTriggerOk

`func (o *UpdateAutomationRequest) GetTriggerOk() (*UpdateAutomationRequestTrigger, bool)`

GetTriggerOk returns a tuple with the Trigger field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrigger

`func (o *UpdateAutomationRequest) SetTrigger(v UpdateAutomationRequestTrigger)`

SetTrigger sets Trigger field to given value.

### HasTrigger

`func (o *UpdateAutomationRequest) HasTrigger() bool`

HasTrigger returns a boolean if a field has been set.

### SetTriggerNil

`func (o *UpdateAutomationRequest) SetTriggerNil(b bool)`

 SetTriggerNil sets the value for Trigger to be an explicit nil

### UnsetTrigger
`func (o *UpdateAutomationRequest) UnsetTrigger()`

UnsetTrigger ensures that no value is present for Trigger, not even an explicit nil
### GetConditions

`func (o *UpdateAutomationRequest) GetConditions() []AutomationResponseConditionsInner`

GetConditions returns the Conditions field if non-nil, zero value otherwise.

### GetConditionsOk

`func (o *UpdateAutomationRequest) GetConditionsOk() (*[]AutomationResponseConditionsInner, bool)`

GetConditionsOk returns a tuple with the Conditions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConditions

`func (o *UpdateAutomationRequest) SetConditions(v []AutomationResponseConditionsInner)`

SetConditions sets Conditions field to given value.

### HasConditions

`func (o *UpdateAutomationRequest) HasConditions() bool`

HasConditions returns a boolean if a field has been set.

### SetConditionsNil

`func (o *UpdateAutomationRequest) SetConditionsNil(b bool)`

 SetConditionsNil sets the value for Conditions to be an explicit nil

### UnsetConditions
`func (o *UpdateAutomationRequest) UnsetConditions()`

UnsetConditions ensures that no value is present for Conditions, not even an explicit nil
### GetActions

`func (o *UpdateAutomationRequest) GetActions() []AutomationResponseActionsInner`

GetActions returns the Actions field if non-nil, zero value otherwise.

### GetActionsOk

`func (o *UpdateAutomationRequest) GetActionsOk() (*[]AutomationResponseActionsInner, bool)`

GetActionsOk returns a tuple with the Actions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActions

`func (o *UpdateAutomationRequest) SetActions(v []AutomationResponseActionsInner)`

SetActions sets Actions field to given value.

### HasActions

`func (o *UpdateAutomationRequest) HasActions() bool`

HasActions returns a boolean if a field has been set.

### SetActionsNil

`func (o *UpdateAutomationRequest) SetActionsNil(b bool)`

 SetActionsNil sets the value for Actions to be an explicit nil

### UnsetActions
`func (o *UpdateAutomationRequest) UnsetActions()`

UnsetActions ensures that no value is present for Actions, not even an explicit nil
### GetCooldownSeconds

`func (o *UpdateAutomationRequest) GetCooldownSeconds() int32`

GetCooldownSeconds returns the CooldownSeconds field if non-nil, zero value otherwise.

### GetCooldownSecondsOk

`func (o *UpdateAutomationRequest) GetCooldownSecondsOk() (*int32, bool)`

GetCooldownSecondsOk returns a tuple with the CooldownSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCooldownSeconds

`func (o *UpdateAutomationRequest) SetCooldownSeconds(v int32)`

SetCooldownSeconds sets CooldownSeconds field to given value.

### HasCooldownSeconds

`func (o *UpdateAutomationRequest) HasCooldownSeconds() bool`

HasCooldownSeconds returns a boolean if a field has been set.

### SetCooldownSecondsNil

`func (o *UpdateAutomationRequest) SetCooldownSecondsNil(b bool)`

 SetCooldownSecondsNil sets the value for CooldownSeconds to be an explicit nil

### UnsetCooldownSeconds
`func (o *UpdateAutomationRequest) UnsetCooldownSeconds()`

UnsetCooldownSeconds ensures that no value is present for CooldownSeconds, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


