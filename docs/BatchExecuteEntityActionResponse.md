# BatchExecuteEntityActionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Atomic** | **bool** | Whether the batch ran as a single transaction. | 
**Total** | **int32** | Number of records submitted. | 
**Executed** | **int32** | Records the action ran on. | 
**PreconditionFailed** | **int32** | Records skipped because the precondition did not hold. | 
**RuleViolated** | **int32** | Records refused by a template rule. | 
**Failed** | **int32** | Records refused for any other reason. | 
**Results** | [**[]EntityActionOutcome**](EntityActionOutcome.md) |  | 

## Methods

### NewBatchExecuteEntityActionResponse

`func NewBatchExecuteEntityActionResponse(atomic bool, total int32, executed int32, preconditionFailed int32, ruleViolated int32, failed int32, results []EntityActionOutcome, ) *BatchExecuteEntityActionResponse`

NewBatchExecuteEntityActionResponse instantiates a new BatchExecuteEntityActionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBatchExecuteEntityActionResponseWithDefaults

`func NewBatchExecuteEntityActionResponseWithDefaults() *BatchExecuteEntityActionResponse`

NewBatchExecuteEntityActionResponseWithDefaults instantiates a new BatchExecuteEntityActionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAtomic

`func (o *BatchExecuteEntityActionResponse) GetAtomic() bool`

GetAtomic returns the Atomic field if non-nil, zero value otherwise.

### GetAtomicOk

`func (o *BatchExecuteEntityActionResponse) GetAtomicOk() (*bool, bool)`

GetAtomicOk returns a tuple with the Atomic field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAtomic

`func (o *BatchExecuteEntityActionResponse) SetAtomic(v bool)`

SetAtomic sets Atomic field to given value.


### GetTotal

`func (o *BatchExecuteEntityActionResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *BatchExecuteEntityActionResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *BatchExecuteEntityActionResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.


### GetExecuted

`func (o *BatchExecuteEntityActionResponse) GetExecuted() int32`

GetExecuted returns the Executed field if non-nil, zero value otherwise.

### GetExecutedOk

`func (o *BatchExecuteEntityActionResponse) GetExecutedOk() (*int32, bool)`

GetExecutedOk returns a tuple with the Executed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecuted

`func (o *BatchExecuteEntityActionResponse) SetExecuted(v int32)`

SetExecuted sets Executed field to given value.


### GetPreconditionFailed

`func (o *BatchExecuteEntityActionResponse) GetPreconditionFailed() int32`

GetPreconditionFailed returns the PreconditionFailed field if non-nil, zero value otherwise.

### GetPreconditionFailedOk

`func (o *BatchExecuteEntityActionResponse) GetPreconditionFailedOk() (*int32, bool)`

GetPreconditionFailedOk returns a tuple with the PreconditionFailed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreconditionFailed

`func (o *BatchExecuteEntityActionResponse) SetPreconditionFailed(v int32)`

SetPreconditionFailed sets PreconditionFailed field to given value.


### GetRuleViolated

`func (o *BatchExecuteEntityActionResponse) GetRuleViolated() int32`

GetRuleViolated returns the RuleViolated field if non-nil, zero value otherwise.

### GetRuleViolatedOk

`func (o *BatchExecuteEntityActionResponse) GetRuleViolatedOk() (*int32, bool)`

GetRuleViolatedOk returns a tuple with the RuleViolated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRuleViolated

`func (o *BatchExecuteEntityActionResponse) SetRuleViolated(v int32)`

SetRuleViolated sets RuleViolated field to given value.


### GetFailed

`func (o *BatchExecuteEntityActionResponse) GetFailed() int32`

GetFailed returns the Failed field if non-nil, zero value otherwise.

### GetFailedOk

`func (o *BatchExecuteEntityActionResponse) GetFailedOk() (*int32, bool)`

GetFailedOk returns a tuple with the Failed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailed

`func (o *BatchExecuteEntityActionResponse) SetFailed(v int32)`

SetFailed sets Failed field to given value.


### GetResults

`func (o *BatchExecuteEntityActionResponse) GetResults() []EntityActionOutcome`

GetResults returns the Results field if non-nil, zero value otherwise.

### GetResultsOk

`func (o *BatchExecuteEntityActionResponse) GetResultsOk() (*[]EntityActionOutcome, bool)`

GetResultsOk returns a tuple with the Results field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResults

`func (o *BatchExecuteEntityActionResponse) SetResults(v []EntityActionOutcome)`

SetResults sets Results field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


