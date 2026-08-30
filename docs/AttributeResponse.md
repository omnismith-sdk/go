# AttributeResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Attribute UUID | [optional] 
**Slug** | Pointer to **NullableString** | Unique slug identifier within the project | [optional] 
**Name** | Pointer to **string** | Human-readable attribute name | [optional] 
**Description** | Pointer to **NullableString** | Attribute description | [optional] 
**AttributeType** | Pointer to **int32** | 0: Dimension, 1: Metric, 2: List, 3: Reference | [optional] 
**DataType** | Pointer to **int32** | 0: String, 1: Number, 2: Boolean, 3: Datetime, 4: Date, 5: File, 6: Image, 7: Markdown | [optional] 
**TemplateIds** | Pointer to **[]string** | Array of template UUIDs associated with this attribute | [optional] 
**ReferenceConfig** | Pointer to [**NullableAttributeResponseReferenceConfig**](AttributeResponseReferenceConfig.md) |  | [optional] 
**CreatedAt** | Pointer to **time.Time** | Creation timestamp | [optional] 
**UpdatedAt** | Pointer to **time.Time** | Last update timestamp | [optional] 
**DeletedAt** | Pointer to **NullableTime** | Deletion timestamp if soft-deleted | [optional] 

## Methods

### NewAttributeResponse

`func NewAttributeResponse() *AttributeResponse`

NewAttributeResponse instantiates a new AttributeResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAttributeResponseWithDefaults

`func NewAttributeResponseWithDefaults() *AttributeResponse`

NewAttributeResponseWithDefaults instantiates a new AttributeResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *AttributeResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AttributeResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AttributeResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *AttributeResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetSlug

`func (o *AttributeResponse) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *AttributeResponse) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *AttributeResponse) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *AttributeResponse) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### SetSlugNil

`func (o *AttributeResponse) SetSlugNil(b bool)`

 SetSlugNil sets the value for Slug to be an explicit nil

### UnsetSlug
`func (o *AttributeResponse) UnsetSlug()`

UnsetSlug ensures that no value is present for Slug, not even an explicit nil
### GetName

`func (o *AttributeResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *AttributeResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *AttributeResponse) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *AttributeResponse) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *AttributeResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *AttributeResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *AttributeResponse) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *AttributeResponse) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *AttributeResponse) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *AttributeResponse) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetAttributeType

`func (o *AttributeResponse) GetAttributeType() int32`

GetAttributeType returns the AttributeType field if non-nil, zero value otherwise.

### GetAttributeTypeOk

`func (o *AttributeResponse) GetAttributeTypeOk() (*int32, bool)`

GetAttributeTypeOk returns a tuple with the AttributeType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeType

`func (o *AttributeResponse) SetAttributeType(v int32)`

SetAttributeType sets AttributeType field to given value.

### HasAttributeType

`func (o *AttributeResponse) HasAttributeType() bool`

HasAttributeType returns a boolean if a field has been set.

### GetDataType

`func (o *AttributeResponse) GetDataType() int32`

GetDataType returns the DataType field if non-nil, zero value otherwise.

### GetDataTypeOk

`func (o *AttributeResponse) GetDataTypeOk() (*int32, bool)`

GetDataTypeOk returns a tuple with the DataType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataType

`func (o *AttributeResponse) SetDataType(v int32)`

SetDataType sets DataType field to given value.

### HasDataType

`func (o *AttributeResponse) HasDataType() bool`

HasDataType returns a boolean if a field has been set.

### GetTemplateIds

`func (o *AttributeResponse) GetTemplateIds() []string`

GetTemplateIds returns the TemplateIds field if non-nil, zero value otherwise.

### GetTemplateIdsOk

`func (o *AttributeResponse) GetTemplateIdsOk() (*[]string, bool)`

GetTemplateIdsOk returns a tuple with the TemplateIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateIds

`func (o *AttributeResponse) SetTemplateIds(v []string)`

SetTemplateIds sets TemplateIds field to given value.

### HasTemplateIds

`func (o *AttributeResponse) HasTemplateIds() bool`

HasTemplateIds returns a boolean if a field has been set.

### GetReferenceConfig

`func (o *AttributeResponse) GetReferenceConfig() AttributeResponseReferenceConfig`

GetReferenceConfig returns the ReferenceConfig field if non-nil, zero value otherwise.

### GetReferenceConfigOk

`func (o *AttributeResponse) GetReferenceConfigOk() (*AttributeResponseReferenceConfig, bool)`

GetReferenceConfigOk returns a tuple with the ReferenceConfig field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferenceConfig

`func (o *AttributeResponse) SetReferenceConfig(v AttributeResponseReferenceConfig)`

SetReferenceConfig sets ReferenceConfig field to given value.

### HasReferenceConfig

`func (o *AttributeResponse) HasReferenceConfig() bool`

HasReferenceConfig returns a boolean if a field has been set.

### SetReferenceConfigNil

`func (o *AttributeResponse) SetReferenceConfigNil(b bool)`

 SetReferenceConfigNil sets the value for ReferenceConfig to be an explicit nil

### UnsetReferenceConfig
`func (o *AttributeResponse) UnsetReferenceConfig()`

UnsetReferenceConfig ensures that no value is present for ReferenceConfig, not even an explicit nil
### GetCreatedAt

`func (o *AttributeResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *AttributeResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *AttributeResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *AttributeResponse) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *AttributeResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *AttributeResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *AttributeResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *AttributeResponse) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.

### GetDeletedAt

`func (o *AttributeResponse) GetDeletedAt() time.Time`

GetDeletedAt returns the DeletedAt field if non-nil, zero value otherwise.

### GetDeletedAtOk

`func (o *AttributeResponse) GetDeletedAtOk() (*time.Time, bool)`

GetDeletedAtOk returns a tuple with the DeletedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeletedAt

`func (o *AttributeResponse) SetDeletedAt(v time.Time)`

SetDeletedAt sets DeletedAt field to given value.

### HasDeletedAt

`func (o *AttributeResponse) HasDeletedAt() bool`

HasDeletedAt returns a boolean if a field has been set.

### SetDeletedAtNil

`func (o *AttributeResponse) SetDeletedAtNil(b bool)`

 SetDeletedAtNil sets the value for DeletedAt to be an explicit nil

### UnsetDeletedAt
`func (o *AttributeResponse) UnsetDeletedAt()`

UnsetDeletedAt ensures that no value is present for DeletedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


