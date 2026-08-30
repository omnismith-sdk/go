# CreateEntityRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | Pointer to **NullableString** | Template UUID to instantiate (mutually exclusive with template_slug) | [optional] 
**AttributeValues** | Pointer to [**[]CreateEntityRequestAttributeValuesInner**](CreateEntityRequestAttributeValuesInner.md) | Initial attribute values for dimensions, lists, references, and initial metrics | [optional] 
**Id** | Pointer to **NullableString** | Optional client-assigned UUIDv7 identifier for the entity record. If omitted, a UUIDv7 is automatically generated. | [optional] 
**TemplateSlug** | Pointer to **NullableString** | Template slug identifier to instantiate (mutually exclusive with template_id) | [optional] 

## Methods

### NewCreateEntityRequest

`func NewCreateEntityRequest() *CreateEntityRequest`

NewCreateEntityRequest instantiates a new CreateEntityRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateEntityRequestWithDefaults

`func NewCreateEntityRequestWithDefaults() *CreateEntityRequest`

NewCreateEntityRequestWithDefaults instantiates a new CreateEntityRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *CreateEntityRequest) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *CreateEntityRequest) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *CreateEntityRequest) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *CreateEntityRequest) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### SetTemplateIdNil

`func (o *CreateEntityRequest) SetTemplateIdNil(b bool)`

 SetTemplateIdNil sets the value for TemplateId to be an explicit nil

### UnsetTemplateId
`func (o *CreateEntityRequest) UnsetTemplateId()`

UnsetTemplateId ensures that no value is present for TemplateId, not even an explicit nil
### GetAttributeValues

`func (o *CreateEntityRequest) GetAttributeValues() []CreateEntityRequestAttributeValuesInner`

GetAttributeValues returns the AttributeValues field if non-nil, zero value otherwise.

### GetAttributeValuesOk

`func (o *CreateEntityRequest) GetAttributeValuesOk() (*[]CreateEntityRequestAttributeValuesInner, bool)`

GetAttributeValuesOk returns a tuple with the AttributeValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeValues

`func (o *CreateEntityRequest) SetAttributeValues(v []CreateEntityRequestAttributeValuesInner)`

SetAttributeValues sets AttributeValues field to given value.

### HasAttributeValues

`func (o *CreateEntityRequest) HasAttributeValues() bool`

HasAttributeValues returns a boolean if a field has been set.

### GetId

`func (o *CreateEntityRequest) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *CreateEntityRequest) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *CreateEntityRequest) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *CreateEntityRequest) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *CreateEntityRequest) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *CreateEntityRequest) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetTemplateSlug

`func (o *CreateEntityRequest) GetTemplateSlug() string`

GetTemplateSlug returns the TemplateSlug field if non-nil, zero value otherwise.

### GetTemplateSlugOk

`func (o *CreateEntityRequest) GetTemplateSlugOk() (*string, bool)`

GetTemplateSlugOk returns a tuple with the TemplateSlug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateSlug

`func (o *CreateEntityRequest) SetTemplateSlug(v string)`

SetTemplateSlug sets TemplateSlug field to given value.

### HasTemplateSlug

`func (o *CreateEntityRequest) HasTemplateSlug() bool`

HasTemplateSlug returns a boolean if a field has been set.

### SetTemplateSlugNil

`func (o *CreateEntityRequest) SetTemplateSlugNil(b bool)`

 SetTemplateSlugNil sets the value for TemplateSlug to be an explicit nil

### UnsetTemplateSlug
`func (o *CreateEntityRequest) UnsetTemplateSlug()`

UnsetTemplateSlug ensures that no value is present for TemplateSlug, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


