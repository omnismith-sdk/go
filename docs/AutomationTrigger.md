# AutomationTrigger

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** | What fires the automation: a record event (&#x60;on_entity_created&#x60;, &#x60;on_entity_updated&#x60;, &#x60;on_attribute_changed&#x60;, &#x60;on_action_executed&#x60;) or the clock (&#x60;schedule&#x60;, &#x60;date_reached&#x60;, &#x60;no_change_within&#x60;). | 
**TemplateId** | Pointer to **NullableString** | Template id the trigger watches. Required for &#x60;date_reached&#x60; and &#x60;no_change_within&#x60;; optional for record events (none &#x3D; every template) and for &#x60;schedule&#x60; (none &#x3D; one run without a record). | [optional] 
**AttributeId** | Pointer to **NullableString** | Attribute id of the template; required for &#x60;on_attribute_changed&#x60;, &#x60;date_reached&#x60; (a date or datetime attribute) and &#x60;no_change_within&#x60; (the watched attribute; not a metric), absent otherwise. | [optional] 
**ActionId** | Pointer to **NullableString** | Entity action id; required for &#x60;on_action_executed&#x60;, absent otherwise. | [optional] 
**Cron** | Pointer to **NullableString** | &#x60;schedule&#x60; only: a 5-field cron expression (minute hour day-of-month month day-of-week), read in &#x60;timezone&#x60;. Runs at least 5 minutes apart. | [optional] 
**Timezone** | Pointer to **NullableString** | Time-based triggers only: the IANA timezone their times are read in, e.g. &#x60;Europe/Berlin&#x60;. | [optional] 
**DelayMinutes** | Pointer to **NullableInt32** | &#x60;no_change_within&#x60; only: how long the watched attribute must stay unchanged, 5 to 129600 minutes (90 days). Also accepted as &#x60;delay_minutes&#x60;. | [optional] 
**OffsetMinutes** | Pointer to **NullableInt32** | &#x60;date_reached&#x60; only: signed whole minutes from the date, negative for before it; at most 527040 (366 days) either way. Also accepted as &#x60;offset_minutes&#x60;. | [optional] 

## Methods

### NewAutomationTrigger

`func NewAutomationTrigger(type_ string, ) *AutomationTrigger`

NewAutomationTrigger instantiates a new AutomationTrigger object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAutomationTriggerWithDefaults

`func NewAutomationTriggerWithDefaults() *AutomationTrigger`

NewAutomationTriggerWithDefaults instantiates a new AutomationTrigger object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *AutomationTrigger) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *AutomationTrigger) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *AutomationTrigger) SetType(v string)`

SetType sets Type field to given value.


### GetTemplateId

`func (o *AutomationTrigger) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *AutomationTrigger) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *AutomationTrigger) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *AutomationTrigger) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### SetTemplateIdNil

`func (o *AutomationTrigger) SetTemplateIdNil(b bool)`

 SetTemplateIdNil sets the value for TemplateId to be an explicit nil

### UnsetTemplateId
`func (o *AutomationTrigger) UnsetTemplateId()`

UnsetTemplateId ensures that no value is present for TemplateId, not even an explicit nil
### GetAttributeId

