# EntityActionPreset

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | **string** | Attribute UUID to set. Must belong to the template and must not be a metric or a field of the same action. | 
**Value** | **string** | Value serialized as a string: a list item UUID for list attributes, an entity UUID for references, &#x60;true&#x60;/&#x60;false&#x60; for booleans, a number or date as text. | 

## Methods

### NewEntityActionPreset

`func NewEntityActionPreset(attributeId string, value string, ) *EntityActionPreset`

NewEntityActionPreset instantiates a new EntityActionPreset object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityActionPresetWithDefaults

`func NewEntityActionPresetWithDefaults() *EntityActionPreset`

NewEntityActionPresetWithDefaults instantiates a new EntityActionPreset object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeId

`func (o *EntityActionPreset) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *EntityActionPreset) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *EntityActionPreset) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.


### GetValue

`func (o *EntityActionPreset) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *EntityActionPreset) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *EntityActionPreset) SetValue(v string)`

SetValue sets Value field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


