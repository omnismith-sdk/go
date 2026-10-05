# AutomationTimerResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Timer UUID. There is at most one pending timer per automation, record and kind, so re-arming keeps the id. | 
**AutomationId** | **string** | Automation the timer belongs to | 
**AutomationName** | **string** | Name of that automation | 
**EntityId** | **NullableString** | Record the timer is about; null for a timer that belongs to no record (a schedule without a template) | 
**Kind** | **string** | What the timer is for: the next slot of a schedule, a date attribute reaching its moment, or a \&quot;no change within\&quot; deadline | 
**DueAt** | **time.Time** | When the timer fires (UTC). It fires within about 30 seconds of this moment; one that came due while the service was down fires once, late. | 

## Methods

### NewAutomationTimerResponse

`func NewAutomationTimerResponse(id string, automationId string, automationName string, entityId NullableString, kind string, dueAt time.Time, ) *AutomationTimerResponse`

NewAutomationTimerResponse instantiates a new AutomationTimerResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAutomationTimerResponseWithDefaults

`func NewAutomationTimerResponseWithDefaults() *AutomationTimerResponse`

NewAutomationTimerResponseWithDefaults instantiates a new AutomationTimerResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *AutomationTimerResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AutomationTimerResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AutomationTimerResponse) SetId(v string)`

SetId sets Id field to given value.


### GetAutomationId

`func (o *AutomationTimerResponse) GetAutomationId() string`

GetAutomationId returns the AutomationId field if non-nil, zero value otherwise.

### GetAutomationIdOk

`func (o *AutomationTimerResponse) GetAutomationIdOk() (*string, bool)`

GetAutomationIdOk returns a tuple with the AutomationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutomationId

`func (o *AutomationTimerResponse) SetAutomationId(v string)`

SetAutomationId sets AutomationId field to given value.


### GetAutomationName

`func (o *AutomationTimerResponse) GetAutomationName() string`

GetAutomationName returns the AutomationName field if non-nil, zero value otherwise.

### GetAutomationNameOk

`func (o *AutomationTimerResponse) GetAutomationNameOk() (*string, bool)`

GetAutomationNameOk returns a tuple with the AutomationName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutomationName

`func (o *AutomationTimerResponse) SetAutomationName(v string)`

SetAutomationName sets AutomationName field to given value.


### GetEntityId

`func (o *AutomationTimerResponse) GetEntityId() string`

GetEntityId returns the EntityId field if non-nil, zero value otherwise.

### GetEntityIdOk

`func (o *AutomationTimerResponse) GetEntityIdOk() (*string, bool)`

GetEntityIdOk returns a tuple with the EntityId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityId

`func (o *AutomationTimerResponse) SetEntityId(v string)`

SetEntityId sets EntityId field to given value.


### SetEntityIdNil

`func (o *AutomationTimerResponse) SetEntityIdNil(b bool)`

 SetEntityIdNil sets the value for EntityId to be an explicit nil

### UnsetEntityId
`func (o *AutomationTimerResponse) UnsetEntityId()`

UnsetEntityId ensures that no value is present for EntityId, not even an explicit nil
### GetKind

`func (o *AutomationTimerResponse) GetKind() string`

GetKind returns the Kind field if non-nil, zero value otherwise.

### GetKindOk

`func (o *AutomationTimerResponse) GetKindOk() (*string, bool)`

GetKindOk returns a tuple with the Kind field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKind

`func (o *AutomationTimerResponse) SetKind(v string)`

SetKind sets Kind field to given value.


### GetDueAt

`func (o *AutomationTimerResponse) GetDueAt() time.Time`

GetDueAt returns the DueAt field if non-nil, zero value otherwise.

### GetDueAtOk

`func (o *AutomationTimerResponse) GetDueAtOk() (*time.Time, bool)`

GetDueAtOk returns a tuple with the DueAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDueAt

`func (o *AutomationTimerResponse) SetDueAt(v time.Time)`

SetDueAt sets DueAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


