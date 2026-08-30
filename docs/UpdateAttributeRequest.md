# UpdateAttributeRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Updated human-readable name of the attribute. | 
**TemplateIds** | Pointer to **[]string** | Complete list of template UUIDs associated with this attribute. Replaces current template associations while preserving restricted templates. | [optional] 
**Description** | Pointer to **NullableString** | Updated description of the attribute. | [optional] 
**ReferenceConfig** | Pointer to [**NullablePatchAttributeRequestReferenceConfig**](PatchAttributeRequestReferenceConfig.md) |  | [optional] 
**DataType** | Pointer to **NullableInt32** | Target data type for lossless transition on Dimension (0) attributes: Number(1)-&gt;String(0), Boolean(2)-&gt;String(0), Date(4)&lt;-&gt;Datetime(3), Date/Datetime-&gt;String(0), String(0)&lt;-&gt;Markdown(7). | [optional] 
**Slug** | Pointer to **NullableString** | Updated unique slug identifier within the project. | [optional] 

## Methods

### NewUpdateAttributeRequest

`func NewUpdateAttributeRequest(name string, ) *UpdateAttributeRequest`

NewUpdateAttributeRequest instantiates a new UpdateAttributeRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateAttributeRequestWithDefaults

`func NewUpdateAttributeRequestWithDefaults() *UpdateAttributeRequest`

NewUpdateAttributeRequestWithDefaults instantiates a new UpdateAttributeRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *UpdateAttributeRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateAttributeRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateAttributeRequest) SetName(v string)`

SetName sets Name field to given value.


### GetTemplateIds

`func (o *UpdateAttributeRequest) GetTemplateIds() []string`

GetTemplateIds returns the TemplateIds field if non-nil, zero value otherwise.

### GetTemplateIdsOk

`func (o *UpdateAttributeRequest) GetTemplateIdsOk() (*[]string, bool)`

GetTemplateIdsOk returns a tuple with the TemplateIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateIds

`func (o *UpdateAttributeRequest) SetTemplateIds(v []string)`

SetTemplateIds sets TemplateIds field to given value.

### HasTemplateIds

`func (o *UpdateAttributeRequest) HasTemplateIds() bool`

HasTemplateIds returns a boolean if a field has been set.

### GetDescription

`func (o *UpdateAttributeRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *UpdateAttributeRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *UpdateAttributeRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *UpdateAttributeRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *UpdateAttributeRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *UpdateAttributeRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetReferenceConfig

`func (o *UpdateAttributeRequest) GetReferenceConfig() PatchAttributeRequestReferenceConfig`

GetReferenceConfig returns the ReferenceConfig field if non-nil, zero value otherwise.

### GetReferenceConfigOk

`func (o *UpdateAttributeRequest) GetReferenceConfigOk() (*PatchAttributeRequestReferenceConfig, bool)`

GetReferenceConfigOk returns a tuple with the ReferenceConfig field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferenceConfig

`func (o *UpdateAttributeRequest) SetReferenceConfig(v PatchAttributeRequestReferenceConfig)`

SetReferenceConfig sets ReferenceConfig field to given value.

### HasReferenceConfig

`func (o *UpdateAttributeRequest) HasReferenceConfig() bool`

HasReferenceConfig returns a boolean if a field has been set.

### SetReferenceConfigNil

`func (o *UpdateAttributeRequest) SetReferenceConfigNil(b bool)`

 SetReferenceConfigNil sets the value for ReferenceConfig to be an explicit nil

### UnsetReferenceConfig
`func (o *UpdateAttributeRequest) UnsetReferenceConfig()`

UnsetReferenceConfig ensures that no value is present for ReferenceConfig, not even an explicit nil
### GetDataType

`func (o *UpdateAttributeRequest) GetDataType() int32`

GetDataType returns the DataType field if non-nil, zero value otherwise.

### GetDataTypeOk

`func (o *UpdateAttributeRequest) GetDataTypeOk() (*int32, bool)`

GetDataTypeOk returns a tuple with the DataType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataType

`func (o *UpdateAttributeRequest) SetDataType(v int32)`

SetDataType sets DataType field to given value.

### HasDataType

`func (o *UpdateAttributeRequest) HasDataType() bool`

HasDataType returns a boolean if a field has been set.

### SetDataTypeNil

`func (o *UpdateAttributeRequest) SetDataTypeNil(b bool)`

 SetDataTypeNil sets the value for DataType to be an explicit nil

### UnsetDataType
`func (o *UpdateAttributeRequest) UnsetDataType()`

UnsetDataType ensures that no value is present for DataType, not even an explicit nil
### GetSlug

`func (o *UpdateAttributeRequest) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *UpdateAttributeRequest) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *UpdateAttributeRequest) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *UpdateAttributeRequest) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### SetSlugNil

`func (o *UpdateAttributeRequest) SetSlugNil(b bool)`

 SetSlugNil sets the value for Slug to be an explicit nil

### UnsetSlug
`func (o *UpdateAttributeRequest) UnsetSlug()`

UnsetSlug ensures that no value is present for Slug, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


