# EntityRuleOverviewResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Rule UUID | 
**Name** | **string** | Short rule name | 
**Message** | **string** | Error message returned on violation | 
**IsEnabled** | **bool** | Whether the rule is actively enforced | 
**When** | [**[]EntityRulePredicateOverviewResponse**](EntityRulePredicateOverviewResponse.md) | Activating conditions; empty means unconditional | 
**Then** | [**[]EntityRulePredicateOverviewResponse**](EntityRulePredicateOverviewResponse.md) | Enforced constraints | 

## Methods

### NewEntityRuleOverviewResponse

`func NewEntityRuleOverviewResponse(id string, name string, message string, isEnabled bool, when []EntityRulePredicateOverviewResponse, then []EntityRulePredicateOverviewResponse, ) *EntityRuleOverviewResponse`

NewEntityRuleOverviewResponse instantiates a new EntityRuleOverviewResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityRuleOverviewResponseWithDefaults

`func NewEntityRuleOverviewResponseWithDefaults() *EntityRuleOverviewResponse`

NewEntityRuleOverviewResponseWithDefaults instantiates a new EntityRuleOverviewResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *EntityRuleOverviewResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *EntityRuleOverviewResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *EntityRuleOverviewResponse) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *EntityRuleOverviewResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *EntityRuleOverviewResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *EntityRuleOverviewResponse) SetName(v string)`

SetName sets Name field to given value.


### GetMessage

`func (o *EntityRuleOverviewResponse) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *EntityRuleOverviewResponse) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *EntityRuleOverviewResponse) SetMessage(v string)`

SetMessage sets Message field to given value.


### GetIsEnabled

`func (o *EntityRuleOverviewResponse) GetIsEnabled() bool`

GetIsEnabled returns the IsEnabled field if non-nil, zero value otherwise.

### GetIsEnabledOk

`func (o *EntityRuleOverviewResponse) GetIsEnabledOk() (*bool, bool)`

GetIsEnabledOk returns a tuple with the IsEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsEnabled

`func (o *EntityRuleOverviewResponse) SetIsEnabled(v bool)`

SetIsEnabled sets IsEnabled field to given value.


### GetWhen

`func (o *EntityRuleOverviewResponse) GetWhen() []EntityRulePredicateOverviewResponse`

GetWhen returns the When field if non-nil, zero value otherwise.

### GetWhenOk

`func (o *EntityRuleOverviewResponse) GetWhenOk() (*[]EntityRulePredicateOverviewResponse, bool)`

GetWhenOk returns a tuple with the When field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWhen

`func (o *EntityRuleOverviewResponse) SetWhen(v []EntityRulePredicateOverviewResponse)`

SetWhen sets When field to given value.


### GetThen

`func (o *EntityRuleOverviewResponse) GetThen() []EntityRulePredicateOverviewResponse`

GetThen returns the Then field if non-nil, zero value otherwise.

### GetThenOk

`func (o *EntityRuleOverviewResponse) GetThenOk() (*[]EntityRulePredicateOverviewResponse, bool)`

GetThenOk returns a tuple with the Then field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThen

`func (o *EntityRuleOverviewResponse) SetThen(v []EntityRulePredicateOverviewResponse)`

SetThen sets Then field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


