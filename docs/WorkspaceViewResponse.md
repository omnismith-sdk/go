# WorkspaceViewResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Workspace view unique identifier | [optional] 
**WorkspaceId** | Pointer to **string** | Parent workspace unique identifier | [optional] 
**TemplateId** | Pointer to **string** | Bound entity template unique identifier | [optional] 
**Name** | Pointer to **string** | Display name for the view pane tab or header | [optional] 
**Filters** | Pointer to **[]map[string]interface{}** | Dynamic filter rules applied to entities in this view | [optional] 
**SearchString** | Pointer to **NullableString** | Active search query string | [optional] 
**SearchMode** | Pointer to **string** | Search execution mode | [optional] 
**Sort** | Pointer to [**WorkspaceViewResponseSort**](WorkspaceViewResponseSort.md) |  | [optional] 
**DisplayMode** | Pointer to **string** | Presentation layout mode | [optional] 
**DisplayedColumns** | Pointer to **[]string** | List of displayed attribute slugs or UUIDs for table view | [optional] 
**PaneOrder** | Pointer to **int32** | Display sequence index of this pane within the workspace layout | [optional] 
**CreatedAt** | Pointer to **time.Time** | ISO 8601 creation timestamp | [optional] 
**UpdatedAt** | Pointer to **NullableTime** | ISO 8601 last update timestamp | [optional] 

## Methods

### NewWorkspaceViewResponse

`func NewWorkspaceViewResponse() *WorkspaceViewResponse`

NewWorkspaceViewResponse instantiates a new WorkspaceViewResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewWorkspaceViewResponseWithDefaults

`func NewWorkspaceViewResponseWithDefaults() *WorkspaceViewResponse`

NewWorkspaceViewResponseWithDefaults instantiates a new WorkspaceViewResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *WorkspaceViewResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *WorkspaceViewResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *WorkspaceViewResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *WorkspaceViewResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetWorkspaceId

`func (o *WorkspaceViewResponse) GetWorkspaceId() string`

GetWorkspaceId returns the WorkspaceId field if non-nil, zero value otherwise.

### GetWorkspaceIdOk

`func (o *WorkspaceViewResponse) GetWorkspaceIdOk() (*string, bool)`

GetWorkspaceIdOk returns a tuple with the WorkspaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkspaceId

`func (o *WorkspaceViewResponse) SetWorkspaceId(v string)`

SetWorkspaceId sets WorkspaceId field to given value.

### HasWorkspaceId

`func (o *WorkspaceViewResponse) HasWorkspaceId() bool`

HasWorkspaceId returns a boolean if a field has been set.

### GetTemplateId

