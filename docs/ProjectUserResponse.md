# ProjectUserResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**UserId** | Pointer to **string** |  | [optional] 
**ProjectId** | Pointer to **string** |  | [optional] 
**RoleId** | Pointer to **string** |  | [optional] 
**RoleName** | Pointer to **string** | Human-readable role name | [optional] [readonly] 
**UserEmail** | Pointer to **string** | User&#39;s email address | [optional] [readonly] 
**UserName** | Pointer to **NullableString** | User&#39;s display name | [optional] [readonly] 
**JoinedAt** | Pointer to **time.Time** |  | [optional] 
**LeftAt** | Pointer to **NullableTime** |  | [optional] 

## Methods

### NewProjectUserResponse

`func NewProjectUserResponse() *ProjectUserResponse`

NewProjectUserResponse instantiates a new ProjectUserResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewProjectUserResponseWithDefaults

`func NewProjectUserResponseWithDefaults() *ProjectUserResponse`

NewProjectUserResponseWithDefaults instantiates a new ProjectUserResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *ProjectUserResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *ProjectUserResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *ProjectUserResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *ProjectUserResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetUserId

`func (o *ProjectUserResponse) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *ProjectUserResponse) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *ProjectUserResponse) SetUserId(v string)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *ProjectUserResponse) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetProjectId

`func (o *ProjectUserResponse) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *ProjectUserResponse) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *ProjectUserResponse) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.

### HasProjectId

`func (o *ProjectUserResponse) HasProjectId() bool`

HasProjectId returns a boolean if a field has been set.

### GetRoleId

`func (o *ProjectUserResponse) GetRoleId() string`

GetRoleId returns the RoleId field if non-nil, zero value otherwise.

### GetRoleIdOk

`func (o *ProjectUserResponse) GetRoleIdOk() (*string, bool)`

GetRoleIdOk returns a tuple with the RoleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoleId

`func (o *ProjectUserResponse) SetRoleId(v string)`

SetRoleId sets RoleId field to given value.

### HasRoleId

`func (o *ProjectUserResponse) HasRoleId() bool`

HasRoleId returns a boolean if a field has been set.

### GetRoleName

`func (o *ProjectUserResponse) GetRoleName() string`

GetRoleName returns the RoleName field if non-nil, zero value otherwise.

### GetRoleNameOk

`func (o *ProjectUserResponse) GetRoleNameOk() (*string, bool)`

GetRoleNameOk returns a tuple with the RoleName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoleName

`func (o *ProjectUserResponse) SetRoleName(v string)`

SetRoleName sets RoleName field to given value.

### HasRoleName

`func (o *ProjectUserResponse) HasRoleName() bool`

HasRoleName returns a boolean if a field has been set.

### GetUserEmail

`func (o *ProjectUserResponse) GetUserEmail() string`

GetUserEmail returns the UserEmail field if non-nil, zero value otherwise.

### GetUserEmailOk

`func (o *ProjectUserResponse) GetUserEmailOk() (*string, bool)`

GetUserEmailOk returns a tuple with the UserEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserEmail

`func (o *ProjectUserResponse) SetUserEmail(v string)`

SetUserEmail sets UserEmail field to given value.

### HasUserEmail

`func (o *ProjectUserResponse) HasUserEmail() bool`

HasUserEmail returns a boolean if a field has been set.

### GetUserName

`func (o *ProjectUserResponse) GetUserName() string`

GetUserName returns the UserName field if non-nil, zero value otherwise.

### GetUserNameOk

`func (o *ProjectUserResponse) GetUserNameOk() (*string, bool)`

GetUserNameOk returns a tuple with the UserName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserName

`func (o *ProjectUserResponse) SetUserName(v string)`

SetUserName sets UserName field to given value.

### HasUserName

`func (o *ProjectUserResponse) HasUserName() bool`

HasUserName returns a boolean if a field has been set.

### SetUserNameNil

`func (o *ProjectUserResponse) SetUserNameNil(b bool)`

 SetUserNameNil sets the value for UserName to be an explicit nil

### UnsetUserName
`func (o *ProjectUserResponse) UnsetUserName()`

UnsetUserName ensures that no value is present for UserName, not even an explicit nil
### GetJoinedAt

`func (o *ProjectUserResponse) GetJoinedAt() time.Time`

GetJoinedAt returns the JoinedAt field if non-nil, zero value otherwise.

### GetJoinedAtOk

`func (o *ProjectUserResponse) GetJoinedAtOk() (*time.Time, bool)`

GetJoinedAtOk returns a tuple with the JoinedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJoinedAt

`func (o *ProjectUserResponse) SetJoinedAt(v time.Time)`

SetJoinedAt sets JoinedAt field to given value.

### HasJoinedAt

`func (o *ProjectUserResponse) HasJoinedAt() bool`

HasJoinedAt returns a boolean if a field has been set.

### GetLeftAt

`func (o *ProjectUserResponse) GetLeftAt() time.Time`

GetLeftAt returns the LeftAt field if non-nil, zero value otherwise.

### GetLeftAtOk

`func (o *ProjectUserResponse) GetLeftAtOk() (*time.Time, bool)`

GetLeftAtOk returns a tuple with the LeftAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLeftAt

`func (o *ProjectUserResponse) SetLeftAt(v time.Time)`

SetLeftAt sets LeftAt field to given value.

### HasLeftAt

`func (o *ProjectUserResponse) HasLeftAt() bool`

HasLeftAt returns a boolean if a field has been set.

### SetLeftAtNil

`func (o *ProjectUserResponse) SetLeftAtNil(b bool)`

 SetLeftAtNil sets the value for LeftAt to be an explicit nil

### UnsetLeftAt
`func (o *ProjectUserResponse) UnsetLeftAt()`

UnsetLeftAt ensures that no value is present for LeftAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


