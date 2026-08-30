# EntityAttributeValue

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Value** | Pointer to **string** | Raw serialized attribute value (string, numeric string, ISO date, or UUID) | [optional] 
**CustomValue** | Pointer to **NullableString** | Resolved display label or custom representation (for list options, reference entities, or formatted values) | [optional] 
**ReferenceEntityId** | Pointer to **NullableString** | Target entity UUID when the attribute kind is reference | [optional] 
**AttributeId** | Pointer to **NullableString** | Canonical attribute definition UUID | [optional] 
**AttributeSlug** | Pointer to **NullableString** | Human-readable attribute slug identifier | [optional] 

## Methods

### NewEntityAttributeValue

`func NewEntityAttributeValue() *EntityAttributeValue`

NewEntityAttributeValue instantiates a new EntityAttributeValue object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityAttributeValueWithDefaults

`func NewEntityAttributeValueWithDefaults() *EntityAttributeValue`

NewEntityAttributeValueWithDefaults instantiates a new EntityAttributeValue object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValue

`func (o *EntityAttributeValue) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *EntityAttributeValue) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *EntityAttributeValue) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *EntityAttributeValue) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetCustomValue

`func (o *EntityAttributeValue) GetCustomValue() string`

GetCustomValue returns the CustomValue field if non-nil, zero value otherwise.

### GetCustomValueOk

`func (o *EntityAttributeValue) GetCustomValueOk() (*string, bool)`

GetCustomValueOk returns a tuple with the CustomValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCustomValue

`func (o *EntityAttributeValue) SetCustomValue(v string)`

SetCustomValue sets CustomValue field to given value.

### HasCustomValue

`func (o *EntityAttributeValue) HasCustomValue() bool`

HasCustomValue returns a boolean if a field has been set.

### SetCustomValueNil

`func (o *EntityAttributeValue) SetCustomValueNil(b bool)`

 SetCustomValueNil sets the value for CustomValue to be an explicit nil

### UnsetCustomValue
`func (o *EntityAttributeValue) UnsetCustomValue()`

UnsetCustomValue ensures that no value is present for CustomValue, not even an explicit nil
### GetReferenceEntityId

`func (o *EntityAttributeValue) GetReferenceEntityId() string`

GetReferenceEntityId returns the ReferenceEntityId field if non-nil, zero value otherwise.

### GetReferenceEntityIdOk

`func (o *EntityAttributeValue) GetReferenceEntityIdOk() (*string, bool)`

GetReferenceEntityIdOk returns a tuple with the ReferenceEntityId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferenceEntityId

`func (o *EntityAttributeValue) SetReferenceEntityId(v string)`

SetReferenceEntityId sets ReferenceEntityId field to given value.

### HasReferenceEntityId

`func (o *EntityAttributeValue) HasReferenceEntityId() bool`

HasReferenceEntityId returns a boolean if a field has been set.

### SetReferenceEntityIdNil

`func (o *EntityAttributeValue) SetReferenceEntityIdNil(b bool)`

 SetReferenceEntityIdNil sets the value for ReferenceEntityId to be an explicit nil

### UnsetReferenceEntityId
`func (o *EntityAttributeValue) UnsetReferenceEntityId()`

UnsetReferenceEntityId ensures that no value is present for ReferenceEntityId, not even an explicit nil
### GetAttributeId

`func (o *EntityAttributeValue) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *EntityAttributeValue) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *EntityAttributeValue) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.

### HasAttributeId

`func (o *EntityAttributeValue) HasAttributeId() bool`

HasAttributeId returns a boolean if a field has been set.

### SetAttributeIdNil

`func (o *EntityAttributeValue) SetAttributeIdNil(b bool)`

 SetAttributeIdNil sets the value for AttributeId to be an explicit nil

### UnsetAttributeId
`func (o *EntityAttributeValue) UnsetAttributeId()`

UnsetAttributeId ensures that no value is present for AttributeId, not even an explicit nil
### GetAttributeSlug

`func (o *EntityAttributeValue) GetAttributeSlug() string`

GetAttributeSlug returns the AttributeSlug field if non-nil, zero value otherwise.

### GetAttributeSlugOk

`func (o *EntityAttributeValue) GetAttributeSlugOk() (*string, bool)`

GetAttributeSlugOk returns a tuple with the AttributeSlug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeSlug

`func (o *EntityAttributeValue) SetAttributeSlug(v string)`

SetAttributeSlug sets AttributeSlug field to given value.

### HasAttributeSlug

`func (o *EntityAttributeValue) HasAttributeSlug() bool`

HasAttributeSlug returns a boolean if a field has been set.

### SetAttributeSlugNil

`func (o *EntityAttributeValue) SetAttributeSlugNil(b bool)`

 SetAttributeSlugNil sets the value for AttributeSlug to be an explicit nil

### UnsetAttributeSlug
`func (o *EntityAttributeValue) UnsetAttributeSlug()`

UnsetAttributeSlug ensures that no value is present for AttributeSlug, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


