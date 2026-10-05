# UpsertEntityByKeyResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Identifier of the record that holds the key | 
**Created** | **bool** | True when the record was created by this call, false when an existing record was updated | 

## Methods

### NewUpsertEntityByKeyResponse

`func NewUpsertEntityByKeyResponse(id string, created bool, ) *UpsertEntityByKeyResponse`

NewUpsertEntityByKeyResponse instantiates a new UpsertEntityByKeyResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpsertEntityByKeyResponseWithDefaults

`func NewUpsertEntityByKeyResponseWithDefaults() *UpsertEntityByKeyResponse`

NewUpsertEntityByKeyResponseWithDefaults instantiates a new UpsertEntityByKeyResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *UpsertEntityByKeyResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *UpsertEntityByKeyResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *UpsertEntityByKeyResponse) SetId(v string)`

SetId sets Id field to given value.


### GetCreated

`func (o *UpsertEntityByKeyResponse) GetCreated() bool`

GetCreated returns the Created field if non-nil, zero value otherwise.

### GetCreatedOk

`func (o *UpsertEntityByKeyResponse) GetCreatedOk() (*bool, bool)`

GetCreatedOk returns a tuple with the Created field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreated

`func (o *UpsertEntityByKeyResponse) SetCreated(v bool)`

SetCreated sets Created field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


