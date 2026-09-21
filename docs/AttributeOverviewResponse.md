# AttributeOverviewResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Attribute UUID | 
**Slug** | Pointer to **NullableString** | Unique slug identifier within the project | [optional] 
**Name** | **string** | Human-readable attribute name | 
**Type** | **string** | Semantic data kind: string, number, boolean, datetime, date, file, image, markdown, list, reference, metric | 
**Description** | Pointer to **NullableString** | Attribute description | [optional] 
**Options** | Pointer to [**[]ListOptionOverviewResponse**](ListOptionOverviewResponse.md) | Selectable choice options for list-type attributes (null for other types) | [optional] 
**Reference** | Pointer to [**NullableReferenceOverviewResponse**](ReferenceOverviewResponse.md) |  | [optional] 

## Methods

### NewAttributeOverviewResponse

`func NewAttributeOverviewResponse(id string, name string, type_ string, ) *AttributeOverviewResponse`

NewAttributeOverviewResponse instantiates a new AttributeOverviewResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAttributeOverviewResponseWithDefaults

`func NewAttributeOverviewResponseWithDefaults() *AttributeOverviewResponse`

NewAttributeOverviewResponseWithDefaults instantiates a new AttributeOverviewResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *AttributeOverviewResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *AttributeOverviewResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *AttributeOverviewResponse) SetId(v string)`

SetId sets Id field to given value.


### GetSlug

`func (o *AttributeOverviewResponse) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *AttributeOverviewResponse) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *AttributeOverviewResponse) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *AttributeOverviewResponse) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### SetSlugNil

`func (o *AttributeOverviewResponse) SetSlugNil(b bool)`

 SetSlugNil sets the value for Slug to be an explicit nil

### UnsetSlug
`func (o *AttributeOverviewResponse) UnsetSlug()`

UnsetSlug ensures that no value is present for Slug, not even an explicit nil
### GetName

`func (o *AttributeOverviewResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *AttributeOverviewResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *AttributeOverviewResponse) SetName(v string)`

SetName sets Name field to given value.


### GetType

`func (o *AttributeOverviewResponse) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *AttributeOverviewResponse) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *AttributeOverviewResponse) SetType(v string)`

SetType sets Type field to given value.


### GetDescription

`func (o *AttributeOverviewResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *AttributeOverviewResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *AttributeOverviewResponse) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *AttributeOverviewResponse) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *AttributeOverviewResponse) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *AttributeOverviewResponse) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetOptions

`func (o *AttributeOverviewResponse) GetOptions() []ListOptionOverviewResponse`

GetOptions returns the Options field if non-nil, zero value otherwise.

### GetOptionsOk

`func (o *AttributeOverviewResponse) GetOptionsOk() (*[]ListOptionOverviewResponse, bool)`

GetOptionsOk returns a tuple with the Options field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOptions

`func (o *AttributeOverviewResponse) SetOptions(v []ListOptionOverviewResponse)`

SetOptions sets Options field to given value.

### HasOptions

`func (o *AttributeOverviewResponse) HasOptions() bool`

HasOptions returns a boolean if a field has been set.

### SetOptionsNil

`func (o *AttributeOverviewResponse) SetOptionsNil(b bool)`

 SetOptionsNil sets the value for Options to be an explicit nil

### UnsetOptions
`func (o *AttributeOverviewResponse) UnsetOptions()`

UnsetOptions ensures that no value is present for Options, not even an explicit nil
### GetReference

`func (o *AttributeOverviewResponse) GetReference() ReferenceOverviewResponse`

GetReference returns the Reference field if non-nil, zero value otherwise.

### GetReferenceOk

`func (o *AttributeOverviewResponse) GetReferenceOk() (*ReferenceOverviewResponse, bool)`

GetReferenceOk returns a tuple with the Reference field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReference

`func (o *AttributeOverviewResponse) SetReference(v ReferenceOverviewResponse)`

SetReference sets Reference field to given value.

### HasReference

`func (o *AttributeOverviewResponse) HasReference() bool`

HasReference returns a boolean if a field has been set.

### SetReferenceNil

`func (o *AttributeOverviewResponse) SetReferenceNil(b bool)`

 SetReferenceNil sets the value for Reference to be an explicit nil

### UnsetReference
`func (o *AttributeOverviewResponse) UnsetReference()`

UnsetReference ensures that no value is present for Reference, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


