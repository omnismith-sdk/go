# EntityAttributesInputValue

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Value** | **float32** | The operand, as a JSON number. | 
**UpdatedAt** | Pointer to **time.Time** | RFC 3339 timestamp with an explicit offset (&#x60;Z&#x60; or &#x60;±HH:MM&#x60;). Defaults to now when omitted. | [optional] 
**Op** | **string** | The operation. &#x60;increment&#x60; adds &#x60;value&#x60; (negative to subtract). | 

## Methods

### NewEntityAttributesInputValue

`func NewEntityAttributesInputValue(value float32, op string, ) *EntityAttributesInputValue`

NewEntityAttributesInputValue instantiates a new EntityAttributesInputValue object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityAttributesInputValueWithDefaults

`func NewEntityAttributesInputValueWithDefaults() *EntityAttributesInputValue`

NewEntityAttributesInputValueWithDefaults instantiates a new EntityAttributesInputValue object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetValue

`func (o *EntityAttributesInputValue) GetValue() float32`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *EntityAttributesInputValue) GetValueOk() (*float32, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *EntityAttributesInputValue) SetValue(v float32)`

SetValue sets Value field to given value.


### GetUpdatedAt

`func (o *EntityAttributesInputValue) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *EntityAttributesInputValue) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *EntityAttributesInputValue) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *EntityAttributesInputValue) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.

### GetOp

`func (o *EntityAttributesInputValue) GetOp() string`

GetOp returns the Op field if non-nil, zero value otherwise.

### GetOpOk

`func (o *EntityAttributesInputValue) GetOpOk() (*string, bool)`

GetOpOk returns a tuple with the Op field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOp

`func (o *EntityAttributesInputValue) SetOp(v string)`

SetOp sets Op field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


