# BatchOperationResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Index** | Pointer to **int32** | Position of this operation in the submitted array. | [optional] 
**Op** | Pointer to **string** | The operation that was attempted. | [optional] 
**Id** | Pointer to **NullableString** | Entity the operation acted on. For a successful create this is the newly generated identifier. Null when a create failed before an identifier existed. | [optional] 
**Status** | Pointer to **string** | Outcome of this operation. | [optional] 
**Error** | Pointer to [**NullableErrorResponse**](ErrorResponse.md) |  | [optional] 

## Methods

### NewBatchOperationResult

`func NewBatchOperationResult() *BatchOperationResult`

NewBatchOperationResult instantiates a new BatchOperationResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBatchOperationResultWithDefaults

`func NewBatchOperationResultWithDefaults() *BatchOperationResult`

NewBatchOperationResultWithDefaults instantiates a new BatchOperationResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIndex

`func (o *BatchOperationResult) GetIndex() int32`

GetIndex returns the Index field if non-nil, zero value otherwise.

### GetIndexOk

`func (o *BatchOperationResult) GetIndexOk() (*int32, bool)`

GetIndexOk returns a tuple with the Index field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIndex

`func (o *BatchOperationResult) SetIndex(v int32)`

SetIndex sets Index field to given value.

### HasIndex

`func (o *BatchOperationResult) HasIndex() bool`

HasIndex returns a boolean if a field has been set.

### GetOp

`func (o *BatchOperationResult) GetOp() string`

GetOp returns the Op field if non-nil, zero value otherwise.

### GetOpOk

`func (o *BatchOperationResult) GetOpOk() (*string, bool)`

GetOpOk returns a tuple with the Op field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOp

`func (o *BatchOperationResult) SetOp(v string)`

SetOp sets Op field to given value.

### HasOp

`func (o *BatchOperationResult) HasOp() bool`

HasOp returns a boolean if a field has been set.

### GetId

`func (o *BatchOperationResult) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *BatchOperationResult) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *BatchOperationResult) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *BatchOperationResult) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *BatchOperationResult) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *BatchOperationResult) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetStatus

`func (o *BatchOperationResult) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *BatchOperationResult) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *BatchOperationResult) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *BatchOperationResult) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetError

`func (o *BatchOperationResult) GetError() ErrorResponse`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *BatchOperationResult) GetErrorOk() (*ErrorResponse, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *BatchOperationResult) SetError(v ErrorResponse)`

SetError sets Error field to given value.

### HasError

`func (o *BatchOperationResult) HasError() bool`

HasError returns a boolean if a field has been set.

### SetErrorNil

`func (o *BatchOperationResult) SetErrorNil(b bool)`

 SetErrorNil sets the value for Error to be an explicit nil

### UnsetError
`func (o *BatchOperationResult) UnsetError()`

UnsetError ensures that no value is present for Error, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


