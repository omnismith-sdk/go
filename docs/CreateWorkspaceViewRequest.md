# CreateWorkspaceViewRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | **string** | Target template ID defining entity schema bound to this view pane | 
**Name** | **string** | Display label for the view pane tab or header | 
**Filters** | Pointer to **[]map[string]interface{}** | Dynamic filtering rules applied to entities rendered in this view pane | [optional] 
**SearchString** | Pointer to **NullableString** | Initial search query string applied to entities in this view | [optional] 
**SearchMode** | Pointer to **string** | Search execution mode (keyword text search or semantic vector similarity search) | [optional] [default to "keyword"]
**Sort** | Pointer to [**NullableCreateWorkspaceViewRequestSort**](CreateWorkspaceViewRequestSort.md) |  | [optional] 
**DisplayMode** | Pointer to **string** | Presentation layout type for entity records (table or card grid) | [optional] [default to "table"]
**DisplayedColumns** | Pointer to **[]string** | List of attribute slugs or UUIDs to display as columns in table mode | [optional] 
**PaneOrder** | Pointer to **NullableInt32** | Display sequence index of this pane within the workspace layout | [optional] 

## Methods

### NewCreateWorkspaceViewRequest

`func NewCreateWorkspaceViewRequest(templateId string, name string, ) *CreateWorkspaceViewRequest`

NewCreateWorkspaceViewRequest instantiates a new CreateWorkspaceViewRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateWorkspaceViewRequestWithDefaults

`func NewCreateWorkspaceViewRequestWithDefaults() *CreateWorkspaceViewRequest`

NewCreateWorkspaceViewRequestWithDefaults instantiates a new CreateWorkspaceViewRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *CreateWorkspaceViewRequest) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *CreateWorkspaceViewRequest) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *CreateWorkspaceViewRequest) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.


### GetName

`func (o *CreateWorkspaceViewRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateWorkspaceViewRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateWorkspaceViewRequest) SetName(v string)`

SetName sets Name field to given value.


### GetFilters

`func (o *CreateWorkspaceViewRequest) GetFilters() []map[string]interface{}`

GetFilters returns the Filters field if non-nil, zero value otherwise.

### GetFiltersOk

`func (o *CreateWorkspaceViewRequest) GetFiltersOk() (*[]map[string]interface{}, bool)`

GetFiltersOk returns a tuple with the Filters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilters

`func (o *CreateWorkspaceViewRequest) SetFilters(v []map[string]interface{})`

SetFilters sets Filters field to given value.

### HasFilters

`func (o *CreateWorkspaceViewRequest) HasFilters() bool`

HasFilters returns a boolean if a field has been set.

### GetSearchString

`func (o *CreateWorkspaceViewRequest) GetSearchString() string`

GetSearchString returns the SearchString field if non-nil, zero value otherwise.

### GetSearchStringOk

`func (o *CreateWorkspaceViewRequest) GetSearchStringOk() (*string, bool)`

GetSearchStringOk returns a tuple with the SearchString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSearchString

`func (o *CreateWorkspaceViewRequest) SetSearchString(v string)`

SetSearchString sets SearchString field to given value.

### HasSearchString

`func (o *CreateWorkspaceViewRequest) HasSearchString() bool`

HasSearchString returns a boolean if a field has been set.

### SetSearchStringNil

`func (o *CreateWorkspaceViewRequest) SetSearchStringNil(b bool)`

 SetSearchStringNil sets the value for SearchString to be an explicit nil

### UnsetSearchString
`func (o *CreateWorkspaceViewRequest) UnsetSearchString()`

UnsetSearchString ensures that no value is present for SearchString, not even an explicit nil
### GetSearchMode

`func (o *CreateWorkspaceViewRequest) GetSearchMode() string`

GetSearchMode returns the SearchMode field if non-nil, zero value otherwise.

### GetSearchModeOk

`func (o *CreateWorkspaceViewRequest) GetSearchModeOk() (*string, bool)`

