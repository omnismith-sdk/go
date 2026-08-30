# AutomationResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Unique automation UUID | [optional] 
**Name** | Pointer to **string** | Name of the automation rule | [optional] 
**Description** | Pointer to **NullableString** | Optional description of the automation rule | [optional] 
**IsEnabled** | Pointer to **bool** | Whether the automation is currently active and listening for events | [optional] 
**Trigger** | Pointer to [**AutomationResponseTrigger**](AutomationResponseTrigger.md) |  | [optional] 
**Conditions** | Pointer to [**[]AutomationResponseConditionsInner**](AutomationResponseConditionsInner.md) | Condition expressions that must all evaluate to true to execute actions | [optional] 
**Actions** | Pointer to [**[]AutomationResponseActionsInner**](AutomationResponseActionsInner.md) | Actions dispatched when conditions evaluate to true | [optional] 
**CooldownSeconds** | Pointer to **NullableInt32** | Minimum cooldown seconds between trigger firings for the same entity | [optional] 
**LastTriggeredAt** | Pointer to **NullableTime** | Timestamp when this automation last fired | [optional] 
**CreatedAt** | Pointer to **time.Time** | Creation timestamp | [optional] 
**UpdatedAt** | Pointer to **time.Time** | Last update timestamp | [optional] 

## Methods

### NewAutomationResponse

`func NewAutomationResponse() *AutomationResponse`

NewAutomationResponse instantiates a new AutomationResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAutomationResponseWithDefaults

`func NewAutomationResponseWithDefaults() *AutomationResponse`

NewAutomationResponseWithDefaults instantiates a new AutomationResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *AutomationResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AutomationResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AutomationResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *AutomationResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *AutomationResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *AutomationResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *AutomationResponse) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *AutomationResponse) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *AutomationResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *AutomationResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *AutomationResponse) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *AutomationResponse) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *AutomationResponse) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *AutomationResponse) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetIsEnabled

`func (o *AutomationResponse) GetIsEnabled() bool`

GetIsEnabled returns the IsEnabled field if non-nil, zero value otherwise.

### GetIsEnabledOk

`func (o *AutomationResponse) GetIsEnabledOk() (*bool, bool)`

GetIsEnabledOk returns a tuple with the IsEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsEnabled

`func (o *AutomationResponse) SetIsEnabled(v bool)`

SetIsEnabled sets IsEnabled field to given value.

### HasIsEnabled

`func (o *AutomationResponse) HasIsEnabled() bool`

HasIsEnabled returns a boolean if a field has been set.

### GetTrigger

`func (o *AutomationResponse) GetTrigger() AutomationResponseTrigger`

GetTrigger returns the Trigger field if non-nil, zero value otherwise.

### GetTriggerOk

`func (o *AutomationResponse) GetTriggerOk() (*AutomationResponseTrigger, bool)`

GetTriggerOk returns a tuple with the Trigger field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTrigger

`func (o *AutomationResponse) SetTrigger(v AutomationResponseTrigger)`

SetTrigger sets Trigger field to given value.

### HasTrigger

`func (o *AutomationResponse) HasTrigger() bool`

HasTrigger returns a boolean if a field has been set.

### GetConditions

`func (o *AutomationResponse) GetConditions() []AutomationResponseConditionsInner`

GetConditions returns the Conditions field if non-nil, zero value otherwise.

### GetConditionsOk

`func (o *AutomationResponse) GetConditionsOk() (*[]AutomationResponseConditionsInner, bool)`

GetConditionsOk returns a tuple with the Conditions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConditions

`func (o *AutomationResponse) SetConditions(v []AutomationResponseConditionsInner)`

SetConditions sets Conditions field to given value.

### HasConditions

`func (o *AutomationResponse) HasConditions() bool`

HasConditions returns a boolean if a field has been set.

### GetActions

`func (o *AutomationResponse) GetActions() []AutomationResponseActionsInner`

GetActions returns the Actions field if non-nil, zero value otherwise.

### GetActionsOk

`func (o *AutomationResponse) GetActionsOk() (*[]AutomationResponseActionsInner, bool)`

GetActionsOk returns a tuple with the Actions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActions

`func (o *AutomationResponse) SetActions(v []AutomationResponseActionsInner)`

SetActions sets Actions field to given value.

### HasActions

`func (o *AutomationResponse) HasActions() bool`

HasActions returns a boolean if a field has been set.

### GetCooldownSeconds

`func (o *AutomationResponse) GetCooldownSeconds() int32`

GetCooldownSeconds returns the CooldownSeconds field if non-nil, zero value otherwise.

### GetCooldownSecondsOk

`func (o *AutomationResponse) GetCooldownSecondsOk() (*int32, bool)`

GetCooldownSecondsOk returns a tuple with the CooldownSeconds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCooldownSeconds

`func (o *AutomationResponse) SetCooldownSeconds(v int32)`

SetCooldownSeconds sets CooldownSeconds field to given value.

### HasCooldownSeconds

`func (o *AutomationResponse) HasCooldownSeconds() bool`

HasCooldownSeconds returns a boolean if a field has been set.

### SetCooldownSecondsNil

`func (o *AutomationResponse) SetCooldownSecondsNil(b bool)`

 SetCooldownSecondsNil sets the value for CooldownSeconds to be an explicit nil

### UnsetCooldownSeconds
`func (o *AutomationResponse) UnsetCooldownSeconds()`

UnsetCooldownSeconds ensures that no value is present for CooldownSeconds, not even an explicit nil
### GetLastTriggeredAt

`func (o *AutomationResponse) GetLastTriggeredAt() time.Time`

GetLastTriggeredAt returns the LastTriggeredAt field if non-nil, zero value otherwise.

### GetLastTriggeredAtOk

`func (o *AutomationResponse) GetLastTriggeredAtOk() (*time.Time, bool)`

GetLastTriggeredAtOk returns a tuple with the LastTriggeredAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLastTriggeredAt

`func (o *AutomationResponse) SetLastTriggeredAt(v time.Time)`

SetLastTriggeredAt sets LastTriggeredAt field to given value.

### HasLastTriggeredAt

`func (o *AutomationResponse) HasLastTriggeredAt() bool`

HasLastTriggeredAt returns a boolean if a field has been set.

### SetLastTriggeredAtNil

`func (o *AutomationResponse) SetLastTriggeredAtNil(b bool)`

 SetLastTriggeredAtNil sets the value for LastTriggeredAt to be an explicit nil

### UnsetLastTriggeredAt
`func (o *AutomationResponse) UnsetLastTriggeredAt()`

UnsetLastTriggeredAt ensures that no value is present for LastTriggeredAt, not even an explicit nil
### GetCreatedAt

`func (o *AutomationResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *AutomationResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *AutomationResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *AutomationResponse) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *AutomationResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *AutomationResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *AutomationResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *AutomationResponse) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


