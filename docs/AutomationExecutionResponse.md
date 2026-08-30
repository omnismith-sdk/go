# AutomationExecutionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Unique execution record UUID | [optional] 
**AutomationId** | Pointer to **string** | Associated automation rule UUID | [optional] 
**EntityId** | Pointer to **string** | UUID of the entity that triggered the execution | [optional] 
**TriggeredAt** | Pointer to **time.Time** | Timestamp when the trigger event was evaluated | [optional] 
**CompletedAt** | Pointer to **NullableTime** | Timestamp when all actions completed execution | [optional] 
**Status** | Pointer to **string** | Overall execution outcome status | [optional] 
**ActionResults** | Pointer to [**[]AutomationExecutionResponseActionResultsInner**](AutomationExecutionResponseActionResultsInner.md) | Individual action execution outcomes | [optional] 
**ErrorMessage** | Pointer to **NullableString** | Top-level error message if execution failed | [optional] 

## Methods

### NewAutomationExecutionResponse

`func NewAutomationExecutionResponse() *AutomationExecutionResponse`

NewAutomationExecutionResponse instantiates a new AutomationExecutionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAutomationExecutionResponseWithDefaults

`func NewAutomationExecutionResponseWithDefaults() *AutomationExecutionResponse`

NewAutomationExecutionResponseWithDefaults instantiates a new AutomationExecutionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *AutomationExecutionResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AutomationExecutionResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AutomationExecutionResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *AutomationExecutionResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetAutomationId

`func (o *AutomationExecutionResponse) GetAutomationId() string`

GetAutomationId returns the AutomationId field if non-nil, zero value otherwise.

### GetAutomationIdOk

`func (o *AutomationExecutionResponse) GetAutomationIdOk() (*string, bool)`

GetAutomationIdOk returns a tuple with the AutomationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutomationId

`func (o *AutomationExecutionResponse) SetAutomationId(v string)`

SetAutomationId sets AutomationId field to given value.

### HasAutomationId

`func (o *AutomationExecutionResponse) HasAutomationId() bool`

HasAutomationId returns a boolean if a field has been set.

### GetEntityId

`func (o *AutomationExecutionResponse) GetEntityId() string`

GetEntityId returns the EntityId field if non-nil, zero value otherwise.

### GetEntityIdOk

`func (o *AutomationExecutionResponse) GetEntityIdOk() (*string, bool)`

GetEntityIdOk returns a tuple with the EntityId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityId

`func (o *AutomationExecutionResponse) SetEntityId(v string)`

SetEntityId sets EntityId field to given value.

### HasEntityId

`func (o *AutomationExecutionResponse) HasEntityId() bool`

HasEntityId returns a boolean if a field has been set.

### GetTriggeredAt

`func (o *AutomationExecutionResponse) GetTriggeredAt() time.Time`

GetTriggeredAt returns the TriggeredAt field if non-nil, zero value otherwise.

### GetTriggeredAtOk

`func (o *AutomationExecutionResponse) GetTriggeredAtOk() (*time.Time, bool)`

GetTriggeredAtOk returns a tuple with the TriggeredAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTriggeredAt

`func (o *AutomationExecutionResponse) SetTriggeredAt(v time.Time)`

SetTriggeredAt sets TriggeredAt field to given value.

### HasTriggeredAt

`func (o *AutomationExecutionResponse) HasTriggeredAt() bool`

HasTriggeredAt returns a boolean if a field has been set.

### GetCompletedAt

`func (o *AutomationExecutionResponse) GetCompletedAt() time.Time`

GetCompletedAt returns the CompletedAt field if non-nil, zero value otherwise.

### GetCompletedAtOk

`func (o *AutomationExecutionResponse) GetCompletedAtOk() (*time.Time, bool)`

GetCompletedAtOk returns a tuple with the CompletedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompletedAt

`func (o *AutomationExecutionResponse) SetCompletedAt(v time.Time)`

SetCompletedAt sets CompletedAt field to given value.

### HasCompletedAt

`func (o *AutomationExecutionResponse) HasCompletedAt() bool`

HasCompletedAt returns a boolean if a field has been set.

### SetCompletedAtNil

`func (o *AutomationExecutionResponse) SetCompletedAtNil(b bool)`

 SetCompletedAtNil sets the value for CompletedAt to be an explicit nil

### UnsetCompletedAt
`func (o *AutomationExecutionResponse) UnsetCompletedAt()`

UnsetCompletedAt ensures that no value is present for CompletedAt, not even an explicit nil
### GetStatus

`func (o *AutomationExecutionResponse) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *AutomationExecutionResponse) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *AutomationExecutionResponse) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *AutomationExecutionResponse) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetActionResults

`func (o *AutomationExecutionResponse) GetActionResults() []AutomationExecutionResponseActionResultsInner`

GetActionResults returns the ActionResults field if non-nil, zero value otherwise.

### GetActionResultsOk

`func (o *AutomationExecutionResponse) GetActionResultsOk() (*[]AutomationExecutionResponseActionResultsInner, bool)`

GetActionResultsOk returns a tuple with the ActionResults field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionResults

`func (o *AutomationExecutionResponse) SetActionResults(v []AutomationExecutionResponseActionResultsInner)`

SetActionResults sets ActionResults field to given value.

### HasActionResults

`func (o *AutomationExecutionResponse) HasActionResults() bool`

HasActionResults returns a boolean if a field has been set.

### GetErrorMessage

`func (o *AutomationExecutionResponse) GetErrorMessage() string`

GetErrorMessage returns the ErrorMessage field if non-nil, zero value otherwise.

### GetErrorMessageOk

`func (o *AutomationExecutionResponse) GetErrorMessageOk() (*string, bool)`

GetErrorMessageOk returns a tuple with the ErrorMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorMessage

`func (o *AutomationExecutionResponse) SetErrorMessage(v string)`

SetErrorMessage sets ErrorMessage field to given value.

### HasErrorMessage

`func (o *AutomationExecutionResponse) HasErrorMessage() bool`

HasErrorMessage returns a boolean if a field has been set.

### SetErrorMessageNil

`func (o *AutomationExecutionResponse) SetErrorMessageNil(b bool)`

 SetErrorMessageNil sets the value for ErrorMessage to be an explicit nil

### UnsetErrorMessage
`func (o *AutomationExecutionResponse) UnsetErrorMessage()`

UnsetErrorMessage ensures that no value is present for ErrorMessage, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


