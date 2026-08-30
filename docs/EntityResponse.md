# EntityResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Unique entity identifier (UUIDv7) | [optional] 
**TemplateId** | Pointer to **string** | UUID of the template schema to which this entity conforms | [optional] 
**TemplateSlug** | Pointer to **NullableString** | Human-readable slug of the template schema | [optional] 
**CreatedAt** | Pointer to **time.Time** | Record creation timestamp in ISO 8601 format | [optional] 
**UpdatedAt** | Pointer to **time.Time** | Last modification timestamp in ISO 8601 format | [optional] 
**AttributeValues** | Pointer to [**map[string]EntityAttributeValue**](EntityAttributeValue.md) | Dictionary of attribute values keyed by attribute UUID or attribute slug (controlled by the attribute_key query parameter) | [optional] 

## Methods

### NewEntityResponse

`func NewEntityResponse() *EntityResponse`

NewEntityResponse instantiates a new EntityResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityResponseWithDefaults

`func NewEntityResponseWithDefaults() *EntityResponse`

NewEntityResponseWithDefaults instantiates a new EntityResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *EntityResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *EntityResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *EntityResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *EntityResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetTemplateId

`func (o *EntityResponse) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *EntityResponse) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *EntityResponse) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *EntityResponse) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetTemplateSlug

`func (o *EntityResponse) GetTemplateSlug() string`

GetTemplateSlug returns the TemplateSlug field if non-nil, zero value otherwise.

### GetTemplateSlugOk

`func (o *EntityResponse) GetTemplateSlugOk() (*string, bool)`

GetTemplateSlugOk returns a tuple with the TemplateSlug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateSlug

`func (o *EntityResponse) SetTemplateSlug(v string)`

SetTemplateSlug sets TemplateSlug field to given value.

### HasTemplateSlug

`func (o *EntityResponse) HasTemplateSlug() bool`

HasTemplateSlug returns a boolean if a field has been set.

### SetTemplateSlugNil

`func (o *EntityResponse) SetTemplateSlugNil(b bool)`

 SetTemplateSlugNil sets the value for TemplateSlug to be an explicit nil

### UnsetTemplateSlug
`func (o *EntityResponse) UnsetTemplateSlug()`

UnsetTemplateSlug ensures that no value is present for TemplateSlug, not even an explicit nil
### GetCreatedAt

`func (o *EntityResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *EntityResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *EntityResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *EntityResponse) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *EntityResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *EntityResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *EntityResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *EntityResponse) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.

### GetAttributeValues

`func (o *EntityResponse) GetAttributeValues() map[string]EntityAttributeValue`

GetAttributeValues returns the AttributeValues field if non-nil, zero value otherwise.

### GetAttributeValuesOk

`func (o *EntityResponse) GetAttributeValuesOk() (*map[string]EntityAttributeValue, bool)`

GetAttributeValuesOk returns a tuple with the AttributeValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeValues

`func (o *EntityResponse) SetAttributeValues(v map[string]EntityAttributeValue)`

SetAttributeValues sets AttributeValues field to given value.

### HasAttributeValues

`func (o *EntityResponse) HasAttributeValues() bool`

HasAttributeValues returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


