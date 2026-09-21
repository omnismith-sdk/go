# EntityActionFieldOverviewResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | **string** | Attribute UUID to set | 
**AttributeSlug** | Pointer to **NullableString** | Attribute slug identifier | [optional] 
**Required** | **bool** | Whether the field must be supplied | 
**Hint** | Pointer to **NullableString** | Guidance text for the operator | [optional] 

## Methods

### NewEntityActionFieldOverviewResponse

`func NewEntityActionFieldOverviewResponse(attributeId string, required bool, ) *EntityActionFieldOverviewResponse`

NewEntityActionFieldOverviewResponse instantiates a new EntityActionFieldOverviewResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityActionFieldOverviewResponseWithDefaults

`func NewEntityActionFieldOverviewResponseWithDefaults() *EntityActionFieldOverviewResponse`

NewEntityActionFieldOverviewResponseWithDefaults instantiates a new EntityActionFieldOverviewResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeId

`func (o *EntityActionFieldOverviewResponse) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *EntityActionFieldOverviewResponse) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *EntityActionFieldOverviewResponse) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.


### GetAttributeSlug

`func (o *EntityActionFieldOverviewResponse) GetAttributeSlug() string`

GetAttributeSlug returns the AttributeSlug field if non-nil, zero value otherwise.

### GetAttributeSlugOk

`func (o *EntityActionFieldOverviewResponse) GetAttributeSlugOk() (*string, bool)`

GetAttributeSlugOk returns a tuple with the AttributeSlug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeSlug

`func (o *EntityActionFieldOverviewResponse) SetAttributeSlug(v string)`

SetAttributeSlug sets AttributeSlug field to given value.

### HasAttributeSlug

`func (o *EntityActionFieldOverviewResponse) HasAttributeSlug() bool`

HasAttributeSlug returns a boolean if a field has been set.

### SetAttributeSlugNil

`func (o *EntityActionFieldOverviewResponse) SetAttributeSlugNil(b bool)`

 SetAttributeSlugNil sets the value for AttributeSlug to be an explicit nil

### UnsetAttributeSlug
`func (o *EntityActionFieldOverviewResponse) UnsetAttributeSlug()`

UnsetAttributeSlug ensures that no value is present for AttributeSlug, not even an explicit nil
### GetRequired

`func (o *EntityActionFieldOverviewResponse) GetRequired() bool`

GetRequired returns the Required field if non-nil, zero value otherwise.

### GetRequiredOk

`func (o *EntityActionFieldOverviewResponse) GetRequiredOk() (*bool, bool)`

GetRequiredOk returns a tuple with the Required field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequired

`func (o *EntityActionFieldOverviewResponse) SetRequired(v bool)`

SetRequired sets Required field to given value.


### GetHint

`func (o *EntityActionFieldOverviewResponse) GetHint() string`

GetHint returns the Hint field if non-nil, zero value otherwise.

### GetHintOk

`func (o *EntityActionFieldOverviewResponse) GetHintOk() (*string, bool)`

GetHintOk returns a tuple with the Hint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHint

`func (o *EntityActionFieldOverviewResponse) SetHint(v string)`

SetHint sets Hint field to given value.

### HasHint

`func (o *EntityActionFieldOverviewResponse) HasHint() bool`

HasHint returns a boolean if a field has been set.

### SetHintNil

`func (o *EntityActionFieldOverviewResponse) SetHintNil(b bool)`

 SetHintNil sets the value for Hint to be an explicit nil

### UnsetHint
`func (o *EntityActionFieldOverviewResponse) UnsetHint()`

UnsetHint ensures that no value is present for Hint, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


