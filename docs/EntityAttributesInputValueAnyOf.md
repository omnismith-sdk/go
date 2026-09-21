# EntityAttributesInputValueAnyOf

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Value** | [**EntityAttributesInputValueAnyOfValue**](EntityAttributesInputValueAnyOfValue.md) |  | 
**UpdatedAt** | Pointer to **time.Time** | RFC 3339 timestamp with an explicit offset (&#x60;Z&#x60; or &#x60;±HH:MM&#x60;). Defaults to now when omitted. | [optional] 

## Methods

### NewEntityAttributesInputValueAnyOf

`func NewEntityAttributesInputValueAnyOf(value EntityAttributesInputValueAnyOfValue, ) *EntityAttributesInputValueAnyOf`

NewEntityAttributesInputValueAnyOf instantiates a new EntityAttributesInputValueAnyOf object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityAttributesInputValueAnyOfWithDefaults

`func NewEntityAttributesInputValueAnyOfWithDefaults() *EntityAttributesInputValueAnyOf`

NewEntityAttributesInputValueAnyOfWithDefaults instantiates a new EntityAttributesInputValueAnyOf object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValue

`func (o *EntityAttributesInputValueAnyOf) GetValue() EntityAttributesInputValueAnyOfValue`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *EntityAttributesInputValueAnyOf) GetValueOk() (*EntityAttributesInputValueAnyOfValue, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *EntityAttributesInputValueAnyOf) SetValue(v EntityAttributesInputValueAnyOfValue)`

SetValue sets Value field to given value.


### GetUpdatedAt

`func (o *EntityAttributesInputValueAnyOf) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *EntityAttributesInputValueAnyOf) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *EntityAttributesInputValueAnyOf) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *EntityAttributesInputValueAnyOf) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


