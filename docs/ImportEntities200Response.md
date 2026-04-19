# ImportEntities200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Total** | Pointer to **int32** | Total rows processed | [optional] 
**Created** | Pointer to **int32** | Number of entities created | [optional] 
**Updated** | Pointer to **int32** | Number of entities updated | [optional] 
**Skipped** | Pointer to **int32** | Number of rows skipped (no changes) | [optional] 
**Failed** | Pointer to **int32** | Number of rows that failed | [optional] 
**Errors** | Pointer to [**[]ImportEntities200ResponseErrorsInner**](ImportEntities200ResponseErrorsInner.md) |  | [optional] 

## Methods

### NewImportEntities200Response

`func NewImportEntities200Response() *ImportEntities200Response`

NewImportEntities200Response instantiates a new ImportEntities200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewImportEntities200ResponseWithDefaults

`func NewImportEntities200ResponseWithDefaults() *ImportEntities200Response`

NewImportEntities200ResponseWithDefaults instantiates a new ImportEntities200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTotal

`func (o *ImportEntities200Response) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ImportEntities200Response) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ImportEntities200Response) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *ImportEntities200Response) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetCreated

`func (o *ImportEntities200Response) GetCreated() int32`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *ImportEntities200Response) GetCreatedOk() (*int32, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *ImportEntities200Response) SetCreated(v int32)`

SetCreated sets Created field to given value.

### HasCreated

`func (o *ImportEntities200Response) HasCreated() bool`

HasCreated returns a boolean if a field has been set.

### GetUpdated

`func (o *ImportEntities200Response) GetUpdated() int32`

GetUpdated returns the Updated field if non-nil, zero value otherwise.

### GetUpdatedOk

`func (o *ImportEntities200Response) GetUpdatedOk() (*int32, bool)`

GetUpdatedOk returns a tuple with the Updated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdated

`func (o *ImportEntities200Response) SetUpdated(v int32)`

SetUpdated sets Updated field to given value.

### HasUpdated

`func (o *ImportEntities200Response) HasUpdated() bool`

HasUpdated returns a boolean if a field has been set.

### GetSkipped

`func (o *ImportEntities200Response) GetSkipped() int32`

GetSkipped returns the Skipped field if non-nil, zero value otherwise.

### GetSkippedOk

`func (o *ImportEntities200Response) GetSkippedOk() (*int32, bool)`

GetSkippedOk returns a tuple with the Skipped field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSkipped

`func (o *ImportEntities200Response) SetSkipped(v int32)`

SetSkipped sets Skipped field to given value.

### HasSkipped

`func (o *ImportEntities200Response) HasSkipped() bool`

HasSkipped returns a boolean if a field has been set.

### GetFailed

`func (o *ImportEntities200Response) GetFailed() int32`

GetFailed returns the Failed field if non-nil, zero value otherwise.

### GetFailedOk

`func (o *ImportEntities200Response) GetFailedOk() (*int32, bool)`

GetFailedOk returns a tuple with the Failed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFailed

`func (o *ImportEntities200Response) SetFailed(v int32)`

SetFailed sets Failed field to given value.

### HasFailed

`func (o *ImportEntities200Response) HasFailed() bool`

HasFailed returns a boolean if a field has been set.

### GetErrors

`func (o *ImportEntities200Response) GetErrors() []ImportEntities200ResponseErrorsInner`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *ImportEntities200Response) GetErrorsOk() (*[]ImportEntities200ResponseErrorsInner, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *ImportEntities200Response) SetErrors(v []ImportEntities200ResponseErrorsInner)`

SetErrors sets Errors field to given value.

### HasErrors

`func (o *ImportEntities200Response) HasErrors() bool`

HasErrors returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


