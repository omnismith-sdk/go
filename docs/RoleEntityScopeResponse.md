# RoleEntityScopeResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | Pointer to **string** | Target template UUID to which this scope applies | [optional] 
**Conditions** | Pointer to [**[]RoleEntityScopeConditionResponse**](RoleEntityScopeConditionResponse.md) | List of filter criteria that entities must satisfy for users with this role to access them | [optional] 

## Methods

### NewRoleEntityScopeResponse

`func NewRoleEntityScopeResponse() *RoleEntityScopeResponse`

NewRoleEntityScopeResponse instantiates a new RoleEntityScopeResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRoleEntityScopeResponseWithDefaults

`func NewRoleEntityScopeResponseWithDefaults() *RoleEntityScopeResponse`

NewRoleEntityScopeResponseWithDefaults instantiates a new RoleEntityScopeResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *RoleEntityScopeResponse) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *RoleEntityScopeResponse) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *RoleEntityScopeResponse) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *RoleEntityScopeResponse) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetConditions

`func (o *RoleEntityScopeResponse) GetConditions() []RoleEntityScopeConditionResponse`

GetConditions returns the Conditions field if non-nil, zero value otherwise.

### GetConditionsOk

`func (o *RoleEntityScopeResponse) GetConditionsOk() (*[]RoleEntityScopeConditionResponse, bool)`

GetConditionsOk returns a tuple with the Conditions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConditions

`func (o *RoleEntityScopeResponse) SetConditions(v []RoleEntityScopeConditionResponse)`

SetConditions sets Conditions field to given value.

### HasConditions

`func (o *RoleEntityScopeResponse) HasConditions() bool`

HasConditions returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


