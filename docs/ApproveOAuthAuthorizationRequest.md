# ApproveOAuthAuthorizationRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ClientId** | **string** | Client identifier | 
**RedirectUri** | **string** | Redirection URI to return the authorization code | 
**ProjectId** | **string** | Selected Project UUID that client will be authorized to access | 
**CodeChallenge** | **string** | PKCE code challenge string (RFC 7636) | 
**CodeChallengeMethod** | Pointer to **string** | PKCE challenge transformation method | [optional] 
**Scopes** | Pointer to **[]string** | Authorized scope strings | [optional] 
**State** | Pointer to **NullableString** | Opaque client state parameter for CSRF mitigation | [optional] 

## Methods

### NewApproveOAuthAuthorizationRequest

`func NewApproveOAuthAuthorizationRequest(clientId string, redirectUri string, projectId string, codeChallenge string, ) *ApproveOAuthAuthorizationRequest`

NewApproveOAuthAuthorizationRequest instantiates a new ApproveOAuthAuthorizationRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApproveOAuthAuthorizationRequestWithDefaults

`func NewApproveOAuthAuthorizationRequestWithDefaults() *ApproveOAuthAuthorizationRequest`

NewApproveOAuthAuthorizationRequestWithDefaults instantiates a new ApproveOAuthAuthorizationRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetClientId

`func (o *ApproveOAuthAuthorizationRequest) GetClientId() string`

GetClientId returns the ClientId field if non-nil, zero value otherwise.

### GetClientIdOk

`func (o *ApproveOAuthAuthorizationRequest) GetClientIdOk() (*string, bool)`

GetClientIdOk returns a tuple with the ClientId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientId

`func (o *ApproveOAuthAuthorizationRequest) SetClientId(v string)`

SetClientId sets ClientId field to given value.


### GetRedirectUri

`func (o *ApproveOAuthAuthorizationRequest) GetRedirectUri() string`

GetRedirectUri returns the RedirectUri field if non-nil, zero value otherwise.

### GetRedirectUriOk

`func (o *ApproveOAuthAuthorizationRequest) GetRedirectUriOk() (*string, bool)`

GetRedirectUriOk returns a tuple with the RedirectUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRedirectUri

`func (o *ApproveOAuthAuthorizationRequest) SetRedirectUri(v string)`

SetRedirectUri sets RedirectUri field to given value.


### GetProjectId

`func (o *ApproveOAuthAuthorizationRequest) GetProjectId() string`

GetProjectId returns the ProjectId field if non-nil, zero value otherwise.

### GetProjectIdOk

`func (o *ApproveOAuthAuthorizationRequest) GetProjectIdOk() (*string, bool)`

GetProjectIdOk returns a tuple with the ProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectId

`func (o *ApproveOAuthAuthorizationRequest) SetProjectId(v string)`

SetProjectId sets ProjectId field to given value.


### GetCodeChallenge

`func (o *ApproveOAuthAuthorizationRequest) GetCodeChallenge() string`

GetCodeChallenge returns the CodeChallenge field if non-nil, zero value otherwise.

### GetCodeChallengeOk

`func (o *ApproveOAuthAuthorizationRequest) GetCodeChallengeOk() (*string, bool)`

GetCodeChallengeOk returns a tuple with the CodeChallenge field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCodeChallenge

`func (o *ApproveOAuthAuthorizationRequest) SetCodeChallenge(v string)`

SetCodeChallenge sets CodeChallenge field to given value.


### GetCodeChallengeMethod

`func (o *ApproveOAuthAuthorizationRequest) GetCodeChallengeMethod() string`

GetCodeChallengeMethod returns the CodeChallengeMethod field if non-nil, zero value otherwise.

### GetCodeChallengeMethodOk

`func (o *ApproveOAuthAuthorizationRequest) GetCodeChallengeMethodOk() (*string, bool)`

GetCodeChallengeMethodOk returns a tuple with the CodeChallengeMethod field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCodeChallengeMethod

`func (o *ApproveOAuthAuthorizationRequest) SetCodeChallengeMethod(v string)`

SetCodeChallengeMethod sets CodeChallengeMethod field to given value.

### HasCodeChallengeMethod

`func (o *ApproveOAuthAuthorizationRequest) HasCodeChallengeMethod() bool`

HasCodeChallengeMethod returns a boolean if a field has been set.

### GetScopes

`func (o *ApproveOAuthAuthorizationRequest) GetScopes() []string`

GetScopes returns the Scopes field if non-nil, zero value otherwise.

### GetScopesOk

`func (o *ApproveOAuthAuthorizationRequest) GetScopesOk() (*[]string, bool)`

GetScopesOk returns a tuple with the Scopes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScopes

`func (o *ApproveOAuthAuthorizationRequest) SetScopes(v []string)`

SetScopes sets Scopes field to given value.

### HasScopes

`func (o *ApproveOAuthAuthorizationRequest) HasScopes() bool`

HasScopes returns a boolean if a field has been set.

### GetState

`func (o *ApproveOAuthAuthorizationRequest) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *ApproveOAuthAuthorizationRequest) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *ApproveOAuthAuthorizationRequest) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *ApproveOAuthAuthorizationRequest) HasState() bool`

HasState returns a boolean if a field has been set.

### SetStateNil

`func (o *ApproveOAuthAuthorizationRequest) SetStateNil(b bool)`

 SetStateNil sets the value for State to be an explicit nil

### UnsetState
`func (o *ApproveOAuthAuthorizationRequest) UnsetState()`

UnsetState ensures that no value is present for State, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


