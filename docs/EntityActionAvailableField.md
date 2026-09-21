# EntityActionAvailableField

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | **string** |  | 
**Slug** | **NullableString** | Attribute slug; the key to use in &#x60;values&#x60;. Null for an attribute without a slug — use &#x60;attribute_id&#x60; then. | 
**Name** | **string** |  | 
**AttributeType** | **int32** | 0: Dimension, 2: List, 3: Reference (metrics are never action fields) | 
**DataType** | **int32** | 0: String, 1: Number, 2: Boolean, 3: Datetime, 4: Date, 5: File, 6: Image, 7: Markdown | 
**Required** | **bool** | Execution refuses an empty value with 422 keyed by &#x60;attributes.&lt;slug&gt;&#x60; | 
**Hint** | **NullableString** |  | 
**ListItems** | [**[]EntityActionAvailableFieldListItemsInner**](EntityActionAvailableFieldListItemsInner.md) | The choices of a list attribute; the value to send is the item &#x60;id&#x60;. Empty for other attribute types. | 
**ReferenceConfig** | [**NullableEntityActionAvailableFieldReferenceConfig**](EntityActionAvailableFieldReferenceConfig.md) |  | 

## Methods

### NewEntityActionAvailableField

`func NewEntityActionAvailableField(attributeId string, slug NullableString, name string, attributeType int32, dataType int32, required bool, hint NullableString, listItems []EntityActionAvailableFieldListItemsInner, referenceConfig NullableEntityActionAvailableFieldReferenceConfig, ) *EntityActionAvailableField`

NewEntityActionAvailableField instantiates a new EntityActionAvailableField object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityActionAvailableFieldWithDefaults

`func NewEntityActionAvailableFieldWithDefaults() *EntityActionAvailableField`

NewEntityActionAvailableFieldWithDefaults instantiates a new EntityActionAvailableField object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeId

`func (o *EntityActionAvailableField) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *EntityActionAvailableField) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *EntityActionAvailableField) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.


### GetSlug

`func (o *EntityActionAvailableField) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *EntityActionAvailableField) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *EntityActionAvailableField) SetSlug(v string)`

SetSlug sets Slug field to given value.


### SetSlugNil

`func (o *EntityActionAvailableField) SetSlugNil(b bool)`

 SetSlugNil sets the value for Slug to be an explicit nil

### UnsetSlug
`func (o *EntityActionAvailableField) UnsetSlug()`

UnsetSlug ensures that no value is present for Slug, not even an explicit nil
### GetName

`func (o *EntityActionAvailableField) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *EntityActionAvailableField) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *EntityActionAvailableField) SetName(v string)`

SetName sets Name field to given value.


### GetAttributeType

`func (o *EntityActionAvailableField) GetAttributeType() int32`

GetAttributeType returns the AttributeType field if non-nil, zero value otherwise.

### GetAttributeTypeOk

`func (o *EntityActionAvailableField) GetAttributeTypeOk() (*int32, bool)`

GetAttributeTypeOk returns a tuple with the AttributeType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeType

`func (o *EntityActionAvailableField) SetAttributeType(v int32)`

SetAttributeType sets AttributeType field to given value.


### GetDataType

`func (o *EntityActionAvailableField) GetDataType() int32`

GetDataType returns the DataType field if non-nil, zero value otherwise.

### GetDataTypeOk

`func (o *EntityActionAvailableField) GetDataTypeOk() (*int32, bool)`

GetDataTypeOk returns a tuple with the DataType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataType

`func (o *EntityActionAvailableField) SetDataType(v int32)`

SetDataType sets DataType field to given value.


### GetRequired

`func (o *EntityActionAvailableField) GetRequired() bool`

GetRequired returns the Required field if non-nil, zero value otherwise.

### GetRequiredOk

`func (o *EntityActionAvailableField) GetRequiredOk() (*bool, bool)`

GetRequiredOk returns a tuple with the Required field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequired

`func (o *EntityActionAvailableField) SetRequired(v bool)`

SetRequired sets Required field to given value.


### GetHint

`func (o *EntityActionAvailableField) GetHint() string`

GetHint returns the Hint field if non-nil, zero value otherwise.

### GetHintOk

`func (o *EntityActionAvailableField) GetHintOk() (*string, bool)`

GetHintOk returns a tuple with the Hint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHint

`func (o *EntityActionAvailableField) SetHint(v string)`

SetHint sets Hint field to given value.


### SetHintNil

`func (o *EntityActionAvailableField) SetHintNil(b bool)`

 SetHintNil sets the value for Hint to be an explicit nil

### UnsetHint
`func (o *EntityActionAvailableField) UnsetHint()`

UnsetHint ensures that no value is present for Hint, not even an explicit nil
### GetListItems

`func (o *EntityActionAvailableField) GetListItems() []EntityActionAvailableFieldListItemsInner`

GetListItems returns the ListItems field if non-nil, zero value otherwise.

### GetListItemsOk

`func (o *EntityActionAvailableField) GetListItemsOk() (*[]EntityActionAvailableFieldListItemsInner, bool)`

GetListItemsOk returns a tuple with the ListItems field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListItems

`func (o *EntityActionAvailableField) SetListItems(v []EntityActionAvailableFieldListItemsInner)`

SetListItems sets ListItems field to given value.


### GetReferenceConfig

`func (o *EntityActionAvailableField) GetReferenceConfig() EntityActionAvailableFieldReferenceConfig`

GetReferenceConfig returns the ReferenceConfig field if non-nil, zero value otherwise.

### GetReferenceConfigOk

`func (o *EntityActionAvailableField) GetReferenceConfigOk() (*EntityActionAvailableFieldReferenceConfig, bool)`

GetReferenceConfigOk returns a tuple with the ReferenceConfig field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferenceConfig

`func (o *EntityActionAvailableField) SetReferenceConfig(v EntityActionAvailableFieldReferenceConfig)`

SetReferenceConfig sets ReferenceConfig field to given value.


### SetReferenceConfigNil

`func (o *EntityActionAvailableField) SetReferenceConfigNil(b bool)`

 SetReferenceConfigNil sets the value for ReferenceConfig to be an explicit nil

### UnsetReferenceConfig
`func (o *EntityActionAvailableField) UnsetReferenceConfig()`

UnsetReferenceConfig ensures that no value is present for ReferenceConfig, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


