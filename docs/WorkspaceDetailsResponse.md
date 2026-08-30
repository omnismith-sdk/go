# WorkspaceDetailsResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Workspace unique identifier | [optional] 
**Name** | Pointer to **string** | Display name of the workspace | [optional] 
**Description** | Pointer to **string** | Detailed workspace description | [optional] 
**Layout** | Pointer to **string** | Multi-pane layout structure | [optional] 
**IsDefault** | Pointer to **bool** | Whether this workspace is designated as the default project view | [optional] 
**SortOrder** | Pointer to **int32** | Display ordering index in the workspace navigation switcher | [optional] 
**Views** | Pointer to [**[]WorkspaceViewResponse**](WorkspaceViewResponse.md) | Ordered list of view panes attached to this workspace | [optional] 
**CreatedAt** | Pointer to **time.Time** | ISO 8601 creation timestamp | [optional] 
**UpdatedAt** | Pointer to **NullableTime** | ISO 8601 last update timestamp | [optional] 

## Methods

### NewWorkspaceDetailsResponse

`func NewWorkspaceDetailsResponse() *WorkspaceDetailsResponse`

NewWorkspaceDetailsResponse instantiates a new WorkspaceDetailsResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWorkspaceDetailsResponseWithDefaults

`func NewWorkspaceDetailsResponseWithDefaults() *WorkspaceDetailsResponse`

NewWorkspaceDetailsResponseWithDefaults instantiates a new WorkspaceDetailsResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *WorkspaceDetailsResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *WorkspaceDetailsResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *WorkspaceDetailsResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *WorkspaceDetailsResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *WorkspaceDetailsResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *WorkspaceDetailsResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *WorkspaceDetailsResponse) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *WorkspaceDetailsResponse) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *WorkspaceDetailsResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *WorkspaceDetailsResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *WorkspaceDetailsResponse) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *WorkspaceDetailsResponse) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetLayout

`func (o *WorkspaceDetailsResponse) GetLayout() string`

GetLayout returns the Layout field if non-nil, zero value otherwise.

### GetLayoutOk

`func (o *WorkspaceDetailsResponse) GetLayoutOk() (*string, bool)`

GetLayoutOk returns a tuple with the Layout field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLayout

`func (o *WorkspaceDetailsResponse) SetLayout(v string)`

SetLayout sets Layout field to given value.

### HasLayout

`func (o *WorkspaceDetailsResponse) HasLayout() bool`

HasLayout returns a boolean if a field has been set.

### GetIsDefault

`func (o *WorkspaceDetailsResponse) GetIsDefault() bool`

GetIsDefault returns the IsDefault field if non-nil, zero value otherwise.

### GetIsDefaultOk

`func (o *WorkspaceDetailsResponse) GetIsDefaultOk() (*bool, bool)`

GetIsDefaultOk returns a tuple with the IsDefault field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDefault

`func (o *WorkspaceDetailsResponse) SetIsDefault(v bool)`

SetIsDefault sets IsDefault field to given value.

### HasIsDefault

`func (o *WorkspaceDetailsResponse) HasIsDefault() bool`

HasIsDefault returns a boolean if a field has been set.

### GetSortOrder

`func (o *WorkspaceDetailsResponse) GetSortOrder() int32`

GetSortOrder returns the SortOrder field if non-nil, zero value otherwise.

### GetSortOrderOk

`func (o *WorkspaceDetailsResponse) GetSortOrderOk() (*int32, bool)`

GetSortOrderOk returns a tuple with the SortOrder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortOrder

`func (o *WorkspaceDetailsResponse) SetSortOrder(v int32)`

SetSortOrder sets SortOrder field to given value.

### HasSortOrder

`func (o *WorkspaceDetailsResponse) HasSortOrder() bool`

HasSortOrder returns a boolean if a field has been set.

### GetViews

`func (o *WorkspaceDetailsResponse) GetViews() []WorkspaceViewResponse`

GetViews returns the Views field if non-nil, zero value otherwise.

### GetViewsOk

`func (o *WorkspaceDetailsResponse) GetViewsOk() (*[]WorkspaceViewResponse, bool)`

GetViewsOk returns a tuple with the Views field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetViews

`func (o *WorkspaceDetailsResponse) SetViews(v []WorkspaceViewResponse)`

SetViews sets Views field to given value.

### HasViews

`func (o *WorkspaceDetailsResponse) HasViews() bool`

HasViews returns a boolean if a field has been set.

### GetCreatedAt

`func (o *WorkspaceDetailsResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *WorkspaceDetailsResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *WorkspaceDetailsResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *WorkspaceDetailsResponse) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *WorkspaceDetailsResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *WorkspaceDetailsResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *WorkspaceDetailsResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *WorkspaceDetailsResponse) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.

### SetUpdatedAtNil

`func (o *WorkspaceDetailsResponse) SetUpdatedAtNil(b bool)`

 SetUpdatedAtNil sets the value for UpdatedAt to be an explicit nil

### UnsetUpdatedAt
`func (o *WorkspaceDetailsResponse) UnsetUpdatedAt()`

UnsetUpdatedAt ensures that no value is present for UpdatedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


