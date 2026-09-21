# BatchWriteEntitiesResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Atomic** | Pointer to **bool** | Whether the batch ran as a single transaction. | [optional] 
**Total** | Pointer to **int32** | Number of operations submitted. | [optional] 
**Created** | Pointer to **int32** | Number of entities created. | [optional] 
**Updated** | Pointer to **int32** | Number of entities updated. | [optional] 
**Replaced** | Pointer to **int32** | Number of entities replaced. | [optional] 
**Deleted** | Pointer to **int32** | Number of entities soft-deleted. | [optional] 
**Failed** | Pointer to **int32** | Number of operations that failed. Non-zero means the batch partially applied. | [optional] 
**Results** | Pointer to [**[]BatchOperationResult**](BatchOperationResult.md) | One entry per submitted operation, in the submitted order. | [optional] 

## Methods

### NewBatchWriteEntitiesResponse

`func NewBatchWriteEntitiesResponse() *BatchWriteEntitiesResponse`

NewBatchWriteEntitiesResponse instantiates a new BatchWriteEntitiesResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBatchWriteEntitiesResponseWithDefaults

`func NewBatchWriteEntitiesResponseWithDefaults() *BatchWriteEntitiesResponse`

NewBatchWriteEntitiesResponseWithDefaults instantiates a new BatchWriteEntitiesResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAtomic

`func (o *BatchWriteEntitiesResponse) GetAtomic() bool`

GetAtomic returns the Atomic field if non-nil, zero value otherwise.

### GetAtomicOk

`func (o *BatchWriteEntitiesResponse) GetAtomicOk() (*bool, bool)`

GetAtomicOk returns a tuple with the Atomic field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAtomic

`func (o *BatchWriteEntitiesResponse) SetAtomic(v bool)`

SetAtomic sets Atomic field to given value.

### HasAtomic

`func (o *BatchWriteEntitiesResponse) HasAtomic() bool`

HasAtomic returns a boolean if a field has been set.

### GetTotal

`func (o *BatchWriteEntitiesResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *BatchWriteEntitiesResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *BatchWriteEntitiesResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *BatchWriteEntitiesResponse) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetCreated

`func (o *BatchWriteEntitiesResponse) GetCreated() int32`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *BatchWriteEntitiesResponse) GetCreatedOk() (*int32, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *BatchWriteEntitiesResponse) SetCreated(v int32)`

SetCreated sets Created field to given value.

### HasCreated

`func (o *BatchWriteEntitiesResponse) HasCreated() bool`

HasCreated returns a boolean if a field has been set.

### GetUpdated

`func (o *BatchWriteEntitiesResponse) GetUpdated() int32`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *BatchWriteEntitiesResponse) GetUpdatedOk() (*int32, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *BatchWriteEntitiesResponse) SetUpdated(v int32)`

SetUpdated sets Updated field to given value.

### HasUpdated

`func (o *BatchWriteEntitiesResponse) HasUpdated() bool`

HasUpdated returns a boolean if a field has been set.

### GetReplaced

`func (o *BatchWriteEntitiesResponse) GetReplaced() int32`

GetReplaced returns the Replaced field if non-nil, zero value otherwise.

### GetReplacedOk

`func (o *BatchWriteEntitiesResponse) GetReplacedOk() (*int32, bool)`

GetReplacedOk returns a tuple with the Replaced field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplaced

`func (o *BatchWriteEntitiesResponse) SetReplaced(v int32)`

SetReplaced sets Replaced field to given value.

### HasReplaced

`func (o *BatchWriteEntitiesResponse) HasReplaced() bool`

HasReplaced returns a boolean if a field has been set.

### GetDeleted

`func (o *BatchWriteEntitiesResponse) GetDeleted() int32`

GetDeleted returns the Deleted field if non-nil, zero value otherwise.

### GetDeletedOk

`func (o *BatchWriteEntitiesResponse) GetDeletedOk() (*int32, bool)`

GetDeletedOk returns a tuple with the Deleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeleted

`func (o *BatchWriteEntitiesResponse) SetDeleted(v int32)`

SetDeleted sets Deleted field to given value.

### HasDeleted

`func (o *BatchWriteEntitiesResponse) HasDeleted() bool`

HasDeleted returns a boolean if a field has been set.

### GetFailed

`func (o *BatchWriteEntitiesResponse) GetFailed() int32`

GetFailed returns the Failed field if non-nil, zero value otherwise.

### GetFailedOk

`func (o *BatchWriteEntitiesResponse) GetFailedOk() (*int32, bool)`

GetFailedOk returns a tuple with the Failed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailed

`func (o *BatchWriteEntitiesResponse) SetFailed(v int32)`

SetFailed sets Failed field to given value.

### HasFailed

`func (o *BatchWriteEntitiesResponse) HasFailed() bool`

HasFailed returns a boolean if a field has been set.

### GetResults

`func (o *BatchWriteEntitiesResponse) GetResults() []BatchOperationResult`

GetResults returns the Results field if non-nil, zero value otherwise.

### GetResultsOk

`func (o *BatchWriteEntitiesResponse) GetResultsOk() (*[]BatchOperationResult, bool)`

GetResultsOk returns a tuple with the Results field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResults

`func (o *BatchWriteEntitiesResponse) SetResults(v []BatchOperationResult)`

SetResults sets Results field to given value.

### HasResults

`func (o *BatchWriteEntitiesResponse) HasResults() bool`

HasResults returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


