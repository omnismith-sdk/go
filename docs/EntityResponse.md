# EntityResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Unique entity identifier (UUIDv7) | [optional] 
**TemplateId** | Pointer to **string** | UUID of the template schema to which this entity conforms | [optional] 
**TemplateSlug** | Pointer to **NullableString** | Human-readable slug of the template schema | [optional] 
**CreatedAt** | Pointer to **time.Time** | Record creation timestamp in ISO 8601 format | [optional] 
**UpdatedAt** | Pointer to **time.Time** | Last modification timestamp in ISO 8601 format | [optional] 
**AttributeValues** | Pointer to [**EntityResponseAttributeValues**](EntityResponseAttributeValues.md) |  | [optional] 
**ListItemIds** | Pointer to **map[string]string** | Compact mode only: list option ids behind the labels shown in &#x60;attribute_values&#x60;, keyed like &#x60;attribute_values&#x60;. Use these ids when writing the attribute or filtering by it — writes and filters take ids, not labels. Absent when &#x60;verbose&#x3D;true&#x60; (the items carry &#x60;value&#x60;). | [optional] 
**ReferenceEntityIds** | Pointer to **map[string]string** | Compact mode only: referenced entity ids behind the labels shown in &#x60;attribute_values&#x60;, keyed like &#x60;attribute_values&#x60;. Pass one to &#x60;GET /entities/{id}&#x60; to load the referenced record, or use it when writing or filtering the attribute. Absent when &#x60;verbose&#x3D;true&#x60;. | [optional] 
**FileIds** | Pointer to **map[string]string** | Compact mode only: file attachment ids behind the filenames shown in &#x60;attribute_values&#x60;, keyed like &#x60;attribute_values&#x60;. Absent when &#x60;verbose&#x3D;true&#x60;. | [optional] 

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

`func (o *EntityResponse) GetAttributeValues() EntityResponseAttributeValues`

GetAttributeValues returns the AttributeValues field if non-nil, zero value otherwise.

### GetAttributeValuesOk

`func (o *EntityResponse) GetAttributeValuesOk() (*EntityResponseAttributeValues, bool)`

GetAttributeValuesOk returns a tuple with the AttributeValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeValues

`func (o *EntityResponse) SetAttributeValues(v EntityResponseAttributeValues)`

SetAttributeValues sets AttributeValues field to given value.

### HasAttributeValues

`func (o *EntityResponse) HasAttributeValues() bool`

HasAttributeValues returns a boolean if a field has been set.

### GetListItemIds

`func (o *EntityResponse) GetListItemIds() map[string]string`

GetListItemIds returns the ListItemIds field if non-nil, zero value otherwise.

### GetListItemIdsOk

`func (o *EntityResponse) GetListItemIdsOk() (*map[string]string, bool)`

GetListItemIdsOk returns a tuple with the ListItemIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListItemIds

`func (o *EntityResponse) SetListItemIds(v map[string]string)`

SetListItemIds sets ListItemIds field to given value.

### HasListItemIds

`func (o *EntityResponse) HasListItemIds() bool`

HasListItemIds returns a boolean if a field has been set.

### GetReferenceEntityIds

`func (o *EntityResponse) GetReferenceEntityIds() map[string]string`

GetReferenceEntityIds returns the ReferenceEntityIds field if non-nil, zero value otherwise.

### GetReferenceEntityIdsOk

`func (o *EntityResponse) GetReferenceEntityIdsOk() (*map[string]string, bool)`

GetReferenceEntityIdsOk returns a tuple with the ReferenceEntityIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferenceEntityIds

`func (o *EntityResponse) SetReferenceEntityIds(v map[string]string)`

SetReferenceEntityIds sets ReferenceEntityIds field to given value.

### HasReferenceEntityIds

`func (o *EntityResponse) HasReferenceEntityIds() bool`

HasReferenceEntityIds returns a boolean if a field has been set.

### GetFileIds

`func (o *EntityResponse) GetFileIds() map[string]string`

GetFileIds returns the FileIds field if non-nil, zero value otherwise.

### GetFileIdsOk

`func (o *EntityResponse) GetFileIdsOk() (*map[string]string, bool)`

GetFileIdsOk returns a tuple with the FileIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFileIds

`func (o *EntityResponse) SetFileIds(v map[string]string)`

SetFileIds sets FileIds field to given value.

### HasFileIds

`func (o *EntityResponse) HasFileIds() bool`

HasFileIds returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


