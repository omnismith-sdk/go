# CreateDashboardBlockRequestConfigAggregationsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Op** | Pointer to **string** |  | [optional] 
**Field** | Pointer to **NullableString** | Attribute slug or UUID to reduce. Required for every op except count, which must omit it. | [optional] 

## Methods

### NewCreateDashboardBlockRequestConfigAggregationsInner

`func NewCreateDashboardBlockRequestConfigAggregationsInner() *CreateDashboardBlockRequestConfigAggregationsInner`

NewCreateDashboardBlockRequestConfigAggregationsInner instantiates a new CreateDashboardBlockRequestConfigAggregationsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateDashboardBlockRequestConfigAggregationsInnerWithDefaults

`func NewCreateDashboardBlockRequestConfigAggregationsInnerWithDefaults() *CreateDashboardBlockRequestConfigAggregationsInner`

NewCreateDashboardBlockRequestConfigAggregationsInnerWithDefaults instantiates a new CreateDashboardBlockRequestConfigAggregationsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOp

`func (o *CreateDashboardBlockRequestConfigAggregationsInner) GetOp() string`

GetOp returns the Op field if non-nil, zero value otherwise.

### GetOpOk

`func (o *CreateDashboardBlockRequestConfigAggregationsInner) GetOpOk() (*string, bool)`

GetOpOk returns a tuple with the Op field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOp

`func (o *CreateDashboardBlockRequestConfigAggregationsInner) SetOp(v string)`

SetOp sets Op field to given value.

### HasOp

`func (o *CreateDashboardBlockRequestConfigAggregationsInner) HasOp() bool`

HasOp returns a boolean if a field has been set.

### GetField

`func (o *CreateDashboardBlockRequestConfigAggregationsInner) GetField() string`

GetField returns the Field field if non-nil, zero value otherwise.

### GetFieldOk

`func (o *CreateDashboardBlockRequestConfigAggregationsInner) GetFieldOk() (*string, bool)`

GetFieldOk returns a tuple with the Field field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetField

`func (o *CreateDashboardBlockRequestConfigAggregationsInner) SetField(v string)`

SetField sets Field field to given value.

### HasField

`func (o *CreateDashboardBlockRequestConfigAggregationsInner) HasField() bool`

HasField returns a boolean if a field has been set.

### SetFieldNil

`func (o *CreateDashboardBlockRequestConfigAggregationsInner) SetFieldNil(b bool)`

 SetFieldNil sets the value for Field to be an explicit nil

### UnsetField
`func (o *CreateDashboardBlockRequestConfigAggregationsInner) UnsetField()`

UnsetField ensures that no value is present for Field, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


