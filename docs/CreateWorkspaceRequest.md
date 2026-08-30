# CreateWorkspaceRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Human-readable display name of the workspace | 
**Description** | Pointer to **string** | Detailed description of the workspace purpose and workflow | [optional] 
**Layout** | Pointer to **string** | Multi-pane grid layout arrangement | [optional] [default to "split-v"]
**IsDefault** | Pointer to **bool** | Whether this workspace serves as the default landing view for the project | [optional] [default to false]
**InitialTemplateIds** | Pointer to **[]string** | Optional list of entity template IDs to automatically create and mount as initial view panes | [optional] 

## Methods

### NewCreateWorkspaceRequest

`func NewCreateWorkspaceRequest(name string, ) *CreateWorkspaceRequest`

NewCreateWorkspaceRequest instantiates a new CreateWorkspaceRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateWorkspaceRequestWithDefaults

`func NewCreateWorkspaceRequestWithDefaults() *CreateWorkspaceRequest`

NewCreateWorkspaceRequestWithDefaults instantiates a new CreateWorkspaceRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreateWorkspaceRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateWorkspaceRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateWorkspaceRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *CreateWorkspaceRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateWorkspaceRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateWorkspaceRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CreateWorkspaceRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetLayout

`func (o *CreateWorkspaceRequest) GetLayout() string`

GetLayout returns the Layout field if non-nil, zero value otherwise.

### GetLayoutOk

`func (o *CreateWorkspaceRequest) GetLayoutOk() (*string, bool)`

GetLayoutOk returns a tuple with the Layout field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLayout

`func (o *CreateWorkspaceRequest) SetLayout(v string)`

SetLayout sets Layout field to given value.

### HasLayout

`func (o *CreateWorkspaceRequest) HasLayout() bool`

HasLayout returns a boolean if a field has been set.

### GetIsDefault

`func (o *CreateWorkspaceRequest) GetIsDefault() bool`

GetIsDefault returns the IsDefault field if non-nil, zero value otherwise.

### GetIsDefaultOk

`func (o *CreateWorkspaceRequest) GetIsDefaultOk() (*bool, bool)`

GetIsDefaultOk returns a tuple with the IsDefault field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDefault

`func (o *CreateWorkspaceRequest) SetIsDefault(v bool)`

SetIsDefault sets IsDefault field to given value.

### HasIsDefault

`func (o *CreateWorkspaceRequest) HasIsDefault() bool`

HasIsDefault returns a boolean if a field has been set.

### GetInitialTemplateIds

`func (o *CreateWorkspaceRequest) GetInitialTemplateIds() []string`

GetInitialTemplateIds returns the InitialTemplateIds field if non-nil, zero value otherwise.

### GetInitialTemplateIdsOk

`func (o *CreateWorkspaceRequest) GetInitialTemplateIdsOk() (*[]string, bool)`

GetInitialTemplateIdsOk returns a tuple with the InitialTemplateIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInitialTemplateIds

`func (o *CreateWorkspaceRequest) SetInitialTemplateIds(v []string)`

SetInitialTemplateIds sets InitialTemplateIds field to given value.

### HasInitialTemplateIds

`func (o *CreateWorkspaceRequest) HasInitialTemplateIds() bool`

HasInitialTemplateIds returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


