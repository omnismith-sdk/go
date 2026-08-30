# TemplateResponseAttributesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | **string** | Attribute UUID | 
**DefaultValue** | Pointer to **NullableString** | Per-template default value for newly created entities (or null) | [optional] 

## Methods

### NewTemplateResponseAttributesInner

`func NewTemplateResponseAttributesInner(attributeId string, ) *TemplateResponseAttributesInner`

NewTemplateResponseAttributesInner instantiates a new TemplateResponseAttributesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTemplateResponseAttributesInnerWithDefaults

`func NewTemplateResponseAttributesInnerWithDefaults() *TemplateResponseAttributesInner`

NewTemplateResponseAttributesInnerWithDefaults instantiates a new TemplateResponseAttributesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeId

`func (o *TemplateResponseAttributesInner) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *TemplateResponseAttributesInner) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *TemplateResponseAttributesInner) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.


### GetDefaultValue

`func (o *TemplateResponseAttributesInner) GetDefaultValue() string`

GetDefaultValue returns the DefaultValue field if non-nil, zero value otherwise.

### GetDefaultValueOk

`func (o *TemplateResponseAttributesInner) GetDefaultValueOk() (*string, bool)`

GetDefaultValueOk returns a tuple with the DefaultValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultValue

`func (o *TemplateResponseAttributesInner) SetDefaultValue(v string)`

SetDefaultValue sets DefaultValue field to given value.

### HasDefaultValue

`func (o *TemplateResponseAttributesInner) HasDefaultValue() bool`

HasDefaultValue returns a boolean if a field has been set.

### SetDefaultValueNil

`func (o *TemplateResponseAttributesInner) SetDefaultValueNil(b bool)`

 SetDefaultValueNil sets the value for DefaultValue to be an explicit nil

### UnsetDefaultValue
`func (o *TemplateResponseAttributesInner) UnsetDefaultValue()`

UnsetDefaultValue ensures that no value is present for DefaultValue, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


