# SessionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Unique UUID identifier of the session | [optional] 
**UserId** | Pointer to **string** | UUID of the authenticated user | [optional] 
**Email** | Pointer to **string** | Email address of the session owner | [optional] 
**RoleId** | Pointer to **string** | Active role UUID under this session | [optional] 
**IpAddress** | Pointer to **NullableString** | Client IP address from which the session was established | [optional] 
**UserAgent** | Pointer to **NullableString** | User-Agent header string of the client browser/application | [optional] 
**CreatedAt** | Pointer to **time.Time** | Timestamp when the session was created | [optional] 
**ExpiresAt** | Pointer to **time.Time** | Expiration timestamp after which the session becomes invalid | [optional] 
**RevokedAt** | Pointer to **NullableTime** | Timestamp when the session was explicitly revoked | [optional] 
**RevokedBy** | Pointer to **NullableString** | User UUID who revoked the session | [optional] 
**RevokedReason** | Pointer to **NullableString** | Reason note provided upon session revocation | [optional] 
**Status** | Pointer to **string** | Current session status state | [optional] 

## Methods

### NewSessionResponse

`func NewSessionResponse() *SessionResponse`

NewSessionResponse instantiates a new SessionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSessionResponseWithDefaults

`func NewSessionResponseWithDefaults() *SessionResponse`

NewSessionResponseWithDefaults instantiates a new SessionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *SessionResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *SessionResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *SessionResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *SessionResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetUserId

`func (o *SessionResponse) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *SessionResponse) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *SessionResponse) SetUserId(v string)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *SessionResponse) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetEmail

`func (o *SessionResponse) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *SessionResponse) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *SessionResponse) SetEmail(v string)`

SetEmail sets Email field to given value.

### HasEmail

`func (o *SessionResponse) HasEmail() bool`

HasEmail returns a boolean if a field has been set.

### GetRoleId

`func (o *SessionResponse) GetRoleId() string`

GetRoleId returns the RoleId field if non-nil, zero value otherwise.

### GetRoleIdOk

`func (o *SessionResponse) GetRoleIdOk() (*string, bool)`

GetRoleIdOk returns a tuple with the RoleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRoleId

`func (o *SessionResponse) SetRoleId(v string)`

SetRoleId sets RoleId field to given value.

### HasRoleId

`func (o *SessionResponse) HasRoleId() bool`

HasRoleId returns a boolean if a field has been set.

### GetIpAddress

`func (o *SessionResponse) GetIpAddress() string`

GetIpAddress returns the IpAddress field if non-nil, zero value otherwise.

### GetIpAddressOk

`func (o *SessionResponse) GetIpAddressOk() (*string, bool)`

GetIpAddressOk returns a tuple with the IpAddress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIpAddress

`func (o *SessionResponse) SetIpAddress(v string)`

SetIpAddress sets IpAddress field to given value.

### HasIpAddress

`func (o *SessionResponse) HasIpAddress() bool`

HasIpAddress returns a boolean if a field has been set.

### SetIpAddressNil

`func (o *SessionResponse) SetIpAddressNil(b bool)`

 SetIpAddressNil sets the value for IpAddress to be an explicit nil

### UnsetIpAddress
`func (o *SessionResponse) UnsetIpAddress()`

UnsetIpAddress ensures that no value is present for IpAddress, not even an explicit nil
### GetUserAgent

`func (o *SessionResponse) GetUserAgent() string`

GetUserAgent returns the UserAgent field if non-nil, zero value otherwise.

### GetUserAgentOk

`func (o *SessionResponse) GetUserAgentOk() (*string, bool)`

GetUserAgentOk returns a tuple with the UserAgent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserAgent

`func (o *SessionResponse) SetUserAgent(v string)`

SetUserAgent sets UserAgent field to given value.

### HasUserAgent

`func (o *SessionResponse) HasUserAgent() bool`

HasUserAgent returns a boolean if a field has been set.

### SetUserAgentNil

`func (o *SessionResponse) SetUserAgentNil(b bool)`

 SetUserAgentNil sets the value for UserAgent to be an explicit nil

### UnsetUserAgent
`func (o *SessionResponse) UnsetUserAgent()`

UnsetUserAgent ensures that no value is present for UserAgent, not even an explicit nil
### GetCreatedAt

`func (o *SessionResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *SessionResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *SessionResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *SessionResponse) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetExpiresAt

`func (o *SessionResponse) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *SessionResponse) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *SessionResponse) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *SessionResponse) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### GetRevokedAt

`func (o *SessionResponse) GetRevokedAt() time.Time`

GetRevokedAt returns the RevokedAt field if non-nil, zero value otherwise.

### GetRevokedAtOk

`func (o *SessionResponse) GetRevokedAtOk() (*time.Time, bool)`

GetRevokedAtOk returns a tuple with the RevokedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRevokedAt

`func (o *SessionResponse) SetRevokedAt(v time.Time)`

SetRevokedAt sets RevokedAt field to given value.

### HasRevokedAt

`func (o *SessionResponse) HasRevokedAt() bool`

HasRevokedAt returns a boolean if a field has been set.

### SetRevokedAtNil

`func (o *SessionResponse) SetRevokedAtNil(b bool)`

 SetRevokedAtNil sets the value for RevokedAt to be an explicit nil

### UnsetRevokedAt
`func (o *SessionResponse) UnsetRevokedAt()`

UnsetRevokedAt ensures that no value is present for RevokedAt, not even an explicit nil
### GetRevokedBy

`func (o *SessionResponse) GetRevokedBy() string`

GetRevokedBy returns the RevokedBy field if non-nil, zero value otherwise.

### GetRevokedByOk

`func (o *SessionResponse) GetRevokedByOk() (*string, bool)`

GetRevokedByOk returns a tuple with the RevokedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRevokedBy

`func (o *SessionResponse) SetRevokedBy(v string)`

SetRevokedBy sets RevokedBy field to given value.

### HasRevokedBy

`func (o *SessionResponse) HasRevokedBy() bool`

HasRevokedBy returns a boolean if a field has been set.

### SetRevokedByNil

`func (o *SessionResponse) SetRevokedByNil(b bool)`

 SetRevokedByNil sets the value for RevokedBy to be an explicit nil

### UnsetRevokedBy
`func (o *SessionResponse) UnsetRevokedBy()`

UnsetRevokedBy ensures that no value is present for RevokedBy, not even an explicit nil
### GetRevokedReason

`func (o *SessionResponse) GetRevokedReason() string`

GetRevokedReason returns the RevokedReason field if non-nil, zero value otherwise.

### GetRevokedReasonOk

`func (o *SessionResponse) GetRevokedReasonOk() (*string, bool)`

GetRevokedReasonOk returns a tuple with the RevokedReason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRevokedReason

`func (o *SessionResponse) SetRevokedReason(v string)`

SetRevokedReason sets RevokedReason field to given value.

### HasRevokedReason

`func (o *SessionResponse) HasRevokedReason() bool`

HasRevokedReason returns a boolean if a field has been set.

### SetRevokedReasonNil

`func (o *SessionResponse) SetRevokedReasonNil(b bool)`

 SetRevokedReasonNil sets the value for RevokedReason to be an explicit nil

### UnsetRevokedReason
`func (o *SessionResponse) UnsetRevokedReason()`

UnsetRevokedReason ensures that no value is present for RevokedReason, not even an explicit nil
### GetStatus

`func (o *SessionResponse) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *SessionResponse) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *SessionResponse) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *SessionResponse) HasStatus() bool`

HasStatus returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


