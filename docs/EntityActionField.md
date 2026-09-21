# EntityActionField

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | **string** | Attribute UUID to ask for. Must belong to the template and must not be a metric or a preset of the same action. | 
**Required** | Pointer to **bool** | Whether execution refuses an empty value for this field (422 keyed by &#x60;attributes.&lt;slug&gt;&#x60;). Defaults to false. | [optional] [default to false]
**Hint** | Pointer to **NullableString** | Short guidance shown next to the field | [optional] 

## Methods

### NewEntityActionField

`func NewEntityActionField(attributeId string, ) *EntityActionField`

NewEntityActionField instantiates a new EntityActionField object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityActionFieldWithDefaults

`func NewEntityActionFieldWithDefaults() *EntityActionField`

NewEntityActionFieldWithDefaults instantiates a new EntityActionField object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeId

`func (o *EntityActionField) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *EntityActionField) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *EntityActionField) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.


### GetRequired

`func (o *EntityActionField) GetRequired() bool`

GetRequired returns the Required field if non-nil, zero value otherwise.

### GetRequiredOk

`func (o *EntityActionField) GetRequiredOk() (*bool, bool)`

GetRequiredOk returns a tuple with the Required field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequired

`func (o *EntityActionField) SetRequired(v bool)`

SetRequired sets Required field to given value.

### HasRequired

`func (o *EntityActionField) HasRequired() bool`

HasRequired returns a boolean if a field has been set.

### GetHint

`func (o *EntityActionField) GetHint() string`

GetHint returns the Hint field if non-nil, zero value otherwise.

### GetHintOk

`func (o *EntityActionField) GetHintOk() (*string, bool)`

GetHintOk returns a tuple with the Hint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHint

`func (o *EntityActionField) SetHint(v string)`

SetHint sets Hint field to given value.

### HasHint

`func (o *EntityActionField) HasHint() bool`

HasHint returns a boolean if a field has been set.

### SetHintNil

`func (o *EntityActionField) SetHintNil(b bool)`

 SetHintNil sets the value for Hint to be an explicit nil

### UnsetHint
`func (o *EntityActionField) UnsetHint()`

UnsetHint ensures that no value is present for Hint, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