`func (o *AutomationTrigger) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *AutomationTrigger) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *AutomationTrigger) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.

### HasAttributeId

`func (o *AutomationTrigger) HasAttributeId() bool`

HasAttributeId returns a boolean if a field has been set.

### SetAttributeIdNil

`func (o *AutomationTrigger) SetAttributeIdNil(b bool)`

 SetAttributeIdNil sets the value for AttributeId to be an explicit nil

### UnsetAttributeId
`func (o *AutomationTrigger) UnsetAttributeId()`

UnsetAttributeId ensures that no value is present for AttributeId, not even an explicit nil
### GetActionId

`func (o *AutomationTrigger) GetActionId() string`

GetActionId returns the ActionId field if non-nil, zero value otherwise.

### GetActionIdOk

`func (o *AutomationTrigger) GetActionIdOk() (*string, bool)`

GetActionIdOk returns a tuple with the ActionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionId

`func (o *AutomationTrigger) SetActionId(v string)`

SetActionId sets ActionId field to given value.

### HasActionId

`func (o *AutomationTrigger) HasActionId() bool`

HasActionId returns a boolean if a field has been set.

### SetActionIdNil

`func (o *AutomationTrigger) SetActionIdNil(b bool)`

 SetActionIdNil sets the value for ActionId to be an explicit nil

### UnsetActionId
`func (o *AutomationTrigger) UnsetActionId()`

UnsetActionId ensures that no value is present for ActionId, not even an explicit nil
### GetCron

`func (o *AutomationTrigger) GetCron() string`

GetCron returns the Cron field if non-nil, zero value otherwise.

### GetCronOk

`func (o *AutomationTrigger) GetCronOk() (*string, bool)`

GetCronOk returns a tuple with the Cron field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCron

`func (o *AutomationTrigger) SetCron(v string)`

SetCron sets Cron field to given value.

### HasCron

`func (o *AutomationTrigger) HasCron() bool`

HasCron returns a boolean if a field has been set.

### SetCronNil

`func (o *AutomationTrigger) SetCronNil(b bool)`

 SetCronNil sets the value for Cron to be an explicit nil

### UnsetCron
`func (o *AutomationTrigger) UnsetCron()`

UnsetCron ensures that no value is present for Cron, not even an explicit nil
### GetTimezone

`func (o *AutomationTrigger) GetTimezone() string`

GetTimezone returns the Timezone field if non-nil, zero value otherwise.

### GetTimezoneOk

`func (o *AutomationTrigger) GetTimezoneOk() (*string, bool)`

GetTimezoneOk returns a tuple with the Timezone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimezone

`func (o *AutomationTrigger) SetTimezone(v string)`

SetTimezone sets Timezone field to given value.

### HasTimezone

`func (o *AutomationTrigger) HasTimezone() bool`

HasTimezone returns a boolean if a field has been set.

### SetTimezoneNil

`func (o *AutomationTrigger) SetTimezoneNil(b bool)`

 SetTimezoneNil sets the value for Timezone to be an explicit nil

### UnsetTimezone
`func (o *AutomationTrigger) UnsetTimezone()`

UnsetTimezone ensures that no value is present for Timezone, not even an explicit nil
### GetDelayMinutes

`func (o *AutomationTrigger) GetDelayMinutes() int32`

GetDelayMinutes returns the DelayMinutes field if non-nil, zero value otherwise.

### GetDelayMinutesOk

`func (o *AutomationTrigger) GetDelayMinutesOk() (*int32, bool)`

GetDelayMinutesOk returns a tuple with the DelayMinutes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDelayMinutes

`func (o *AutomationTrigger) SetDelayMinutes(v int32)`

SetDelayMinutes sets DelayMinutes field to given value.

### HasDelayMinutes

`func (o *AutomationTrigger) HasDelayMinutes() bool`

HasDelayMinutes returns a boolean if a field has been set.

### SetDelayMinutesNil

`func (o *AutomationTrigger) SetDelayMinutesNil(b bool)`

 SetDelayMinutesNil sets the value for DelayMinutes to be an explicit nil

### UnsetDelayMinutes
`func (o *AutomationTrigger) UnsetDelayMinutes()`

UnsetDelayMinutes ensures that no value is present for DelayMinutes, not even an explicit nil
### GetOffsetMinutes

`func (o *AutomationTrigger) GetOffsetMinutes() int32`

GetOffsetMinutes returns the OffsetMinutes field if non-nil, zero value otherwise.

### GetOffsetMinutesOk

`func (o *AutomationTrigger) GetOffsetMinutesOk() (*int32, bool)`

GetOffsetMinutesOk returns a tuple with the OffsetMinutes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOffsetMinutes

`func (o *AutomationTrigger) SetOffsetMinutes(v int32)`

SetOffsetMinutes sets OffsetMinutes field to given value.

### HasOffsetMinutes

`func (o *AutomationTrigger) HasOffsetMinutes() bool`

HasOffsetMinutes returns a boolean if a field has been set.

### SetOffsetMinutesNil

`func (o *AutomationTrigger) SetOffsetMinutesNil(b bool)`

 SetOffsetMinutesNil sets the value for OffsetMinutes to be an explicit nil

### UnsetOffsetMinutes
`func (o *AutomationTrigger) UnsetOffsetMinutes()`

UnsetOffsetMinutes ensures that no value is present for OffsetMinutes, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


