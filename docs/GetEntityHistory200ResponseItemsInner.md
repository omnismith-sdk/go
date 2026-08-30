# GetEntityHistory200ResponseItemsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CreatedAt** | Pointer to **time.Time** | Mutation timestamp in ISO 8601 format | [optional] 
**AttributeId** | Pointer to **string** | Mutated attribute UUID | [optional] 
**OldValue** | Pointer to **NullableString** | Previous serialized attribute value | [optional] 
**Value** | Pointer to **string** | New serialized attribute value | [optional] 
**EntityId** | Pointer to **string** | Target entity UUID | [optional] 
**AuthorEmail** | Pointer to **NullableString** | Actor email who performed the change | [optional] 

## Methods

### NewGetEntityHistory200ResponseItemsInner

`func NewGetEntityHistory200ResponseItemsInner() *GetEntityHistory200ResponseItemsInner`

NewGetEntityHistory200ResponseItemsInner instantiates a new GetEntityHistory200ResponseItemsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetEntityHistory200ResponseItemsInnerWithDefaults

`func NewGetEntityHistory200ResponseItemsInnerWithDefaults() *GetEntityHistory200ResponseItemsInner`

NewGetEntityHistory200ResponseItemsInnerWithDefaults instantiates a new GetEntityHistory200ResponseItemsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCreatedAt

`func (o *GetEntityHistory200ResponseItemsInner) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *GetEntityHistory200ResponseItemsInner) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *GetEntityHistory200ResponseItemsInner) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *GetEntityHistory200ResponseItemsInner) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetAttributeId

`func (o *GetEntityHistory200ResponseItemsInner) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *GetEntityHistory200ResponseItemsInner) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *GetEntityHistory200ResponseItemsInner) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.

### HasAttributeId

`func (o *GetEntityHistory200ResponseItemsInner) HasAttributeId() bool`

HasAttributeId returns a boolean if a field has been set.

### GetOldValue

`func (o *GetEntityHistory200ResponseItemsInner) GetOldValue() string`

GetOldValue returns the OldValue field if non-nil, zero value otherwise.

### GetOldValueOk

`func (o *GetEntityHistory200ResponseItemsInner) GetOldValueOk() (*string, bool)`

GetOldValueOk returns a tuple with the OldValue field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOldValue

`func (o *GetEntityHistory200ResponseItemsInner) SetOldValue(v string)`

SetOldValue sets OldValue field to given value.

### HasOldValue

`func (o *GetEntityHistory200ResponseItemsInner) HasOldValue() bool`

HasOldValue returns a boolean if a field has been set.

### SetOldValueNil

`func (o *GetEntityHistory200ResponseItemsInner) SetOldValueNil(b bool)`

 SetOldValueNil sets the value for OldValue to be an explicit nil

### UnsetOldValue
`func (o *GetEntityHistory200ResponseItemsInner) UnsetOldValue()`

UnsetOldValue ensures that no value is present for OldValue, not even an explicit nil
### GetValue

`func (o *GetEntityHistory200ResponseItemsInner) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *GetEntityHistory200ResponseItemsInner) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *GetEntityHistory200ResponseItemsInner) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *GetEntityHistory200ResponseItemsInner) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetEntityId

`func (o *GetEntityHistory200ResponseItemsInner) GetEntityId() string`

GetEntityId returns the EntityId field if non-nil, zero value otherwise.

### GetEntityIdOk

`func (o *GetEntityHistory200ResponseItemsInner) GetEntityIdOk() (*string, bool)`

GetEntityIdOk returns a tuple with the EntityId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityId

`func (o *GetEntityHistory200ResponseItemsInner) SetEntityId(v string)`

SetEntityId sets EntityId field to given value.

### HasEntityId

`func (o *GetEntityHistory200ResponseItemsInner) HasEntityId() bool`

HasEntityId returns a boolean if a field has been set.

### GetAuthorEmail

`func (o *GetEntityHistory200ResponseItemsInner) GetAuthorEmail() string`

GetAuthorEmail returns the AuthorEmail field if non-nil, zero value otherwise.

### GetAuthorEmailOk

`func (o *GetEntityHistory200ResponseItemsInner) GetAuthorEmailOk() (*string, bool)`

GetAuthorEmailOk returns a tuple with the AuthorEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthorEmail

`func (o *GetEntityHistory200ResponseItemsInner) SetAuthorEmail(v string)`

SetAuthorEmail sets AuthorEmail field to given value.

### HasAuthorEmail

`func (o *GetEntityHistory200ResponseItemsInner) HasAuthorEmail() bool`

HasAuthorEmail returns a boolean if a field has been set.

### SetAuthorEmailNil

`func (o *GetEntityHistory200ResponseItemsInner) SetAuthorEmailNil(b bool)`

 SetAuthorEmailNil sets the value for AuthorEmail to be an explicit nil

### UnsetAuthorEmail
`func (o *GetEntityHistory200ResponseItemsInner) UnsetAuthorEmail()`

UnsetAuthorEmail ensures that no value is present for AuthorEmail, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


