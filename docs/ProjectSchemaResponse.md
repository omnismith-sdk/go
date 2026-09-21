# ProjectSchemaResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ProjectId** | Pointer to **NullableString** | Unique identifier of the active project | [optional] 
**ProjectName** | Pointer to **NullableString** | Human-readable name of the active project | [optional] 
**Templates** | [**[]TemplateOverviewResponse**](TemplateOverviewResponse.md) | All active templates with bound attributes, business rules, and executable actions | 
**Attributes** | [**[]AttributeOverviewResponse**](AttributeOverviewResponse.md) | All active attributes with semantic types, list options, and foreign entity references | 

## Methods

### NewProjectSchemaResponse

`func NewProjectSchemaResponse(templates []TemplateOverviewResponse, attributes []AttributeOverviewResponse, ) *ProjectSchemaResponse`

NewProjectSchemaResponse instantiates a new ProjectSchemaResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProjectSchemaResponseWithDefaults

`func NewProjectSchemaResponseWithDefaults() *ProjectSchemaResponse`

NewProjectSchemaResponseWithDefaults instantiates a new ProjectSchemaResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetProjectId

`func (o *ProjectSchemaResponse) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *ProjectSchemaResponse) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *ProjectSchemaResponse) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.

### HasProjectId

`func (o *ProjectSchemaResponse) HasProjectId() bool`

HasProjectId returns a boolean if a field has been set.

### SetProjectIdNil

`func (o *ProjectSchemaResponse) SetProjectIdNil(b bool)`

 SetProjectIdNil sets the value for ProjectId to be an explicit nil

### UnsetProjectId
`func (o *ProjectSchemaResponse) UnsetProjectId()`

UnsetProjectId ensures that no value is present for ProjectId, not even an explicit nil
### GetProjectName

`func (o *ProjectSchemaResponse) GetProjectName() string`

GetProjectName returns the ProjectName field if non-nil, zero value otherwise.

### GetProjectNameOk

`func (o *ProjectSchemaResponse) GetProjectNameOk() (*string, bool)`

GetProjectNameOk returns a tuple with the ProjectName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectName

`func (o *ProjectSchemaResponse) SetProjectName(v string)`

SetProjectName sets ProjectName field to given value.

### HasProjectName

`func (o *ProjectSchemaResponse) HasProjectName() bool`

HasProjectName returns a boolean if a field has been set.

### SetProjectNameNil

`func (o *ProjectSchemaResponse) SetProjectNameNil(b bool)`

 SetProjectNameNil sets the value for ProjectName to be an explicit nil

### UnsetProjectName
`func (o *ProjectSchemaResponse) UnsetProjectName()`

UnsetProjectName ensures that no value is present for ProjectName, not even an explicit nil
### GetTemplates

`func (o *ProjectSchemaResponse) GetTemplates() []TemplateOverviewResponse`

GetTemplates returns the Templates field if non-nil, zero value otherwise.

### GetTemplatesOk

`func (o *ProjectSchemaResponse) GetTemplatesOk() (*[]TemplateOverviewResponse, bool)`

GetTemplatesOk returns a tuple with the Templates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplates

`func (o *ProjectSchemaResponse) SetTemplates(v []TemplateOverviewResponse)`

SetTemplates sets Templates field to given value.


### GetAttributes

`func (o *ProjectSchemaResponse) GetAttributes() []AttributeOverviewResponse`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *ProjectSchemaResponse) GetAttributesOk() (*[]AttributeOverviewResponse, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *ProjectSchemaResponse) SetAttributes(v []AttributeOverviewResponse)`

SetAttributes sets Attributes field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


