# TemplateAttributeOverviewResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Attribute UUID | 
**Slug** | Pointer to **NullableString** | Attribute slug identifier | [optional] 
**DefaultValue** | Pointer to **NullableString** | Per-template default value for newly created entities | [optional] 

## Methods

### NewTemplateAttributeOverviewResponse

`func NewTemplateAttributeOverviewResponse(id string, ) *TemplateAttributeOverviewResponse`

NewTemplateAttributeOverviewResponse instantiates a new TemplateAttributeOverviewResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTemplateAttributeOverviewResponseWithDefaults

`func NewTemplateAttributeOverviewResponseWithDefaults() *TemplateAttributeOverviewResponse`

NewTemplateAttributeOverviewResponseWithDefaults instantiates a new TemplateAttributeOverviewResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *TemplateAttributeOverviewResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *TemplateAttributeOverviewResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *TemplateAttributeOverviewResponse) SetId(v string)`

SetId sets Id field to given value.


### GetSlug

`func (o *TemplateAttributeOverviewResponse) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *TemplateAttributeOverviewResponse) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *TemplateAttributeOverviewResponse) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *TemplateAttributeOverviewResponse) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### SetSlugNil

`func (o *TemplateAttributeOverviewResponse) SetSlugNil(b bool)`

 SetSlugNil sets the value for Slug to be an explicit nil

### UnsetSlug
`func (o *TemplateAttributeOverviewResponse) UnsetSlug()`

UnsetSlug ensures that no value is present for Slug, not even an explicit nil
### GetDefaultValue

`func (o *TemplateAttributeOverviewResponse) GetDefaultValue() string`

GetDefaultValue returns the DefaultValue field if non-nil, zero value otherwise.

### GetDefaultValueOk

`func (o *TemplateAttributeOverviewResponse) GetDefaultValueOk() (*string, bool)`

GetDefaultValueOk returns a tuple with the DefaultValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultValue

`func (o *TemplateAttributeOverviewResponse) SetDefaultValue(v string)`

SetDefaultValue sets DefaultValue field to given value.

### HasDefaultValue

`func (o *TemplateAttributeOverviewResponse) HasDefaultValue() bool`

HasDefaultValue returns a boolean if a field has been set.

### SetDefaultValueNil

`func (o *TemplateAttributeOverviewResponse) SetDefaultValueNil(b bool)`

 SetDefaultValueNil sets the value for DefaultValue to be an explicit nil

### UnsetDefaultValue
`func (o *TemplateAttributeOverviewResponse) UnsetDefaultValue()`

UnsetDefaultValue ensures that no value is present for DefaultValue, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


