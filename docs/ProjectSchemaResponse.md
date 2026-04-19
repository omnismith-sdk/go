# ProjectSchemaResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Attributes** | Pointer to [**[]AttributeResponse**](AttributeResponse.md) |  | [optional] 
**Templates** | Pointer to [**[]TemplateResponse**](TemplateResponse.md) |  | [optional] 
**ListItems** | Pointer to [**[]ListItemResponse**](ListItemResponse.md) |  | [optional] 
**ReferenceConfigs** | Pointer to [**[]ReferenceConfigResponse**](ReferenceConfigResponse.md) |  | [optional] 

## Methods

### NewProjectSchemaResponse

`func NewProjectSchemaResponse() *ProjectSchemaResponse`

NewProjectSchemaResponse instantiates a new ProjectSchemaResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProjectSchemaResponseWithDefaults

`func NewProjectSchemaResponseWithDefaults() *ProjectSchemaResponse`

NewProjectSchemaResponseWithDefaults instantiates a new ProjectSchemaResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributes

`func (o *ProjectSchemaResponse) GetAttributes() []AttributeResponse`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *ProjectSchemaResponse) GetAttributesOk() (*[]AttributeResponse, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *ProjectSchemaResponse) SetAttributes(v []AttributeResponse)`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *ProjectSchemaResponse) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.

### GetTemplates

`func (o *ProjectSchemaResponse) GetTemplates() []TemplateResponse`

GetTemplates returns the Templates field if non-nil, zero value otherwise.

### GetTemplatesOk

`func (o *ProjectSchemaResponse) GetTemplatesOk() (*[]TemplateResponse, bool)`

GetTemplatesOk returns a tuple with the Templates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplates

`func (o *ProjectSchemaResponse) SetTemplates(v []TemplateResponse)`

SetTemplates sets Templates field to given value.

### HasTemplates

`func (o *ProjectSchemaResponse) HasTemplates() bool`

HasTemplates returns a boolean if a field has been set.

### GetListItems

`func (o *ProjectSchemaResponse) GetListItems() []ListItemResponse`

GetListItems returns the ListItems field if non-nil, zero value otherwise.

### GetListItemsOk

`func (o *ProjectSchemaResponse) GetListItemsOk() (*[]ListItemResponse, bool)`

GetListItemsOk returns a tuple with the ListItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListItems

`func (o *ProjectSchemaResponse) SetListItems(v []ListItemResponse)`

SetListItems sets ListItems field to given value.

### HasListItems

`func (o *ProjectSchemaResponse) HasListItems() bool`

HasListItems returns a boolean if a field has been set.

### GetReferenceConfigs

`func (o *ProjectSchemaResponse) GetReferenceConfigs() []ReferenceConfigResponse`

GetReferenceConfigs returns the ReferenceConfigs field if non-nil, zero value otherwise.

### GetReferenceConfigsOk

`func (o *ProjectSchemaResponse) GetReferenceConfigsOk() (*[]ReferenceConfigResponse, bool)`

GetReferenceConfigsOk returns a tuple with the ReferenceConfigs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferenceConfigs

`func (o *ProjectSchemaResponse) SetReferenceConfigs(v []ReferenceConfigResponse)`

SetReferenceConfigs sets ReferenceConfigs field to given value.

### HasReferenceConfigs

`func (o *ProjectSchemaResponse) HasReferenceConfigs() bool`

HasReferenceConfigs returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


