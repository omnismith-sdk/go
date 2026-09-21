# EntityActionOutcome

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EntityId** | **string** | OpenAPI schema for the outcome of the action on one record of a batch. | 
**Status** | **string** | &#x60;executed&#x60; — written as the receipt says. &#x60;precondition_failed&#x60; — the record was not in the state the action needs (&#x60;error.reason&#x60; says why). &#x60;rule_violated&#x60; — a template rule refused the write (&#x60;error.errors&#x60; keyed by &#x60;attributes.&lt;slug&gt;&#x60;). &#x60;failed&#x60; — any other refusal: unknown record, no permission, a value failing its type. | 
**Receipt** | [**NullableExecuteEntityActionResponse**](ExecuteEntityActionResponse.md) |  | 
**Error** | [**NullableErrorResponse**](ErrorResponse.md) |  | 

## Methods

### NewEntityActionOutcome

`func NewEntityActionOutcome(entityId string, status string, receipt NullableExecuteEntityActionResponse, error_ NullableErrorResponse, ) *EntityActionOutcome`

NewEntityActionOutcome instantiates a new EntityActionOutcome object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityActionOutcomeWithDefaults

`func NewEntityActionOutcomeWithDefaults() *EntityActionOutcome`

NewEntityActionOutcomeWithDefaults instantiates a new EntityActionOutcome object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEntityId

`func (o *EntityActionOutcome) GetEntityId() string`

GetEntityId returns the EntityId field if non-nil, zero value otherwise.

### GetEntityIdOk

`func (o *EntityActionOutcome) GetEntityIdOk() (*string, bool)`

GetEntityIdOk returns a tuple with the EntityId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityId

`func (o *EntityActionOutcome) SetEntityId(v string)`

SetEntityId sets EntityId field to given value.


### GetStatus

`func (o *EntityActionOutcome) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *EntityActionOutcome) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *EntityActionOutcome) SetStatus(v string)`

SetStatus sets Status field to given value.


### GetReceipt

`func (o *EntityActionOutcome) GetReceipt() ExecuteEntityActionResponse`

GetReceipt returns the Receipt field if non-nil, zero value otherwise.

### GetReceiptOk

`func (o *EntityActionOutcome) GetReceiptOk() (*ExecuteEntityActionResponse, bool)`

GetReceiptOk returns a tuple with the Receipt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReceipt

`func (o *EntityActionOutcome) SetReceipt(v ExecuteEntityActionResponse)`

SetReceipt sets Receipt field to given value.


### SetReceiptNil

`func (o *EntityActionOutcome) SetReceiptNil(b bool)`

 SetReceiptNil sets the value for Receipt to be an explicit nil

### UnsetReceipt
`func (o *EntityActionOutcome) UnsetReceipt()`

UnsetReceipt ensures that no value is present for Receipt, not even an explicit nil
### GetError

`func (o *EntityActionOutcome) GetError() ErrorResponse`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *EntityActionOutcome) GetErrorOk() (*ErrorResponse, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *EntityActionOutcome) SetError(v ErrorResponse)`

SetError sets Error field to given value.


### SetErrorNil

`func (o *EntityActionOutcome) SetErrorNil(b bool)`

 SetErrorNil sets the value for Error to be an explicit nil

### UnsetError
`func (o *EntityActionOutcome) UnsetError()`

UnsetError ensures that no value is present for Error, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


