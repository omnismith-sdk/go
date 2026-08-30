# InstallMarketplaceBlueprintRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProjectId** | **string** | Target project UUID where templates and attributes will be provisioned | 
**IncludeDemoData** | Pointer to **bool** | Whether to install sample entities and records included in the blueprint package | [optional] [default to false]

## Methods

### NewInstallMarketplaceBlueprintRequest

`func NewInstallMarketplaceBlueprintRequest(projectId string, ) *InstallMarketplaceBlueprintRequest`

NewInstallMarketplaceBlueprintRequest instantiates a new InstallMarketplaceBlueprintRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInstallMarketplaceBlueprintRequestWithDefaults

`func NewInstallMarketplaceBlueprintRequestWithDefaults() *InstallMarketplaceBlueprintRequest`

NewInstallMarketplaceBlueprintRequestWithDefaults instantiates a new InstallMarketplaceBlueprintRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProjectId

`func (o *InstallMarketplaceBlueprintRequest) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *InstallMarketplaceBlueprintRequest) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *InstallMarketplaceBlueprintRequest) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.


### GetIncludeDemoData

`func (o *InstallMarketplaceBlueprintRequest) GetIncludeDemoData() bool`

GetIncludeDemoData returns the IncludeDemoData field if non-nil, zero value otherwise.

### GetIncludeDemoDataOk

`func (o *InstallMarketplaceBlueprintRequest) GetIncludeDemoDataOk() (*bool, bool)`

GetIncludeDemoDataOk returns a tuple with the IncludeDemoData field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIncludeDemoData

`func (o *InstallMarketplaceBlueprintRequest) SetIncludeDemoData(v bool)`

SetIncludeDemoData sets IncludeDemoData field to given value.

### HasIncludeDemoData

`func (o *InstallMarketplaceBlueprintRequest) HasIncludeDemoData() bool`

HasIncludeDemoData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


