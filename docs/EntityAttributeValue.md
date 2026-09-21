# EntityAttributeValue

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Canonical attribute definition UUID | 
**Slug** | **NullableString** | Human-readable attribute slug identifier; null when the attribute has no slug | 
**Value** | **string** | Raw serialized attribute value (string, numeric string, ISO date, or UUID); empty string when unset | 
**CustomValue** | **NullableString** | Resolved display label (list option label, referenced entity display value, original filename) or the raw value for scalars | 
**ReferenceEntityId** | **NullableString** | Target entity UUID when the attribute kind is reference | 

## Methods

### NewEntityAttributeValue

`func NewEntityAttributeValue(id string, slug NullableString, value string, customValue NullableString, referenceEntityId NullableString, ) *EntityAttributeValue`

NewEntityAttributeValue instantiates a new EntityAttributeValue object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityAttributeValueWithDefaults

`func NewEntityAttributeValueWithDefaults() *EntityAttributeValue`

NewEntityAttributeValueWithDefaults instantiates a new EntityAttributeValue object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *EntityAttributeValue) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *EntityAttributeValue) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *EntityAttributeValue) SetId(v string)`

SetId sets Id field to given value.


### GetSlug

`func (o *EntityAttributeValue) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *EntityAttributeValue) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *EntityAttributeValue) SetSlug(v string)`

SetSlug sets Slug field to given value.


### SetSlugNil

`func (o *EntityAttributeValue) SetSlugNil(b bool)`

 SetSlugNil sets the value for Slug to be an explicit nil

### UnsetSlug
`func (o *EntityAttributeValue) UnsetSlug()`

UnsetSlug ensures that no value is present for Slug, not even an explicit nil
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


### SetReferenceEntityIdNil

`func (o *EntityAttributeValue) SetReferenceEntityIdNil(b bool)`

 SetReferenceEntityIdNil sets the value for ReferenceEntityId to be an explicit nil

### UnsetReferenceEntityId
`func (o *EntityAttributeValue) UnsetReferenceEntityId()`

UnsetReferenceEntityId ensures that no value is present for ReferenceEntityId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


