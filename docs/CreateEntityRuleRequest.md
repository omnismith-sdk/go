# CreateEntityRuleRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Short name shown in the template editor | 
**Message** | **string** | Text returned to the client when the rule is violated | 
**When** | Pointer to [**[]EntityRulePredicate**](EntityRulePredicate.md) | Conditions that activate the rule; all must hold. Omit or send an empty list for an unconditional rule (a plain required field). | [optional] 
**Then** | [**[]EntityRulePredicate**](EntityRulePredicate.md) | Constraints that must hold once the rule is active. &#x60;is_not_empty&#x60; on an attribute is the \&quot;required\&quot; constraint. | 

## Methods

### NewCreateEntityRuleRequest

`func NewCreateEntityRuleRequest(name string, message string, then []EntityRulePredicate, ) *CreateEntityRuleRequest`

NewCreateEntityRuleRequest instantiates a new CreateEntityRuleRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateEntityRuleRequestWithDefaults

`func NewCreateEntityRuleRequestWithDefaults() *CreateEntityRuleRequest`

NewCreateEntityRuleRequestWithDefaults instantiates a new CreateEntityRuleRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreateEntityRuleRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateEntityRuleRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateEntityRuleRequest) SetName(v string)`

SetName sets Name field to given value.


### GetMessage

`func (o *CreateEntityRuleRequest) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *CreateEntityRuleRequest) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *CreateEntityRuleRequest) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetWhen

`func (o *CreateEntityRuleRequest) GetWhen() []EntityRulePredicate`

GetWhen returns the When field if non-nil, zero value otherwise.

### GetWhenOk

`func (o *CreateEntityRuleRequest) GetWhenOk() (*[]EntityRulePredicate, bool)`

GetWhenOk returns a tuple with the When field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWhen

`func (o *CreateEntityRuleRequest) SetWhen(v []EntityRulePredicate)`

SetWhen sets When field to given value.

### HasWhen

`func (o *CreateEntityRuleRequest) HasWhen() bool`

HasWhen returns a boolean if a field has been set.

### GetThen

`func (o *CreateEntityRuleRequest) GetThen() []EntityRulePredicate`

GetThen returns the Then field if non-nil, zero value otherwise.

### GetThenOk

`func (o *CreateEntityRuleRequest) GetThenOk() (*[]EntityRulePredicate, bool)`

GetThenOk returns a tuple with the Then field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThen

`func (o *CreateEntityRuleRequest) SetThen(v []EntityRulePredicate)`

SetThen sets Then field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