`func (o *WorkspaceViewResponse) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *WorkspaceViewResponse) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *WorkspaceViewResponse) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *WorkspaceViewResponse) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetName

`func (o *WorkspaceViewResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *WorkspaceViewResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *WorkspaceViewResponse) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *WorkspaceViewResponse) HasName() bool`

HasName returns a boolean if a field has been set.

### GetFilters

`func (o *WorkspaceViewResponse) GetFilters() []map[string]interface{}`

GetFilters returns the Filters field if non-nil, zero value otherwise.

### GetFiltersOk

`func (o *WorkspaceViewResponse) GetFiltersOk() (*[]map[string]interface{}, bool)`

GetFiltersOk returns a tuple with the Filters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilters

`func (o *WorkspaceViewResponse) SetFilters(v []map[string]interface{})`

SetFilters sets Filters field to given value.

### HasFilters

`func (o *WorkspaceViewResponse) HasFilters() bool`

HasFilters returns a boolean if a field has been set.

### GetSearchString

`func (o *WorkspaceViewResponse) GetSearchString() string`

GetSearchString returns the SearchString field if non-nil, zero value otherwise.

### GetSearchStringOk

`func (o *WorkspaceViewResponse) GetSearchStringOk() (*string, bool)`

GetSearchStringOk returns a tuple with the SearchString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSearchString

`func (o *WorkspaceViewResponse) SetSearchString(v string)`

SetSearchString sets SearchString field to given value.

### HasSearchString

`func (o *WorkspaceViewResponse) HasSearchString() bool`

HasSearchString returns a boolean if a field has been set.

### SetSearchStringNil

`func (o *WorkspaceViewResponse) SetSearchStringNil(b bool)`

 SetSearchStringNil sets the value for SearchString to be an explicit nil

### UnsetSearchString
`func (o *WorkspaceViewResponse) UnsetSearchString()`

UnsetSearchString ensures that no value is present for SearchString, not even an explicit nil
### GetSearchMode

`func (o *WorkspaceViewResponse) GetSearchMode() string`

GetSearchMode returns the SearchMode field if non-nil, zero value otherwise.

### GetSearchModeOk

`func (o *WorkspaceViewResponse) GetSearchModeOk() (*string, bool)`

GetSearchModeOk returns a tuple with the SearchMode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSearchMode

`func (o *WorkspaceViewResponse) SetSearchMode(v string)`

SetSearchMode sets SearchMode field to given value.

### HasSearchMode

`func (o *WorkspaceViewResponse) HasSearchMode() bool`

HasSearchMode returns a boolean if a field has been set.

### GetSort

`func (o *WorkspaceViewResponse) GetSort() WorkspaceViewResponseSort`

GetSort returns the Sort field if non-nil, zero value otherwise.

### GetSortOk

`func (o *WorkspaceViewResponse) GetSortOk() (*WorkspaceViewResponseSort, bool)`

GetSortOk returns a tuple with the Sort field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSort

`func (o *WorkspaceViewResponse) SetSort(v WorkspaceViewResponseSort)`

SetSort sets Sort field to given value.

### HasSort

`func (o *WorkspaceViewResponse) HasSort() bool`

HasSort returns a boolean if a field has been set.

### GetDisplayMode

`func (o *WorkspaceViewResponse) GetDisplayMode() string`

GetDisplayMode returns the DisplayMode field if non-nil, zero value otherwise.

### GetDisplayModeOk

`func (o *WorkspaceViewResponse) GetDisplayModeOk() (*string, bool)`

GetDisplayModeOk returns a tuple with the DisplayMode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayMode

`func (o *WorkspaceViewResponse) SetDisplayMode(v string)`

SetDisplayMode sets DisplayMode field to given value.

### HasDisplayMode

`func (o *WorkspaceViewResponse) HasDisplayMode() bool`

HasDisplayMode returns a boolean if a field has been set.

### GetDisplayedColumns

`func (o *WorkspaceViewResponse) GetDisplayedColumns() []string`

GetDisplayedColumns returns the DisplayedColumns field if non-nil, zero value otherwise.

### GetDisplayedColumnsOk

`func (o *WorkspaceViewResponse) GetDisplayedColumnsOk() (*[]string, bool)`

GetDisplayedColumnsOk returns a tuple with the DisplayedColumns field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayedColumns

`func (o *WorkspaceViewResponse) SetDisplayedColumns(v []string)`

SetDisplayedColumns sets DisplayedColumns field to given value.

### HasDisplayedColumns

`func (o *WorkspaceViewResponse) HasDisplayedColumns() bool`

HasDisplayedColumns returns a boolean if a field has been set.

### GetPaneOrder

`func (o *WorkspaceViewResponse) GetPaneOrder() int32`

GetPaneOrder returns the PaneOrder field if non-nil, zero value otherwise.

### GetPaneOrderOk

`func (o *WorkspaceViewResponse) GetPaneOrderOk() (*int32, bool)`

GetPaneOrderOk returns a tuple with the PaneOrder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaneOrder

`func (o *WorkspaceViewResponse) SetPaneOrder(v int32)`

SetPaneOrder sets PaneOrder field to given value.

### HasPaneOrder

`func (o *WorkspaceViewResponse) HasPaneOrder() bool`

HasPaneOrder returns a boolean if a field has been set.

### GetCreatedAt

`func (o *WorkspaceViewResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *WorkspaceViewResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *WorkspaceViewResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *WorkspaceViewResponse) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *WorkspaceViewResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *WorkspaceViewResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *WorkspaceViewResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *WorkspaceViewResponse) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.

### SetUpdatedAtNil

`func (o *WorkspaceViewResponse) SetUpdatedAtNil(b bool)`

 SetUpdatedAtNil sets the value for UpdatedAt to be an explicit nil

### UnsetUpdatedAt
`func (o *WorkspaceViewResponse) UnsetUpdatedAt()`

UnsetUpdatedAt ensures that no value is present for UpdatedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


