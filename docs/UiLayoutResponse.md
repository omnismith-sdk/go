# UiLayoutResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProjectId** | Pointer to **NullableString** | Unique identifier of the active project | [optional] 
**ProjectName** | Pointer to **NullableString** | Human-readable name of the active project | [optional] 
**Templates** | [**[]TemplateLayoutResponse**](TemplateLayoutResponse.md) | Visual form section groups and categories per template | 
**Actions** | [**[]ActionLayoutResponse**](ActionLayoutResponse.md) | Display icons and sort orders for template actions | 
**ListItems** | [**[]ListItemLayoutResponse**](ListItemLayoutResponse.md) | Display sort orders for list choice items | 

## Methods

### NewUiLayoutResponse

`func NewUiLayoutResponse(templates []TemplateLayoutResponse, actions []ActionLayoutResponse, listItems []ListItemLayoutResponse, ) *UiLayoutResponse`

NewUiLayoutResponse instantiates a new UiLayoutResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUiLayoutResponseWithDefaults

`func NewUiLayoutResponseWithDefaults() *UiLayoutResponse`

NewUiLayoutResponseWithDefaults instantiates a new UiLayoutResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProjectId

`func (o *UiLayoutResponse) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *UiLayoutResponse) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *UiLayoutResponse) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.

### HasProjectId

`func (o *UiLayoutResponse) HasProjectId() bool`

HasProjectId returns a boolean if a field has been set.

### SetProjectIdNil

`func (o *UiLayoutResponse) SetProjectIdNil(b bool)`

 SetProjectIdNil sets the value for ProjectId to be an explicit nil

### UnsetProjectId
`func (o *UiLayoutResponse) UnsetProjectId()`

UnsetProjectId ensures that no value is present for ProjectId, not even an explicit nil
### GetProjectName

`func (o *UiLayoutResponse) GetProjectName() string`

GetProjectName returns the ProjectName field if non-nil, zero value otherwise.

### GetProjectNameOk

`func (o *UiLayoutResponse) GetProjectNameOk() (*string, bool)`

GetProjectNameOk returns a tuple with the ProjectName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectName

`func (o *UiLayoutResponse) SetProjectName(v string)`

SetProjectName sets ProjectName field to given value.

### HasProjectName

`func (o *UiLayoutResponse) HasProjectName() bool`

HasProjectName returns a boolean if a field has been set.

### SetProjectNameNil

`func (o *UiLayoutResponse) SetProjectNameNil(b bool)`

 SetProjectNameNil sets the value for ProjectName to be an explicit nil

### UnsetProjectName
`func (o *UiLayoutResponse) UnsetProjectName()`

UnsetProjectName ensures that no value is present for ProjectName, not even an explicit nil
### GetTemplates

`func (o *UiLayoutResponse) GetTemplates() []TemplateLayoutResponse`

GetTemplates returns the Templates field if non-nil, zero value otherwise.

### GetTemplatesOk

`func (o *UiLayoutResponse) GetTemplatesOk() (*[]TemplateLayoutResponse, bool)`

GetTemplatesOk returns a tuple with the Templates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplates

`func (o *UiLayoutResponse) SetTemplates(v []TemplateLayoutResponse)`

SetTemplates sets Templates field to given value.


### GetActions

`func (o *UiLayoutResponse) GetActions() []ActionLayoutResponse`

GetActions returns the Actions field if non-nil, zero value otherwise.

### GetActionsOk

`func (o *UiLayoutResponse) GetActionsOk() (*[]ActionLayoutResponse, bool)`

GetActionsOk returns a tuple with the Actions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActions

`func (o *UiLayoutResponse) SetActions(v []ActionLayoutResponse)`

SetActions sets Actions field to given value.


### GetListItems

`func (o *UiLayoutResponse) GetListItems() []ListItemLayoutResponse`

GetListItems returns the ListItems field if non-nil, zero value otherwise.

### GetListItemsOk

`func (o *UiLayoutResponse) GetListItemsOk() (*[]ListItemLayoutResponse, bool)`

GetListItemsOk returns a tuple with the ListItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListItems

`func (o *UiLayoutResponse) SetListItems(v []ListItemLayoutResponse)`

SetListItems sets ListItems field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


