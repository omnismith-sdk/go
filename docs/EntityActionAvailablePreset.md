# EntityActionAvailablePreset

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | **string** |  | 
**Slug** | **NullableString** |  | 
**Name** | **string** |  | 
**Value** | **string** | The stored value: a list item id, an entity id, &#x60;true&#x60;/&#x60;false&#x60;, a number or date as text | 
**DisplayValue** | **string** | The list item label for list attributes, otherwise the value itself | 

## Methods

### NewEntityActionAvailablePreset

`func NewEntityActionAvailablePreset(attributeId string, slug NullableString, name string, value string, displayValue string, ) *EntityActionAvailablePreset`

NewEntityActionAvailablePreset instantiates a new EntityActionAvailablePreset object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityActionAvailablePresetWithDefaults

`func NewEntityActionAvailablePresetWithDefaults() *EntityActionAvailablePreset`

NewEntityActionAvailablePresetWithDefaults instantiates a new EntityActionAvailablePreset object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeId

`func (o *EntityActionAvailablePreset) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *EntityActionAvailablePreset) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *EntityActionAvailablePreset) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.


### GetSlug

`func (o *EntityActionAvailablePreset) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *EntityActionAvailablePreset) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *EntityActionAvailablePreset) SetSlug(v string)`

SetSlug sets Slug field to given value.


### SetSlugNil

`func (o *EntityActionAvailablePreset) SetSlugNil(b bool)`

 SetSlugNil sets the value for Slug to be an explicit nil

### UnsetSlug
`func (o *EntityActionAvailablePreset) UnsetSlug()`

UnsetSlug ensures that no value is present for Slug, not even an explicit nil
### GetName

`func (o *EntityActionAvailablePreset) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *EntityActionAvailablePreset) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *EntityActionAvailablePreset) SetName(v string)`

SetName sets Name field to given value.


### GetValue

`func (o *EntityActionAvailablePreset) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *EntityActionAvailablePreset) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *EntityActionAvailablePreset) SetValue(v string)`

SetValue sets Value field to given value.


### GetDisplayValue

`func (o *EntityActionAvailablePreset) GetDisplayValue() string`

GetDisplayValue returns the DisplayValue field if non-nil, zero value otherwise.

### GetDisplayValueOk

`func (o *EntityActionAvailablePreset) GetDisplayValueOk() (*string, bool)`

GetDisplayValueOk returns a tuple with the DisplayValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisplayValue

`func (o *EntityActionAvailablePreset) SetDisplayValue(v string)`

SetDisplayValue sets DisplayValue field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


