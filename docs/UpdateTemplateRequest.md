# UpdateTemplateRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Attributes** | Pointer to [**[]TemplateAttributeInput**](TemplateAttributeInput.md) | Structured template attributes with optional per-template default values. Preferred over flat attribute_ids. | [optional] 
**Groups** | Pointer to [**[]TemplateGroupInput**](TemplateGroupInput.md) | Ordered attribute groups for organizing template fields into visual UI sections. | [optional] 
**Name** | **string** | Updated human-readable name of the template. | 
**Description** | Pointer to **NullableString** | Updated description of the template. | [optional] 
**Category** | Pointer to **NullableString** | Updated category tag for grouping in navigation. | [optional] 
**AttributeIds** | Pointer to **[]string** | Flat list of attribute UUIDs to associate without custom defaults. | [optional] 
**AttributeSlugs** | Pointer to **[]string** | Flat list of attribute slugs to associate with this template. | [optional] 
**Slug** | Pointer to **NullableString** | Updated unique slug identifier within the project. | [optional] 

## Methods

### NewUpdateTemplateRequest

`func NewUpdateTemplateRequest(name string, ) *UpdateTemplateRequest`

NewUpdateTemplateRequest instantiates a new UpdateTemplateRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateTemplateRequestWithDefaults

`func NewUpdateTemplateRequestWithDefaults() *UpdateTemplateRequest`

NewUpdateTemplateRequestWithDefaults instantiates a new UpdateTemplateRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributes

`func (o *UpdateTemplateRequest) GetAttributes() []TemplateAttributeInput`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *UpdateTemplateRequest) GetAttributesOk() (*[]TemplateAttributeInput, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *UpdateTemplateRequest) SetAttributes(v []TemplateAttributeInput)`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *UpdateTemplateRequest) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.

### GetGroups

`func (o *UpdateTemplateRequest) GetGroups() []TemplateGroupInput`

GetGroups returns the Groups field if non-nil, zero value otherwise.

### GetGroupsOk

`func (o *UpdateTemplateRequest) GetGroupsOk() (*[]TemplateGroupInput, bool)`

GetGroupsOk returns a tuple with the Groups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroups

`func (o *UpdateTemplateRequest) SetGroups(v []TemplateGroupInput)`

SetGroups sets Groups field to given value.

### HasGroups

`func (o *UpdateTemplateRequest) HasGroups() bool`

HasGroups returns a boolean if a field has been set.

### GetName

`func (o *UpdateTemplateRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateTemplateRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateTemplateRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *UpdateTemplateRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *UpdateTemplateRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *UpdateTemplateRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *UpdateTemplateRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *UpdateTemplateRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *UpdateTemplateRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetCategory

`func (o *UpdateTemplateRequest) GetCategory() string`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *UpdateTemplateRequest) GetCategoryOk() (*string, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *UpdateTemplateRequest) SetCategory(v string)`

SetCategory sets Category field to given value.

### HasCategory

`func (o *UpdateTemplateRequest) HasCategory() bool`

HasCategory returns a boolean if a field has been set.

### SetCategoryNil

`func (o *UpdateTemplateRequest) SetCategoryNil(b bool)`

 SetCategoryNil sets the value for Category to be an explicit nil

### UnsetCategory
`func (o *UpdateTemplateRequest) UnsetCategory()`

UnsetCategory ensures that no value is present for Category, not even an explicit nil
### GetAttributeIds

`func (o *UpdateTemplateRequest) GetAttributeIds() []string`

GetAttributeIds returns the AttributeIds field if non-nil, zero value otherwise.

### GetAttributeIdsOk

`func (o *UpdateTemplateRequest) GetAttributeIdsOk() (*[]string, bool)`

GetAttributeIdsOk returns a tuple with the AttributeIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeIds

`func (o *UpdateTemplateRequest) SetAttributeIds(v []string)`

SetAttributeIds sets AttributeIds field to given value.

### HasAttributeIds

`func (o *UpdateTemplateRequest) HasAttributeIds() bool`

HasAttributeIds returns a boolean if a field has been set.

### GetAttributeSlugs

`func (o *UpdateTemplateRequest) GetAttributeSlugs() []string`

GetAttributeSlugs returns the AttributeSlugs field if non-nil, zero value otherwise.

### GetAttributeSlugsOk

`func (o *UpdateTemplateRequest) GetAttributeSlugsOk() (*[]string, bool)`

GetAttributeSlugsOk returns a tuple with the AttributeSlugs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeSlugs

`func (o *UpdateTemplateRequest) SetAttributeSlugs(v []string)`

SetAttributeSlugs sets AttributeSlugs field to given value.

### HasAttributeSlugs

`func (o *UpdateTemplateRequest) HasAttributeSlugs() bool`

HasAttributeSlugs returns a boolean if a field has been set.

### GetSlug

`func (o *UpdateTemplateRequest) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *UpdateTemplateRequest) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *UpdateTemplateRequest) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *UpdateTemplateRequest) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### SetSlugNil

`func (o *UpdateTemplateRequest) SetSlugNil(b bool)`

 SetSlugNil sets the value for Slug to be an explicit nil

### UnsetSlug
`func (o *UpdateTemplateRequest) UnsetSlug()`

UnsetSlug ensures that no value is present for Slug, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


