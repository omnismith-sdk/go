# BatchWriteEntitiesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Operations** | [**[]BatchOperationInput**](BatchOperationInput.md) | Operations applied in the order given, at most 100 per call. | 
**Atomic** | Pointer to **bool** | When false (the default) every operation is attempted and failures are reported per index. When true the batch runs in a single transaction and the first failure rolls all of it back. Atomic batches reject metric values, which are published outside the transaction and cannot be rolled back. | [optional] [default to false]

## Methods

### NewBatchWriteEntitiesRequest

`func NewBatchWriteEntitiesRequest(operations []BatchOperationInput, ) *BatchWriteEntitiesRequest`

NewBatchWriteEntitiesRequest instantiates a new BatchWriteEntitiesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBatchWriteEntitiesRequestWithDefaults

`func NewBatchWriteEntitiesRequestWithDefaults() *BatchWriteEntitiesRequest`

NewBatchWriteEntitiesRequestWithDefaults instantiates a new BatchWriteEntitiesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOperations

`func (o *BatchWriteEntitiesRequest) GetOperations() []BatchOperationInput`

GetOperations returns the Operations field if non-nil, zero value otherwise.

### GetOperationsOk

`func (o *BatchWriteEntitiesRequest) GetOperationsOk() (*[]BatchOperationInput, bool)`

GetOperationsOk returns a tuple with the Operations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperations

`func (o *BatchWriteEntitiesRequest) SetOperations(v []BatchOperationInput)`

SetOperations sets Operations field to given value.


### GetAtomic

`func (o *BatchWriteEntitiesRequest) GetAtomic() bool`

GetAtomic returns the Atomic field if non-nil, zero value otherwise.

### GetAtomicOk

`func (o *BatchWriteEntitiesRequest) GetAtomicOk() (*bool, bool)`

GetAtomicOk returns a tuple with the Atomic field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAtomic

`func (o *BatchWriteEntitiesRequest) SetAtomic(v bool)`

SetAtomic sets Atomic field to given value.

### HasAtomic

`func (o *BatchWriteEntitiesRequest) HasAtomic() bool`

HasAtomic returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


