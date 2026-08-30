# PatchAttributeRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **NullableString** | New human-readable name for the attribute. | [optional] 
**TemplateIds** | Pointer to **[]string** | Updated array of template UUIDs to associate. When provided, replaces the template list while safely merging restricted templates. | [optional] 
**Description** | Pointer to **NullableString** | New descriptive text for the attribute. Pass null to clear. | [optional] 
**ReferenceConfig** | Pointer to [**NullablePatchAttributeRequestReferenceConfig**](PatchAttributeRequestReferenceConfig.md) |  | [optional] 
**DataType** | Pointer to **NullableInt32** | Target data type for lossless transition on Dimension (0) attributes: Number(1)-&gt;String(0), Boolean(2)-&gt;String(0), Date(4)&lt;-&gt;Datetime(3), Date/Datetime-&gt;String(0), String(0)&lt;-&gt;Markdown(7). | [optional] 
**Slug** | Pointer to **NullableString** | New unique slug identifier within the project. | [optional] 

## Methods

### NewPatchAttributeRequest

`func NewPatchAttributeRequest() *PatchAttributeRequest`

NewPatchAttributeRequest instantiates a new PatchAttributeRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPatchAttributeRequestWithDefaults

`func NewPatchAttributeRequestWithDefaults() *PatchAttributeRequest`

NewPatchAttributeRequestWithDefaults instantiates a new PatchAttributeRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *PatchAttributeRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *PatchAttributeRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *PatchAttributeRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *PatchAttributeRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *PatchAttributeRequest) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *PatchAttributeRequest) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetTemplateIds

`func (o *PatchAttributeRequest) GetTemplateIds() []string`

GetTemplateIds returns the TemplateIds field if non-nil, zero value otherwise.

### GetTemplateIdsOk

`func (o *PatchAttributeRequest) GetTemplateIdsOk() (*[]string, bool)`

GetTemplateIdsOk returns a tuple with the TemplateIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateIds

`func (o *PatchAttributeRequest) SetTemplateIds(v []string)`

SetTemplateIds sets TemplateIds field to given value.

### HasTemplateIds

`func (o *PatchAttributeRequest) HasTemplateIds() bool`

HasTemplateIds returns a boolean if a field has been set.

### SetTemplateIdsNil

`func (o *PatchAttributeRequest) SetTemplateIdsNil(b bool)`

 SetTemplateIdsNil sets the value for TemplateIds to be an explicit nil

### UnsetTemplateIds
`func (o *PatchAttributeRequest) UnsetTemplateIds()`

UnsetTemplateIds ensures that no value is present for TemplateIds, not even an explicit nil
### GetDescription

`func (o *PatchAttributeRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *PatchAttributeRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *PatchAttributeRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *PatchAttributeRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *PatchAttributeRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *PatchAttributeRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetReferenceConfig

`func (o *PatchAttributeRequest) GetReferenceConfig() PatchAttributeRequestReferenceConfig`

GetReferenceConfig returns the ReferenceConfig field if non-nil, zero value otherwise.

### GetReferenceConfigOk

`func (o *PatchAttributeRequest) GetReferenceConfigOk() (*PatchAttributeRequestReferenceConfig, bool)`

GetReferenceConfigOk returns a tuple with the ReferenceConfig field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferenceConfig

`func (o *PatchAttributeRequest) SetReferenceConfig(v PatchAttributeRequestReferenceConfig)`

SetReferenceConfig sets ReferenceConfig field to given value.

### HasReferenceConfig

`func (o *PatchAttributeRequest) HasReferenceConfig() bool`

HasReferenceConfig returns a boolean if a field has been set.

### SetReferenceConfigNil

`func (o *PatchAttributeRequest) SetReferenceConfigNil(b bool)`

 SetReferenceConfigNil sets the value for ReferenceConfig to be an explicit nil

### UnsetReferenceConfig
`func (o *PatchAttributeRequest) UnsetReferenceConfig()`

UnsetReferenceConfig ensures that no value is present for ReferenceConfig, not even an explicit nil
### GetDataType

`func (o *PatchAttributeRequest) GetDataType() int32`

GetDataType returns the DataType field if non-nil, zero value otherwise.

### GetDataTypeOk

`func (o *PatchAttributeRequest) GetDataTypeOk() (*int32, bool)`

GetDataTypeOk returns a tuple with the DataType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataType

`func (o *PatchAttributeRequest) SetDataType(v int32)`

SetDataType sets DataType field to given value.

### HasDataType

`func (o *PatchAttributeRequest) HasDataType() bool`

HasDataType returns a boolean if a field has been set.

### SetDataTypeNil

`func (o *PatchAttributeRequest) SetDataTypeNil(b bool)`

 SetDataTypeNil sets the value for DataType to be an explicit nil

### UnsetDataType
`func (o *PatchAttributeRequest) UnsetDataType()`

UnsetDataType ensures that no value is present for DataType, not even an explicit nil
### GetSlug

`func (o *PatchAttributeRequest) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *PatchAttributeRequest) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *PatchAttributeRequest) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *PatchAttributeRequest) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### SetSlugNil

`func (o *PatchAttributeRequest) SetSlugNil(b bool)`

 SetSlugNil sets the value for Slug to be an explicit nil

### UnsetSlug
`func (o *PatchAttributeRequest) UnsetSlug()`

UnsetSlug ensures that no value is present for Slug, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


