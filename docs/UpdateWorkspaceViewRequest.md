# UpdateWorkspaceViewRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **NullableString** | Updated display label for the view pane tab or header | [optional] 
**Filters** | Pointer to **[]map[string]interface{}** | Updated dynamic filtering rules applied to entities in this view | [optional] 
**SearchString** | Pointer to **NullableString** | Updated search query string applied to entities in this view | [optional] 
**SearchMode** | Pointer to **NullableString** | Updated search execution mode (keyword or semantic) | [optional] 
**Sort** | Pointer to [**NullableUpdateWorkspaceViewRequestSort**](UpdateWorkspaceViewRequestSort.md) |  | [optional] 
**DisplayMode** | Pointer to **NullableString** | Updated presentation layout mode (table or grid) | [optional] 
**DisplayedColumns** | Pointer to **[]string** | Updated list of attribute slugs or UUIDs to display as columns | [optional] 
**PaneOrder** | Pointer to **NullableInt32** | Updated display sequence index within the workspace layout | [optional] 

## Methods

### NewUpdateWorkspaceViewRequest

`func NewUpdateWorkspaceViewRequest() *UpdateWorkspaceViewRequest`

NewUpdateWorkspaceViewRequest instantiates a new UpdateWorkspaceViewRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateWorkspaceViewRequestWithDefaults

`func NewUpdateWorkspaceViewRequestWithDefaults() *UpdateWorkspaceViewRequest`

NewUpdateWorkspaceViewRequestWithDefaults instantiates a new UpdateWorkspaceViewRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *UpdateWorkspaceViewRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateWorkspaceViewRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateWorkspaceViewRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *UpdateWorkspaceViewRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *UpdateWorkspaceViewRequest) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *UpdateWorkspaceViewRequest) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetFilters

`func (o *UpdateWorkspaceViewRequest) GetFilters() []map[string]interface{}`

GetFilters returns the Filters field if non-nil, zero value otherwise.

### GetFiltersOk

`func (o *UpdateWorkspaceViewRequest) GetFiltersOk() (*[]map[string]interface{}, bool)`

GetFiltersOk returns a tuple with the Filters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilters

`func (o *UpdateWorkspaceViewRequest) SetFilters(v []map[string]interface{})`

SetFilters sets Filters field to given value.

### HasFilters

`func (o *UpdateWorkspaceViewRequest) HasFilters() bool`

HasFilters returns a boolean if a field has been set.

### SetFiltersNil

`func (o *UpdateWorkspaceViewRequest) SetFiltersNil(b bool)`

 SetFiltersNil sets the value for Filters to be an explicit nil

### UnsetFilters
`func (o *UpdateWorkspaceViewRequest) UnsetFilters()`

UnsetFilters ensures that no value is present for Filters, not even an explicit nil
### GetSearchString

`func (o *UpdateWorkspaceViewRequest) GetSearchString() string`

GetSearchString returns the SearchString field if non-nil, zero value otherwise.

### GetSearchStringOk

`func (o *UpdateWorkspaceViewRequest) GetSearchStringOk() (*string, bool)`

GetSearchStringOk returns a tuple with the SearchString field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSearchString

`func (o *UpdateWorkspaceViewRequest) SetSearchString(v string)`

SetSearchString sets SearchString field to given value.

### HasSearchString

`func (o *UpdateWorkspaceViewRequest) HasSearchString() bool`

HasSearchString returns a boolean if a field has been set.

### SetSearchStringNil

`func (o *UpdateWorkspaceViewRequest) SetSearchStringNil(b bool)`

 SetSearchStringNil sets the value for SearchString to be an explicit nil

### UnsetSearchString
`func (o *UpdateWorkspaceViewRequest) UnsetSearchString()`

UnsetSearchString ensures that no value is present for SearchString, not even an explicit nil
### GetSearchMode

`func (o *UpdateWorkspaceViewRequest) GetSearchMode() string`

GetSearchMode returns the SearchMode field if non-nil, zero value otherwise.

### GetSearchModeOk

`func (o *UpdateWorkspaceViewRequest) GetSearchModeOk() (*string, bool)`

GetSearchModeOk returns a tuple with the SearchMode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSearchMode

`func (o *UpdateWorkspaceViewRequest) SetSearchMode(v string)`

SetSearchMode sets SearchMode field to given value.

### HasSearchMode

`func (o *UpdateWorkspaceViewRequest) HasSearchMode() bool`

HasSearchMode returns a boolean if a field has been set.

### SetSearchModeNil

`func (o *UpdateWorkspaceViewRequest) SetSearchModeNil(b bool)`

 SetSearchModeNil sets the value for SearchMode to be an explicit nil

