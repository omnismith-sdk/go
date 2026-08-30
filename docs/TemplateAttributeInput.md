# TemplateAttributeInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | Pointer to **NullableString** | Attribute UUID. Specify either attribute_id or attribute_slug. | [optional] 
**AttributeSlug** | Pointer to **NullableString** | Attribute unique slug. Specify either attribute_id or attribute_slug. | [optional] 
**DefaultValue** | Pointer to **NullableString** | Default value applied to new entities when omitted. For List attributes, must be a valid list item UUID. For Reference attributes, a target entity UUID. For Metric/Number, a numeric string. For Boolean, \&quot;true\&quot; or \&quot;false\&quot;. For Date/Datetime, an ISO timestamp string. For File/Image, defaults are unsupported. Null means no default. | [optional] 

## Methods

### NewTemplateAttributeInput

`func NewTemplateAttributeInput() *TemplateAttributeInput`

NewTemplateAttributeInput instantiates a new TemplateAttributeInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTemplateAttributeInputWithDefaults

`func NewTemplateAttributeInputWithDefaults() *TemplateAttributeInput`

NewTemplateAttributeInputWithDefaults instantiates a new TemplateAttributeInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeId

`func (o *TemplateAttributeInput) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *TemplateAttributeInput) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *TemplateAttributeInput) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.

### HasAttributeId

`func (o *TemplateAttributeInput) HasAttributeId() bool`

HasAttributeId returns a boolean if a field has been set.

### SetAttributeIdNil

`func (o *TemplateAttributeInput) SetAttributeIdNil(b bool)`

 SetAttributeIdNil sets the value for AttributeId to be an explicit nil

### UnsetAttributeId
`func (o *TemplateAttributeInput) UnsetAttributeId()`

UnsetAttributeId ensures that no value is present for AttributeId, not even an explicit nil
### GetAttributeSlug

`func (o *TemplateAttributeInput) GetAttributeSlug() string`

GetAttributeSlug returns the AttributeSlug field if non-nil, zero value otherwise.

### GetAttributeSlugOk

`func (o *TemplateAttributeInput) GetAttributeSlugOk() (*string, bool)`

GetAttributeSlugOk returns a tuple with the AttributeSlug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeSlug

`func (o *TemplateAttributeInput) SetAttributeSlug(v string)`

SetAttributeSlug sets AttributeSlug field to given value.

### HasAttributeSlug

`func (o *TemplateAttributeInput) HasAttributeSlug() bool`

HasAttributeSlug returns a boolean if a field has been set.

### SetAttributeSlugNil

`func (o *TemplateAttributeInput) SetAttributeSlugNil(b bool)`

 SetAttributeSlugNil sets the value for AttributeSlug to be an explicit nil

### UnsetAttributeSlug
`func (o *TemplateAttributeInput) UnsetAttributeSlug()`

UnsetAttributeSlug ensures that no value is present for AttributeSlug, not even an explicit nil
### GetDefaultValue

`func (o *TemplateAttributeInput) GetDefaultValue() string`

GetDefaultValue returns the DefaultValue field if non-nil, zero value otherwise.

### GetDefaultValueOk

`func (o *TemplateAttributeInput) GetDefaultValueOk() (*string, bool)`

GetDefaultValueOk returns a tuple with the DefaultValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultValue

`func (o *TemplateAttributeInput) SetDefaultValue(v string)`

SetDefaultValue sets DefaultValue field to given value.

### HasDefaultValue

`func (o *TemplateAttributeInput) HasDefaultValue() bool`

HasDefaultValue returns a boolean if a field has been set.

### SetDefaultValueNil

`func (o *TemplateAttributeInput) SetDefaultValueNil(b bool)`

 SetDefaultValueNil sets the value for DefaultValue to be an explicit nil

### UnsetDefaultValue
`func (o *TemplateAttributeInput) UnsetDefaultValue()`

UnsetDefaultValue ensures that no value is present for DefaultValue, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


