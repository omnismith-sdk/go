# EntityRuleResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Rule UUID | [optional] 
**TemplateId** | Pointer to **string** | UUID of the template the rule belongs to | [optional] 
**Name** | Pointer to **string** | Short name shown in the template editor | [optional] 
**Message** | Pointer to **string** | Text returned to the client when the rule is violated | [optional] 
**IsEnabled** | Pointer to **bool** | Disabled rules are stored but not enforced | [optional] 
**When** | Pointer to [**[]EntityRulePredicate**](EntityRulePredicate.md) | Conditions that activate the rule; all must hold. Empty means the rule is unconditional. | [optional] 
**Then** | Pointer to [**[]EntityRulePredicate**](EntityRulePredicate.md) | Constraints that must hold once the rule is active; at least one. Each failing constraint yields an &#x60;attributes.&lt;slug&gt;&#x60; error. | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**UpdatedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewEntityRuleResponse

`func NewEntityRuleResponse() *EntityRuleResponse`

NewEntityRuleResponse instantiates a new EntityRuleResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityRuleResponseWithDefaults

`func NewEntityRuleResponseWithDefaults() *EntityRuleResponse`

NewEntityRuleResponseWithDefaults instantiates a new EntityRuleResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *EntityRuleResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *EntityRuleResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *EntityRuleResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *EntityRuleResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetTemplateId

`func (o *EntityRuleResponse) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *EntityRuleResponse) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *EntityRuleResponse) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *EntityRuleResponse) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetName

`func (o *EntityRuleResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *EntityRuleResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *EntityRuleResponse) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *EntityRuleResponse) HasName() bool`

HasName returns a boolean if a field has been set.

### GetMessage

`func (o *EntityRuleResponse) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *EntityRuleResponse) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *EntityRuleResponse) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *EntityRuleResponse) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetIsEnabled

`func (o *EntityRuleResponse) GetIsEnabled() bool`

GetIsEnabled returns the IsEnabled field if non-nil, zero value otherwise.

### GetIsEnabledOk

`func (o *EntityRuleResponse) GetIsEnabledOk() (*bool, bool)`

GetIsEnabledOk returns a tuple with the IsEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsEnabled

`func (o *EntityRuleResponse) SetIsEnabled(v bool)`

SetIsEnabled sets IsEnabled field to given value.

### HasIsEnabled

`func (o *EntityRuleResponse) HasIsEnabled() bool`

HasIsEnabled returns a boolean if a field has been set.

### GetWhen

`func (o *EntityRuleResponse) GetWhen() []EntityRulePredicate`

GetWhen returns the When field if non-nil, zero value otherwise.

### GetWhenOk

`func (o *EntityRuleResponse) GetWhenOk() (*[]EntityRulePredicate, bool)`

GetWhenOk returns a tuple with the When field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWhen

`func (o *EntityRuleResponse) SetWhen(v []EntityRulePredicate)`

SetWhen sets When field to given value.

### HasWhen

`func (o *EntityRuleResponse) HasWhen() bool`

HasWhen returns a boolean if a field has been set.

### GetThen

`func (o *EntityRuleResponse) GetThen() []EntityRulePredicate`

GetThen returns the Then field if non-nil, zero value otherwise.

### GetThenOk

`func (o *EntityRuleResponse) GetThenOk() (*[]EntityRulePredicate, bool)`

GetThenOk returns a tuple with the Then field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThen

`func (o *EntityRuleResponse) SetThen(v []EntityRulePredicate)`

SetThen sets Then field to given value.

### HasThen

`func (o *EntityRuleResponse) HasThen() bool`

HasThen returns a boolean if a field has been set.

### GetCreatedAt

`func (o *EntityRuleResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *EntityRuleResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *EntityRuleResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *EntityRuleResponse) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *EntityRuleResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *EntityRuleResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *EntityRuleResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *EntityRuleResponse) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


