# CreateAutomationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**Description** | Pointer to **NullableString** |  | [optional] 
**Trigger** | [**CreateAutomationRequestTrigger**](CreateAutomationRequestTrigger.md) |  | 
**Conditions** | [**[]CreateAutomationRequestConditionsInner**](CreateAutomationRequestConditionsInner.md) |  | 
**Actions** | [**[]CreateAutomationRequestActionsInner**](CreateAutomationRequestActionsInner.md) |  | 
**CooldownSeconds** | Pointer to **NullableInt32** |  | [optional] 

## Methods

### NewCreateAutomationRequest

`func NewCreateAutomationRequest(name string, trigger CreateAutomationRequestTrigger, conditions []CreateAutomationRequestConditionsInner, actions []CreateAutomationRequestActionsInner, ) *CreateAutomationRequest`

NewCreateAutomationRequest instantiates a new CreateAutomationRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateAutomationRequestWithDefaults

`func NewCreateAutomationRequestWithDefaults() *CreateAutomationRequest`

NewCreateAutomationRequestWithDefaults instantiates a new CreateAutomationRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreateAutomationRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateAutomationRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateAutomationRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *CreateAutomationRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateAutomationRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateAutomationRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CreateAutomationRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *CreateAutomationRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *CreateAutomationRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetTrigger

`func (o *CreateAutomationRequest) GetTrigger() CreateAutomationRequestTrigger`

GetTrigger returns the Trigger field if non-nil, zero value otherwise.

### GetTriggerOk

`func (o *CreateAutomationRequest) GetTriggerOk() (*CreateAutomationRequestTrigger, bool)`

GetTriggerOk returns a tuple with the Trigger field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrigger

`func (o *CreateAutomationRequest) SetTrigger(v CreateAutomationRequestTrigger)`

SetTrigger sets Trigger field to given value.


### GetConditions

`func (o *CreateAutomationRequest) GetConditions() []CreateAutomationRequestConditionsInner`

GetConditions returns the Conditions field if non-nil, zero value otherwise.

### GetConditionsOk

`func (o *CreateAutomationRequest) GetConditionsOk() (*[]CreateAutomationRequestConditionsInner, bool)`

GetConditionsOk returns a tuple with the Conditions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConditions

`func (o *CreateAutomationRequest) SetConditions(v []CreateAutomationRequestConditionsInner)`

SetConditions sets Conditions field to given value.


### GetActions

`func (o *CreateAutomationRequest) GetActions() []CreateAutomationRequestActionsInner`

GetActions returns the Actions field if non-nil, zero value otherwise.

### GetActionsOk

`func (o *CreateAutomationRequest) GetActionsOk() (*[]CreateAutomationRequestActionsInner, bool)`

GetActionsOk returns a tuple with the Actions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActions

`func (o *CreateAutomationRequest) SetActions(v []CreateAutomationRequestActionsInner)`

SetActions sets Actions field to given value.


### GetCooldownSeconds

`func (o *CreateAutomationRequest) GetCooldownSeconds() int32`

GetCooldownSeconds returns the CooldownSeconds field if non-nil, zero value otherwise.

### GetCooldownSecondsOk

`func (o *CreateAutomationRequest) GetCooldownSecondsOk() (*int32, bool)`

GetCooldownSecondsOk returns a tuple with the CooldownSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCooldownSeconds

`func (o *CreateAutomationRequest) SetCooldownSeconds(v int32)`

SetCooldownSeconds sets CooldownSeconds field to given value.

### HasCooldownSeconds

`func (o *CreateAutomationRequest) HasCooldownSeconds() bool`

HasCooldownSeconds returns a boolean if a field has been set.

### SetCooldownSecondsNil

`func (o *CreateAutomationRequest) SetCooldownSecondsNil(b bool)`

 SetCooldownSecondsNil sets the value for CooldownSeconds to be an explicit nil

### UnsetCooldownSeconds
`func (o *CreateAutomationRequest) UnsetCooldownSeconds()`

UnsetCooldownSeconds ensures that no value is present for CooldownSeconds, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


