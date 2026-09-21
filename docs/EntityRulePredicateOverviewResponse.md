# EntityRulePredicateOverviewResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | **string** | Attribute UUID | 
**AttributeSlug** | Pointer to **NullableString** | Attribute slug identifier | [optional] 
**Operator** | **string** | Comparison operator: eq, neq, gt, gte, lt, lte, contains, not_contains, in, is_empty, is_not_empty | 
**Value** | Pointer to [**NullableEntityRulePredicateOverviewResponseValue**](EntityRulePredicateOverviewResponseValue.md) |  | [optional] 

## Methods

### NewEntityRulePredicateOverviewResponse

`func NewEntityRulePredicateOverviewResponse(attributeId string, operator string, ) *EntityRulePredicateOverviewResponse`

NewEntityRulePredicateOverviewResponse instantiates a new EntityRulePredicateOverviewResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityRulePredicateOverviewResponseWithDefaults

`func NewEntityRulePredicateOverviewResponseWithDefaults() *EntityRulePredicateOverviewResponse`

NewEntityRulePredicateOverviewResponseWithDefaults instantiates a new EntityRulePredicateOverviewResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeId

`func (o *EntityRulePredicateOverviewResponse) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *EntityRulePredicateOverviewResponse) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *EntityRulePredicateOverviewResponse) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.


### GetAttributeSlug

`func (o *EntityRulePredicateOverviewResponse) GetAttributeSlug() string`

GetAttributeSlug returns the AttributeSlug field if non-nil, zero value otherwise.

### GetAttributeSlugOk

`func (o *EntityRulePredicateOverviewResponse) GetAttributeSlugOk() (*string, bool)`

GetAttributeSlugOk returns a tuple with the AttributeSlug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeSlug

`func (o *EntityRulePredicateOverviewResponse) SetAttributeSlug(v string)`

SetAttributeSlug sets AttributeSlug field to given value.

### HasAttributeSlug

`func (o *EntityRulePredicateOverviewResponse) HasAttributeSlug() bool`

HasAttributeSlug returns a boolean if a field has been set.

### SetAttributeSlugNil

`func (o *EntityRulePredicateOverviewResponse) SetAttributeSlugNil(b bool)`

 SetAttributeSlugNil sets the value for AttributeSlug to be an explicit nil

### UnsetAttributeSlug
`func (o *EntityRulePredicateOverviewResponse) UnsetAttributeSlug()`

UnsetAttributeSlug ensures that no value is present for AttributeSlug, not even an explicit nil
### GetOperator

`func (o *EntityRulePredicateOverviewResponse) GetOperator() string`

GetOperator returns the Operator field if non-nil, zero value otherwise.

### GetOperatorOk

`func (o *EntityRulePredicateOverviewResponse) GetOperatorOk() (*string, bool)`

GetOperatorOk returns a tuple with the Operator field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOperator

`func (o *EntityRulePredicateOverviewResponse) SetOperator(v string)`

SetOperator sets Operator field to given value.


### GetValue

`func (o *EntityRulePredicateOverviewResponse) GetValue() EntityRulePredicateOverviewResponseValue`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *EntityRulePredicateOverviewResponse) GetValueOk() (*EntityRulePredicateOverviewResponseValue, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *EntityRulePredicateOverviewResponse) SetValue(v EntityRulePredicateOverviewResponseValue)`

SetValue sets Value field to given value.

### HasValue

`func (o *EntityRulePredicateOverviewResponse) HasValue() bool`

HasValue returns a boolean if a field has been set.

### SetValueNil

`func (o *EntityRulePredicateOverviewResponse) SetValueNil(b bool)`

 SetValueNil sets the value for Value to be an explicit nil

### UnsetValue
`func (o *EntityRulePredicateOverviewResponse) UnsetValue()`

UnsetValue ensures that no value is present for Value, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


