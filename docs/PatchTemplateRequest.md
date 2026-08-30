# PatchTemplateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Attributes** | Pointer to [**[]TemplateAttributeInput**](TemplateAttributeInput.md) | Structured template attributes with optional per-template default values. If provided, replaces attribute associations. | [optional] 
**Groups** | Pointer to [**[]TemplateGroupInput**](TemplateGroupInput.md) | Ordered attribute groups for organizing template fields into visual UI sections. | [optional] 
**Name** | Pointer to **NullableString** | New human-readable name of the template. | [optional] 
**Description** | Pointer to **NullableString** | New description for the template. | [optional] 
**Category** | Pointer to **NullableString** | New category tag for navigation grouping. | [optional] 
**AttributeIds** | Pointer to **[]string** | Flat list of attribute UUIDs to associate. | [optional] 
**AttributeSlugs** | Pointer to **[]string** | Flat list of attribute slugs to associate. | [optional] 
**Slug** | Pointer to **NullableString** | New unique slug identifier within the project. | [optional] 

## Methods

### NewPatchTemplateRequest

`func NewPatchTemplateRequest() *PatchTemplateRequest`

NewPatchTemplateRequest instantiates a new PatchTemplateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchTemplateRequestWithDefaults

`func NewPatchTemplateRequestWithDefaults() *PatchTemplateRequest`

NewPatchTemplateRequestWithDefaults instantiates a new PatchTemplateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributes

`func (o *PatchTemplateRequest) GetAttributes() []TemplateAttributeInput`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *PatchTemplateRequest) GetAttributesOk() (*[]TemplateAttributeInput, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *PatchTemplateRequest) SetAttributes(v []TemplateAttributeInput)`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *PatchTemplateRequest) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.

### SetAttributesNil

`func (o *PatchTemplateRequest) SetAttributesNil(b bool)`

 SetAttributesNil sets the value for Attributes to be an explicit nil

### UnsetAttributes
`func (o *PatchTemplateRequest) UnsetAttributes()`

UnsetAttributes ensures that no value is present for Attributes, not even an explicit nil
### GetGroups

`func (o *PatchTemplateRequest) GetGroups() []TemplateGroupInput`

GetGroups returns the Groups field if non-nil, zero value otherwise.

### GetGroupsOk

`func (o *PatchTemplateRequest) GetGroupsOk() (*[]TemplateGroupInput, bool)`

GetGroupsOk returns a tuple with the Groups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroups

`func (o *PatchTemplateRequest) SetGroups(v []TemplateGroupInput)`

SetGroups sets Groups field to given value.

### HasGroups

`func (o *PatchTemplateRequest) HasGroups() bool`

HasGroups returns a boolean if a field has been set.

### SetGroupsNil

`func (o *PatchTemplateRequest) SetGroupsNil(b bool)`

 SetGroupsNil sets the value for Groups to be an explicit nil

### UnsetGroups
`func (o *PatchTemplateRequest) UnsetGroups()`

UnsetGroups ensures that no value is present for Groups, not even an explicit nil
### GetName

`func (o *PatchTemplateRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *PatchTemplateRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *PatchTemplateRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *PatchTemplateRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *PatchTemplateRequest) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *PatchTemplateRequest) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetDescription

`func (o *PatchTemplateRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *PatchTemplateRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *PatchTemplateRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *PatchTemplateRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *PatchTemplateRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *PatchTemplateRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetCategory

`func (o *PatchTemplateRequest) GetCategory() string`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *PatchTemplateRequest) GetCategoryOk() (*string, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *PatchTemplateRequest) SetCategory(v string)`

SetCategory sets Category field to given value.

### HasCategory

`func (o *PatchTemplateRequest) HasCategory() bool`

HasCategory returns a boolean if a field has been set.

### SetCategoryNil

`func (o *PatchTemplateRequest) SetCategoryNil(b bool)`

 SetCategoryNil sets the value for Category to be an explicit nil

### UnsetCategory
`func (o *PatchTemplateRequest) UnsetCategory()`

UnsetCategory ensures that no value is present for Category, not even an explicit nil
### GetAttributeIds

`func (o *PatchTemplateRequest) GetAttributeIds() []string`

GetAttributeIds returns the AttributeIds field if non-nil, zero value otherwise.

### GetAttributeIdsOk

`func (o *PatchTemplateRequest) GetAttributeIdsOk() (*[]string, bool)`

GetAttributeIdsOk returns a tuple with the AttributeIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeIds

`func (o *PatchTemplateRequest) SetAttributeIds(v []string)`

SetAttributeIds sets AttributeIds field to given value.

### HasAttributeIds

`func (o *PatchTemplateRequest) HasAttributeIds() bool`

HasAttributeIds returns a boolean if a field has been set.

### SetAttributeIdsNil

`func (o *PatchTemplateRequest) SetAttributeIdsNil(b bool)`

 SetAttributeIdsNil sets the value for AttributeIds to be an explicit nil

### UnsetAttributeIds
`func (o *PatchTemplateRequest) UnsetAttributeIds()`

UnsetAttributeIds ensures that no value is present for AttributeIds, not even an explicit nil
### GetAttributeSlugs

`func (o *PatchTemplateRequest) GetAttributeSlugs() []string`

GetAttributeSlugs returns the AttributeSlugs field if non-nil, zero value otherwise.

### GetAttributeSlugsOk

`func (o *PatchTemplateRequest) GetAttributeSlugsOk() (*[]string, bool)`

GetAttributeSlugsOk returns a tuple with the AttributeSlugs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeSlugs

`func (o *PatchTemplateRequest) SetAttributeSlugs(v []string)`

SetAttributeSlugs sets AttributeSlugs field to given value.

### HasAttributeSlugs

`func (o *PatchTemplateRequest) HasAttributeSlugs() bool`

HasAttributeSlugs returns a boolean if a field has been set.

### SetAttributeSlugsNil

`func (o *PatchTemplateRequest) SetAttributeSlugsNil(b bool)`

 SetAttributeSlugsNil sets the value for AttributeSlugs to be an explicit nil

### UnsetAttributeSlugs
`func (o *PatchTemplateRequest) UnsetAttributeSlugs()`

UnsetAttributeSlugs ensures that no value is present for AttributeSlugs, not even an explicit nil
### GetSlug

`func (o *PatchTemplateRequest) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *PatchTemplateRequest) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *PatchTemplateRequest) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *PatchTemplateRequest) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### SetSlugNil

`func (o *PatchTemplateRequest) SetSlugNil(b bool)`

 SetSlugNil sets the value for Slug to be an explicit nil

### UnsetSlug
`func (o *PatchTemplateRequest) UnsetSlug()`

UnsetSlug ensures that no value is present for Slug, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


