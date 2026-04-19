# InviteUserToProjectRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **string** | Email address of the user to invite | 
**RoleId** | **string** | The Role ID to assign | 

## Methods

### NewInviteUserToProjectRequest

`func NewInviteUserToProjectRequest(email string, roleId string, ) *InviteUserToProjectRequest`

NewInviteUserToProjectRequest instantiates a new InviteUserToProjectRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInviteUserToProjectRequestWithDefaults

`func NewInviteUserToProjectRequestWithDefaults() *InviteUserToProjectRequest`

NewInviteUserToProjectRequestWithDefaults instantiates a new InviteUserToProjectRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *InviteUserToProjectRequest) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *InviteUserToProjectRequest) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *InviteUserToProjectRequest) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetRoleId

`func (o *InviteUserToProjectRequest) GetRoleId() string`

GetRoleId returns the RoleId field if non-nil, zero value otherwise.

### GetRoleIdOk

`func (o *InviteUserToProjectRequest) GetRoleIdOk() (*string, bool)`

GetRoleIdOk returns a tuple with the RoleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoleId

`func (o *InviteUserToProjectRequest) SetRoleId(v string)`

SetRoleId sets RoleId field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


