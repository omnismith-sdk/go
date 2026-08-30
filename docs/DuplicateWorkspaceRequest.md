# DuplicateWorkspaceRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**NewName** | Pointer to **NullableString** | Custom name for the duplicated workspace; if omitted, defaults to the source name with a (Copy) suffix | [optional] 

## Methods

### NewDuplicateWorkspaceRequest

`func NewDuplicateWorkspaceRequest() *DuplicateWorkspaceRequest`

NewDuplicateWorkspaceRequest instantiates a new DuplicateWorkspaceRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDuplicateWorkspaceRequestWithDefaults

`func NewDuplicateWorkspaceRequestWithDefaults() *DuplicateWorkspaceRequest`

NewDuplicateWorkspaceRequestWithDefaults instantiates a new DuplicateWorkspaceRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetNewName

`func (o *DuplicateWorkspaceRequest) GetNewName() string`

GetNewName returns the NewName field if non-nil, zero value otherwise.

### GetNewNameOk

`func (o *DuplicateWorkspaceRequest) GetNewNameOk() (*string, bool)`

GetNewNameOk returns a tuple with the NewName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNewName

`func (o *DuplicateWorkspaceRequest) SetNewName(v string)`

SetNewName sets NewName field to given value.

### HasNewName

`func (o *DuplicateWorkspaceRequest) HasNewName() bool`

HasNewName returns a boolean if a field has been set.

### SetNewNameNil

`func (o *DuplicateWorkspaceRequest) SetNewNameNil(b bool)`

 SetNewNameNil sets the value for NewName to be an explicit nil

### UnsetNewName
`func (o *DuplicateWorkspaceRequest) UnsetNewName()`

UnsetNewName ensures that no value is present for NewName, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


