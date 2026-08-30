# UpdateWorkspaceRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **NullableString** | Updated display name of the workspace | [optional] 
**Description** | Pointer to **NullableString** | Updated description of the workspace purpose | [optional] 
**Layout** | Pointer to **NullableString** | Updated multi-pane grid layout arrangement | [optional] 
**IsDefault** | Pointer to **NullableBool** | Whether this workspace should become the default landing view | [optional] 
**SortOrder** | Pointer to **NullableInt32** | Visual display order in the workspace navigation switcher | [optional] 

## Methods

### NewUpdateWorkspaceRequest

`func NewUpdateWorkspaceRequest() *UpdateWorkspaceRequest`

NewUpdateWorkspaceRequest instantiates a new UpdateWorkspaceRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateWorkspaceRequestWithDefaults

`func NewUpdateWorkspaceRequestWithDefaults() *UpdateWorkspaceRequest`

NewUpdateWorkspaceRequestWithDefaults instantiates a new UpdateWorkspaceRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *UpdateWorkspaceRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateWorkspaceRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateWorkspaceRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *UpdateWorkspaceRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *UpdateWorkspaceRequest) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *UpdateWorkspaceRequest) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetDescription

`func (o *UpdateWorkspaceRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *UpdateWorkspaceRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *UpdateWorkspaceRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *UpdateWorkspaceRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *UpdateWorkspaceRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *UpdateWorkspaceRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetLayout

`func (o *UpdateWorkspaceRequest) GetLayout() string`

GetLayout returns the Layout field if non-nil, zero value otherwise.

### GetLayoutOk

`func (o *UpdateWorkspaceRequest) GetLayoutOk() (*string, bool)`

GetLayoutOk returns a tuple with the Layout field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLayout

`func (o *UpdateWorkspaceRequest) SetLayout(v string)`

SetLayout sets Layout field to given value.

### HasLayout

`func (o *UpdateWorkspaceRequest) HasLayout() bool`

HasLayout returns a boolean if a field has been set.

### SetLayoutNil

`func (o *UpdateWorkspaceRequest) SetLayoutNil(b bool)`

 SetLayoutNil sets the value for Layout to be an explicit nil

### UnsetLayout
`func (o *UpdateWorkspaceRequest) UnsetLayout()`

UnsetLayout ensures that no value is present for Layout, not even an explicit nil
### GetIsDefault

`func (o *UpdateWorkspaceRequest) GetIsDefault() bool`

GetIsDefault returns the IsDefault field if non-nil, zero value otherwise.

### GetIsDefaultOk

`func (o *UpdateWorkspaceRequest) GetIsDefaultOk() (*bool, bool)`

GetIsDefaultOk returns a tuple with the IsDefault field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDefault

`func (o *UpdateWorkspaceRequest) SetIsDefault(v bool)`

SetIsDefault sets IsDefault field to given value.

### HasIsDefault

`func (o *UpdateWorkspaceRequest) HasIsDefault() bool`

HasIsDefault returns a boolean if a field has been set.

### SetIsDefaultNil

`func (o *UpdateWorkspaceRequest) SetIsDefaultNil(b bool)`

 SetIsDefaultNil sets the value for IsDefault to be an explicit nil

### UnsetIsDefault
`func (o *UpdateWorkspaceRequest) UnsetIsDefault()`

UnsetIsDefault ensures that no value is present for IsDefault, not even an explicit nil
### GetSortOrder

`func (o *UpdateWorkspaceRequest) GetSortOrder() int32`

GetSortOrder returns the SortOrder field if non-nil, zero value otherwise.

### GetSortOrderOk

`func (o *UpdateWorkspaceRequest) GetSortOrderOk() (*int32, bool)`

GetSortOrderOk returns a tuple with the SortOrder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortOrder

`func (o *UpdateWorkspaceRequest) SetSortOrder(v int32)`

SetSortOrder sets SortOrder field to given value.

### HasSortOrder

`func (o *UpdateWorkspaceRequest) HasSortOrder() bool`

HasSortOrder returns a boolean if a field has been set.

### SetSortOrderNil

`func (o *UpdateWorkspaceRequest) SetSortOrderNil(b bool)`

 SetSortOrderNil sets the value for SortOrder to be an explicit nil

### UnsetSortOrder
`func (o *UpdateWorkspaceRequest) UnsetSortOrder()`

UnsetSortOrder ensures that no value is present for SortOrder, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


