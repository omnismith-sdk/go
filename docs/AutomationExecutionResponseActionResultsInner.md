# AutomationExecutionResponseActionResultsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ActionIndex** | Pointer to **int32** |  | [optional] 
**Success** | Pointer to **bool** |  | [optional] 
**ErrorMessage** | Pointer to **NullableString** |  | [optional] 
**ExecutedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewAutomationExecutionResponseActionResultsInner

`func NewAutomationExecutionResponseActionResultsInner() *AutomationExecutionResponseActionResultsInner`

NewAutomationExecutionResponseActionResultsInner instantiates a new AutomationExecutionResponseActionResultsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAutomationExecutionResponseActionResultsInnerWithDefaults

`func NewAutomationExecutionResponseActionResultsInnerWithDefaults() *AutomationExecutionResponseActionResultsInner`

NewAutomationExecutionResponseActionResultsInnerWithDefaults instantiates a new AutomationExecutionResponseActionResultsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetActionIndex

`func (o *AutomationExecutionResponseActionResultsInner) GetActionIndex() int32`

GetActionIndex returns the ActionIndex field if non-nil, zero value otherwise.

### GetActionIndexOk

`func (o *AutomationExecutionResponseActionResultsInner) GetActionIndexOk() (*int32, bool)`

GetActionIndexOk returns a tuple with the ActionIndex field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionIndex

`func (o *AutomationExecutionResponseActionResultsInner) SetActionIndex(v int32)`

SetActionIndex sets ActionIndex field to given value.

### HasActionIndex

`func (o *AutomationExecutionResponseActionResultsInner) HasActionIndex() bool`

HasActionIndex returns a boolean if a field has been set.

### GetSuccess

`func (o *AutomationExecutionResponseActionResultsInner) GetSuccess() bool`

GetSuccess returns the Success field if non-nil, zero value otherwise.

### GetSuccessOk

`func (o *AutomationExecutionResponseActionResultsInner) GetSuccessOk() (*bool, bool)`

GetSuccessOk returns a tuple with the Success field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSuccess

`func (o *AutomationExecutionResponseActionResultsInner) SetSuccess(v bool)`

SetSuccess sets Success field to given value.

### HasSuccess

`func (o *AutomationExecutionResponseActionResultsInner) HasSuccess() bool`

HasSuccess returns a boolean if a field has been set.

### GetErrorMessage

`func (o *AutomationExecutionResponseActionResultsInner) GetErrorMessage() string`

GetErrorMessage returns the ErrorMessage field if non-nil, zero value otherwise.

### GetErrorMessageOk

`func (o *AutomationExecutionResponseActionResultsInner) GetErrorMessageOk() (*string, bool)`

GetErrorMessageOk returns a tuple with the ErrorMessage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrorMessage

`func (o *AutomationExecutionResponseActionResultsInner) SetErrorMessage(v string)`

SetErrorMessage sets ErrorMessage field to given value.

### HasErrorMessage

`func (o *AutomationExecutionResponseActionResultsInner) HasErrorMessage() bool`

HasErrorMessage returns a boolean if a field has been set.

### SetErrorMessageNil

`func (o *AutomationExecutionResponseActionResultsInner) SetErrorMessageNil(b bool)`

 SetErrorMessageNil sets the value for ErrorMessage to be an explicit nil

### UnsetErrorMessage
`func (o *AutomationExecutionResponseActionResultsInner) UnsetErrorMessage()`

UnsetErrorMessage ensures that no value is present for ErrorMessage, not even an explicit nil
### GetExecutedAt

`func (o *AutomationExecutionResponseActionResultsInner) GetExecutedAt() time.Time`

GetExecutedAt returns the ExecutedAt field if non-nil, zero value otherwise.

### GetExecutedAtOk

`func (o *AutomationExecutionResponseActionResultsInner) GetExecutedAtOk() (*time.Time, bool)`

GetExecutedAtOk returns a tuple with the ExecutedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecutedAt

`func (o *AutomationExecutionResponseActionResultsInner) SetExecutedAt(v time.Time)`

SetExecutedAt sets ExecutedAt field to given value.

### HasExecutedAt

`func (o *AutomationExecutionResponseActionResultsInner) HasExecutedAt() bool`

HasExecutedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


