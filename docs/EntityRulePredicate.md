# EntityRulePredicate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | **string** | Attribute UUID the predicate reads | 
**Operator** | **string** | Comparison operator. &#x60;gt&#x60;/&#x60;gte&#x60;/&#x60;lt&#x60;/&#x60;lte&#x60; apply to number and date attributes, &#x60;contains&#x60;/&#x60;not_contains&#x60; to text, &#x60;in&#x60; to list attributes (value is a list of list item UUIDs), &#x60;eq&#x60;/&#x60;neq&#x60;/&#x60;is_empty&#x60;/&#x60;is_not_empty&#x60; to every non-metric attribute. | 
**Value** | Pointer to [**NullableEntityRulePredicateValue**](EntityRulePredicateValue.md) |  | [optional] 

## Methods

### NewEntityRulePredicate

`func NewEntityRulePredicate(attributeId string, operator string, ) *EntityRulePredicate`

NewEntityRulePredicate instantiates a new EntityRulePredicate object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityRulePredicateWithDefaults

`func NewEntityRulePredicateWithDefaults() *EntityRulePredicate`

NewEntityRulePredicateWithDefaults instantiates a new EntityRulePredicate object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeId

`func (o *EntityRulePredicate) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *EntityRulePredicate) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *EntityRulePredicate) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.


### GetOperator

`func (o *EntityRulePredicate) GetOperator() string`

GetOperator returns the Operator field if non-nil, zero value otherwise.

### GetOperatorOk

`func (o *EntityRulePredicate) GetOperatorOk() (*string, bool)`

GetOperatorOk returns a tuple with the Operator field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperator

`func (o *EntityRulePredicate) SetOperator(v string)`

SetOperator sets Operator field to given value.


### GetValue

`func (o *EntityRulePredicate) GetValue() EntityRulePredicateValue`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *EntityRulePredicate) GetValueOk() (*EntityRulePredicateValue, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *EntityRulePredicate) SetValue(v EntityRulePredicateValue)`

SetValue sets Value field to given value.

### HasValue

`func (o *EntityRulePredicate) HasValue() bool`

HasValue returns a boolean if a field has been set.

### SetValueNil

`func (o *EntityRulePredicate) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *EntityRulePredicate) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


