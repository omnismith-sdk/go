# UpdateEntityRuleRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Short name shown in the template editor | 
**Message** | **string** | Text returned to the client when the rule is violated | 
**When** | Pointer to [**[]EntityRulePredicate**](EntityRulePredicate.md) | Full replacement of the activation conditions; empty for an unconditional rule | [optional] 
**Then** | [**[]EntityRulePredicate**](EntityRulePredicate.md) | Full replacement of the constraints | 

## Methods

### NewUpdateEntityRuleRequest

`func NewUpdateEntityRuleRequest(name string, message string, then []EntityRulePredicate, ) *UpdateEntityRuleRequest`

NewUpdateEntityRuleRequest instantiates a new UpdateEntityRuleRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateEntityRuleRequestWithDefaults

`func NewUpdateEntityRuleRequestWithDefaults() *UpdateEntityRuleRequest`

NewUpdateEntityRuleRequestWithDefaults instantiates a new UpdateEntityRuleRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *UpdateEntityRuleRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateEntityRuleRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateEntityRuleRequest) SetName(v string)`

SetName sets Name field to given value.


### GetMessage

`func (o *UpdateEntityRuleRequest) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *UpdateEntityRuleRequest) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *UpdateEntityRuleRequest) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetWhen

`func (o *UpdateEntityRuleRequest) GetWhen() []EntityRulePredicate`

GetWhen returns the When field if non-nil, zero value otherwise.

### GetWhenOk

`func (o *UpdateEntityRuleRequest) GetWhenOk() (*[]EntityRulePredicate, bool)`

GetWhenOk returns a tuple with the When field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWhen

`func (o *UpdateEntityRuleRequest) SetWhen(v []EntityRulePredicate)`

SetWhen sets When field to given value.

### HasWhen

`func (o *UpdateEntityRuleRequest) HasWhen() bool`

HasWhen returns a boolean if a field has been set.

### GetThen

`func (o *UpdateEntityRuleRequest) GetThen() []EntityRulePredicate`

GetThen returns the Then field if non-nil, zero value otherwise.

### GetThenOk

`func (o *UpdateEntityRuleRequest) GetThenOk() (*[]EntityRulePredicate, bool)`

GetThenOk returns a tuple with the Then field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThen

`func (o *UpdateEntityRuleRequest) SetThen(v []EntityRulePredicate)`

SetThen sets Then field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


