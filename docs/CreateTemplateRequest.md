# CreateTemplateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Attributes** | Pointer to [**[]TemplateAttributeInput**](TemplateAttributeInput.md) | Structured list of template attributes with optional per-template default values. Preferred over flat attribute_ids. | [optional] 
**Groups** | Pointer to [**[]TemplateGroupInput**](TemplateGroupInput.md) | Optional ordered attribute groups for organizing template fields into visual UI sections (1 or 2 columns). | [optional] 
**Name** | **string** | Human-readable name of the template. | 
**Description** | Pointer to **NullableString** | Optional description of what entities conforming to this template represent. | [optional] 
**Category** | Pointer to **NullableString** | Optional category tag for grouping templates in navigation. | [optional] 
**AttributeIds** | Pointer to **[]string** | Flat list of attribute UUIDs to associate with this template without custom default values. | [optional] 
**AttributeSlugs** | Pointer to **[]string** | Flat list of attribute slugs to associate with this template by slug resolution. | [optional] 
**Id** | Pointer to **NullableString** | Optional explicit client-generated UUIDv7. Generated automatically if omitted. | [optional] 
**Slug** | Pointer to **NullableString** | Unique template slug identifier (letters, numbers, underscores). Auto-generated from name if omitted. | [optional] 

## Methods

### NewCreateTemplateRequest

`func NewCreateTemplateRequest(name string, ) *CreateTemplateRequest`

NewCreateTemplateRequest instantiates a new CreateTemplateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateTemplateRequestWithDefaults

`func NewCreateTemplateRequestWithDefaults() *CreateTemplateRequest`

NewCreateTemplateRequestWithDefaults instantiates a new CreateTemplateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributes

`func (o *CreateTemplateRequest) GetAttributes() []TemplateAttributeInput`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *CreateTemplateRequest) GetAttributesOk() (*[]TemplateAttributeInput, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *CreateTemplateRequest) SetAttributes(v []TemplateAttributeInput)`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *CreateTemplateRequest) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.

### GetGroups

`func (o *CreateTemplateRequest) GetGroups() []TemplateGroupInput`

GetGroups returns the Groups field if non-nil, zero value otherwise.

### GetGroupsOk

`func (o *CreateTemplateRequest) GetGroupsOk() (*[]TemplateGroupInput, bool)`

GetGroupsOk returns a tuple with the Groups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroups

`func (o *CreateTemplateRequest) SetGroups(v []TemplateGroupInput)`

SetGroups sets Groups field to given value.

### HasGroups

`func (o *CreateTemplateRequest) HasGroups() bool`

HasGroups returns a boolean if a field has been set.

### GetName

`func (o *CreateTemplateRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateTemplateRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateTemplateRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *CreateTemplateRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateTemplateRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateTemplateRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CreateTemplateRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *CreateTemplateRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *CreateTemplateRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetCategory

`func (o *CreateTemplateRequest) GetCategory() string`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *CreateTemplateRequest) GetCategoryOk() (*string, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *CreateTemplateRequest) SetCategory(v string)`

SetCategory sets Category field to given value.

### HasCategory

`func (o *CreateTemplateRequest) HasCategory() bool`

HasCategory returns a boolean if a field has been set.

### SetCategoryNil

`func (o *CreateTemplateRequest) SetCategoryNil(b bool)`

 SetCategoryNil sets the value for Category to be an explicit nil

### UnsetCategory
`func (o *CreateTemplateRequest) UnsetCategory()`

UnsetCategory ensures that no value is present for Category, not even an explicit nil
### GetAttributeIds

`func (o *CreateTemplateRequest) GetAttributeIds() []string`

GetAttributeIds returns the AttributeIds field if non-nil, zero value otherwise.

### GetAttributeIdsOk

`func (o *CreateTemplateRequest) GetAttributeIdsOk() (*[]string, bool)`

GetAttributeIdsOk returns a tuple with the AttributeIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeIds

`func (o *CreateTemplateRequest) SetAttributeIds(v []string)`

SetAttributeIds sets AttributeIds field to given value.

### HasAttributeIds

`func (o *CreateTemplateRequest) HasAttributeIds() bool`

HasAttributeIds returns a boolean if a field has been set.

### GetAttributeSlugs

`func (o *CreateTemplateRequest) GetAttributeSlugs() []string`

GetAttributeSlugs returns the AttributeSlugs field if non-nil, zero value otherwise.

### GetAttributeSlugsOk

`func (o *CreateTemplateRequest) GetAttributeSlugsOk() (*[]string, bool)`

GetAttributeSlugsOk returns a tuple with the AttributeSlugs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeSlugs

`func (o *CreateTemplateRequest) SetAttributeSlugs(v []string)`

SetAttributeSlugs sets AttributeSlugs field to given value.

### HasAttributeSlugs

`func (o *CreateTemplateRequest) HasAttributeSlugs() bool`

HasAttributeSlugs returns a boolean if a field has been set.

### GetId

`func (o *CreateTemplateRequest) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *CreateTemplateRequest) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *CreateTemplateRequest) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *CreateTemplateRequest) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *CreateTemplateRequest) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *CreateTemplateRequest) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetSlug

`func (o *CreateTemplateRequest) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *CreateTemplateRequest) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *CreateTemplateRequest) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *CreateTemplateRequest) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### SetSlugNil

`func (o *CreateTemplateRequest) SetSlugNil(b bool)`

 SetSlugNil sets the value for Slug to be an explicit nil

### UnsetSlug
`func (o *CreateTemplateRequest) UnsetSlug()`

UnsetSlug ensures that no value is present for Slug, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


