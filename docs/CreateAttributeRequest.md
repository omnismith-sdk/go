# CreateAttributeRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Human-readable name of the attribute. | 
**AttributeType** | **int32** | Attribute kind. 0: Dimension (standard field), 1: Metric (time-series observation), 2: List (enumerated choice option), 3: Reference (foreign entity pointer). | 
**DataType** | **int32** | Storage data type. 0: String, 1: Number, 2: Boolean, 3: Datetime, 4: Date, 5: File, 6: Image, 7: Markdown. | 
**TemplateIds** | Pointer to **[]string** | Optional array of template UUIDs to immediately associate this attribute with. | [optional] 
**Description** | Pointer to **NullableString** | Optional descriptive summary of the attribute and its business purpose. | [optional] 
**ReferenceConfig** | Pointer to [**NullableCreateAttributeRequestReferenceConfig**](CreateAttributeRequestReferenceConfig.md) |  | [optional] 
**Id** | Pointer to **NullableString** | Optional explicit client-generated UUIDv7. If omitted, a UUIDv7 is automatically generated. | [optional] 
**Slug** | Pointer to **NullableString** | Unique slug identifier within the project (letters, numbers, underscores). If omitted, generated automatically from name. | [optional] 

## Methods

### NewCreateAttributeRequest

`func NewCreateAttributeRequest(name string, attributeType int32, dataType int32, ) *CreateAttributeRequest`

NewCreateAttributeRequest instantiates a new CreateAttributeRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateAttributeRequestWithDefaults

`func NewCreateAttributeRequestWithDefaults() *CreateAttributeRequest`

NewCreateAttributeRequestWithDefaults instantiates a new CreateAttributeRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreateAttributeRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateAttributeRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateAttributeRequest) SetName(v string)`

SetName sets Name field to given value.


### GetAttributeType

`func (o *CreateAttributeRequest) GetAttributeType() int32`

GetAttributeType returns the AttributeType field if non-nil, zero value otherwise.

### GetAttributeTypeOk

`func (o *CreateAttributeRequest) GetAttributeTypeOk() (*int32, bool)`

GetAttributeTypeOk returns a tuple with the AttributeType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeType

`func (o *CreateAttributeRequest) SetAttributeType(v int32)`

SetAttributeType sets AttributeType field to given value.


### GetDataType

`func (o *CreateAttributeRequest) GetDataType() int32`

GetDataType returns the DataType field if non-nil, zero value otherwise.

### GetDataTypeOk

`func (o *CreateAttributeRequest) GetDataTypeOk() (*int32, bool)`

GetDataTypeOk returns a tuple with the DataType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataType

`func (o *CreateAttributeRequest) SetDataType(v int32)`

SetDataType sets DataType field to given value.


### GetTemplateIds

`func (o *CreateAttributeRequest) GetTemplateIds() []string`

GetTemplateIds returns the TemplateIds field if non-nil, zero value otherwise.

### GetTemplateIdsOk

`func (o *CreateAttributeRequest) GetTemplateIdsOk() (*[]string, bool)`

GetTemplateIdsOk returns a tuple with the TemplateIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateIds

`func (o *CreateAttributeRequest) SetTemplateIds(v []string)`

SetTemplateIds sets TemplateIds field to given value.

### HasTemplateIds

`func (o *CreateAttributeRequest) HasTemplateIds() bool`

HasTemplateIds returns a boolean if a field has been set.

### GetDescription

`func (o *CreateAttributeRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateAttributeRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateAttributeRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CreateAttributeRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *CreateAttributeRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *CreateAttributeRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetReferenceConfig

`func (o *CreateAttributeRequest) GetReferenceConfig() CreateAttributeRequestReferenceConfig`

GetReferenceConfig returns the ReferenceConfig field if non-nil, zero value otherwise.

### GetReferenceConfigOk

`func (o *CreateAttributeRequest) GetReferenceConfigOk() (*CreateAttributeRequestReferenceConfig, bool)`

GetReferenceConfigOk returns a tuple with the ReferenceConfig field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferenceConfig

`func (o *CreateAttributeRequest) SetReferenceConfig(v CreateAttributeRequestReferenceConfig)`

SetReferenceConfig sets ReferenceConfig field to given value.

### HasReferenceConfig

`func (o *CreateAttributeRequest) HasReferenceConfig() bool`

HasReferenceConfig returns a boolean if a field has been set.

### SetReferenceConfigNil

`func (o *CreateAttributeRequest) SetReferenceConfigNil(b bool)`

 SetReferenceConfigNil sets the value for ReferenceConfig to be an explicit nil

### UnsetReferenceConfig
`func (o *CreateAttributeRequest) UnsetReferenceConfig()`

UnsetReferenceConfig ensures that no value is present for ReferenceConfig, not even an explicit nil
### GetId

`func (o *CreateAttributeRequest) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *CreateAttributeRequest) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *CreateAttributeRequest) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *CreateAttributeRequest) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *CreateAttributeRequest) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *CreateAttributeRequest) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetSlug

`func (o *CreateAttributeRequest) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *CreateAttributeRequest) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *CreateAttributeRequest) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *CreateAttributeRequest) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### SetSlugNil

`func (o *CreateAttributeRequest) SetSlugNil(b bool)`

 SetSlugNil sets the value for Slug to be an explicit nil

### UnsetSlug
`func (o *CreateAttributeRequest) UnsetSlug()`

UnsetSlug ensures that no value is present for Slug, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