GetSearchModeOk returns a tuple with the SearchMode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSearchMode

`func (o *CreateWorkspaceViewRequest) SetSearchMode(v string)`

SetSearchMode sets SearchMode field to given value.

### HasSearchMode

`func (o *CreateWorkspaceViewRequest) HasSearchMode() bool`

HasSearchMode returns a boolean if a field has been set.

### GetSort

`func (o *CreateWorkspaceViewRequest) GetSort() CreateWorkspaceViewRequestSort`

GetSort returns the Sort field if non-nil, zero value otherwise.

### GetSortOk

`func (o *CreateWorkspaceViewRequest) GetSortOk() (*CreateWorkspaceViewRequestSort, bool)`

GetSortOk returns a tuple with the Sort field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSort

`func (o *CreateWorkspaceViewRequest) SetSort(v CreateWorkspaceViewRequestSort)`

SetSort sets Sort field to given value.

### HasSort

`func (o *CreateWorkspaceViewRequest) HasSort() bool`

HasSort returns a boolean if a field has been set.

### SetSortNil

`func (o *CreateWorkspaceViewRequest) SetSortNil(b bool)`

 SetSortNil sets the value for Sort to be an explicit nil

### UnsetSort
`func (o *CreateWorkspaceViewRequest) UnsetSort()`

UnsetSort ensures that no value is present for Sort, not even an explicit nil
### GetDisplayMode

`func (o *CreateWorkspaceViewRequest) GetDisplayMode() string`

GetDisplayMode returns the DisplayMode field if non-nil, zero value otherwise.

### GetDisplayModeOk

`func (o *CreateWorkspaceViewRequest) GetDisplayModeOk() (*string, bool)`

GetDisplayModeOk returns a tuple with the DisplayMode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayMode

`func (o *CreateWorkspaceViewRequest) SetDisplayMode(v string)`

SetDisplayMode sets DisplayMode field to given value.

### HasDisplayMode

`func (o *CreateWorkspaceViewRequest) HasDisplayMode() bool`

HasDisplayMode returns a boolean if a field has been set.

### GetDisplayedColumns

`func (o *CreateWorkspaceViewRequest) GetDisplayedColumns() []string`

GetDisplayedColumns returns the DisplayedColumns field if non-nil, zero value otherwise.

### GetDisplayedColumnsOk

`func (o *CreateWorkspaceViewRequest) GetDisplayedColumnsOk() (*[]string, bool)`

GetDisplayedColumnsOk returns a tuple with the DisplayedColumns field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayedColumns

`func (o *CreateWorkspaceViewRequest) SetDisplayedColumns(v []string)`

SetDisplayedColumns sets DisplayedColumns field to given value.

### HasDisplayedColumns

`func (o *CreateWorkspaceViewRequest) HasDisplayedColumns() bool`

HasDisplayedColumns returns a boolean if a field has been set.

### GetPaneOrder

`func (o *CreateWorkspaceViewRequest) GetPaneOrder() int32`

GetPaneOrder returns the PaneOrder field if non-nil, zero value otherwise.

### GetPaneOrderOk

`func (o *CreateWorkspaceViewRequest) GetPaneOrderOk() (*int32, bool)`

GetPaneOrderOk returns a tuple with the PaneOrder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaneOrder

`func (o *CreateWorkspaceViewRequest) SetPaneOrder(v int32)`

SetPaneOrder sets PaneOrder field to given value.

### HasPaneOrder

`func (o *CreateWorkspaceViewRequest) HasPaneOrder() bool`

HasPaneOrder returns a boolean if a field has been set.

### SetPaneOrderNil

`func (o *CreateWorkspaceViewRequest) SetPaneOrderNil(b bool)`

 SetPaneOrderNil sets the value for PaneOrder to be an explicit nil

### UnsetPaneOrder
`func (o *CreateWorkspaceViewRequest) UnsetPaneOrder()`

UnsetPaneOrder ensures that no value is present for PaneOrder, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