### UnsetSearchMode
`func (o *UpdateWorkspaceViewRequest) UnsetSearchMode()`

UnsetSearchMode ensures that no value is present for SearchMode, not even an explicit nil
### GetSort

`func (o *UpdateWorkspaceViewRequest) GetSort() UpdateWorkspaceViewRequestSort`

GetSort returns the Sort field if non-nil, zero value otherwise.

### GetSortOk

`func (o *UpdateWorkspaceViewRequest) GetSortOk() (*UpdateWorkspaceViewRequestSort, bool)`

GetSortOk returns a tuple with the Sort field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSort

`func (o *UpdateWorkspaceViewRequest) SetSort(v UpdateWorkspaceViewRequestSort)`

SetSort sets Sort field to given value.

### HasSort

`func (o *UpdateWorkspaceViewRequest) HasSort() bool`

HasSort returns a boolean if a field has been set.

### SetSortNil

`func (o *UpdateWorkspaceViewRequest) SetSortNil(b bool)`

 SetSortNil sets the value for Sort to be an explicit nil

### UnsetSort
`func (o *UpdateWorkspaceViewRequest) UnsetSort()`

UnsetSort ensures that no value is present for Sort, not even an explicit nil
### GetDisplayMode

`func (o *UpdateWorkspaceViewRequest) GetDisplayMode() string`

GetDisplayMode returns the DisplayMode field if non-nil, zero value otherwise.

### GetDisplayModeOk

`func (o *UpdateWorkspaceViewRequest) GetDisplayModeOk() (*string, bool)`

GetDisplayModeOk returns a tuple with the DisplayMode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayMode

`func (o *UpdateWorkspaceViewRequest) SetDisplayMode(v string)`

SetDisplayMode sets DisplayMode field to given value.

### HasDisplayMode

`func (o *UpdateWorkspaceViewRequest) HasDisplayMode() bool`

HasDisplayMode returns a boolean if a field has been set.

### SetDisplayModeNil

`func (o *UpdateWorkspaceViewRequest) SetDisplayModeNil(b bool)`

 SetDisplayModeNil sets the value for DisplayMode to be an explicit nil

### UnsetDisplayMode
`func (o *UpdateWorkspaceViewRequest) UnsetDisplayMode()`

UnsetDisplayMode ensures that no value is present for DisplayMode, not even an explicit nil
### GetDisplayedColumns

`func (o *UpdateWorkspaceViewRequest) GetDisplayedColumns() []string`

GetDisplayedColumns returns the DisplayedColumns field if non-nil, zero value otherwise.

### GetDisplayedColumnsOk

`func (o *UpdateWorkspaceViewRequest) GetDisplayedColumnsOk() (*[]string, bool)`

GetDisplayedColumnsOk returns a tuple with the DisplayedColumns field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayedColumns

`func (o *UpdateWorkspaceViewRequest) SetDisplayedColumns(v []string)`

SetDisplayedColumns sets DisplayedColumns field to given value.

### HasDisplayedColumns

`func (o *UpdateWorkspaceViewRequest) HasDisplayedColumns() bool`

HasDisplayedColumns returns a boolean if a field has been set.

### SetDisplayedColumnsNil

`func (o *UpdateWorkspaceViewRequest) SetDisplayedColumnsNil(b bool)`

 SetDisplayedColumnsNil sets the value for DisplayedColumns to be an explicit nil

### UnsetDisplayedColumns
`func (o *UpdateWorkspaceViewRequest) UnsetDisplayedColumns()`

UnsetDisplayedColumns ensures that no value is present for DisplayedColumns, not even an explicit nil
### GetPaneOrder

`func (o *UpdateWorkspaceViewRequest) GetPaneOrder() int32`

GetPaneOrder returns the PaneOrder field if non-nil, zero value otherwise.

### GetPaneOrderOk

`func (o *UpdateWorkspaceViewRequest) GetPaneOrderOk() (*int32, bool)`

GetPaneOrderOk returns a tuple with the PaneOrder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPaneOrder

`func (o *UpdateWorkspaceViewRequest) SetPaneOrder(v int32)`

SetPaneOrder sets PaneOrder field to given value.

### HasPaneOrder

`func (o *UpdateWorkspaceViewRequest) HasPaneOrder() bool`

HasPaneOrder returns a boolean if a field has been set.

### SetPaneOrderNil

`func (o *UpdateWorkspaceViewRequest) SetPaneOrderNil(b bool)`

 SetPaneOrderNil sets the value for PaneOrder to be an explicit nil

### UnsetPaneOrder
`func (o *UpdateWorkspaceViewRequest) UnsetPaneOrder()`

UnsetPaneOrder ensures that no value is present for PaneOrder, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


