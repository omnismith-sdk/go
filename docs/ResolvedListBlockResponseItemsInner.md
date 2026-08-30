# ResolvedListBlockResponseItemsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EntityId** | Pointer to **string** | Entity unique identifier | [optional] 
**CreatedAt** | Pointer to **time.Time** | ISO 8601 creation timestamp | [optional] 
**UpdatedAt** | Pointer to **time.Time** | ISO 8601 last update timestamp | [optional] 
**Attributes** | Pointer to **map[string]interface{}** | Key-value map of resolved entity attributes | [optional] 

## Methods

### NewResolvedListBlockResponseItemsInner

`func NewResolvedListBlockResponseItemsInner() *ResolvedListBlockResponseItemsInner`

NewResolvedListBlockResponseItemsInner instantiates a new ResolvedListBlockResponseItemsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResolvedListBlockResponseItemsInnerWithDefaults

`func NewResolvedListBlockResponseItemsInnerWithDefaults() *ResolvedListBlockResponseItemsInner`

NewResolvedListBlockResponseItemsInnerWithDefaults instantiates a new ResolvedListBlockResponseItemsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEntityId

`func (o *ResolvedListBlockResponseItemsInner) GetEntityId() string`

GetEntityId returns the EntityId field if non-nil, zero value otherwise.

### GetEntityIdOk

`func (o *ResolvedListBlockResponseItemsInner) GetEntityIdOk() (*string, bool)`

GetEntityIdOk returns a tuple with the EntityId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityId

`func (o *ResolvedListBlockResponseItemsInner) SetEntityId(v string)`

SetEntityId sets EntityId field to given value.

### HasEntityId

`func (o *ResolvedListBlockResponseItemsInner) HasEntityId() bool`

HasEntityId returns a boolean if a field has been set.

### GetCreatedAt

`func (o *ResolvedListBlockResponseItemsInner) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *ResolvedListBlockResponseItemsInner) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *ResolvedListBlockResponseItemsInner) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *ResolvedListBlockResponseItemsInner) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *ResolvedListBlockResponseItemsInner) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *ResolvedListBlockResponseItemsInner) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *ResolvedListBlockResponseItemsInner) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *ResolvedListBlockResponseItemsInner) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.

### GetAttributes

`func (o *ResolvedListBlockResponseItemsInner) GetAttributes() map[string]interface{}`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *ResolvedListBlockResponseItemsInner) GetAttributesOk() (*map[string]interface{}, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *ResolvedListBlockResponseItemsInner) SetAttributes(v map[string]interface{})`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *ResolvedListBlockResponseItemsInner) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


