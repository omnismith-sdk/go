# GetOAuthAuthorizeInfo200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ClientId** | Pointer to **string** | OAuth client identifier | [optional] 
**ClientName** | Pointer to **string** | Human-readable client application name | [optional] 
**RedirectUri** | Pointer to **string** | Validated redirection callback URI | [optional] 
**Scopes** | Pointer to **[]string** | List of requested scopes | [optional] 
**UserEmail** | Pointer to **string** | Email address of the currently authenticated user | [optional] 
**ActiveProjectId** | Pointer to **NullableString** | Currently active project ID for the user session | [optional] 
**Projects** | Pointer to [**[]GetOAuthAuthorizeInfo200ResponseProjectsInner**](GetOAuthAuthorizeInfo200ResponseProjectsInner.md) | List of projects accessible by the authenticated user | [optional] 
**State** | Pointer to **NullableString** | Echoed client state parameter | [optional] 

## Methods

### NewGetOAuthAuthorizeInfo200Response

`func NewGetOAuthAuthorizeInfo200Response() *GetOAuthAuthorizeInfo200Response`

NewGetOAuthAuthorizeInfo200Response instantiates a new GetOAuthAuthorizeInfo200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetOAuthAuthorizeInfo200ResponseWithDefaults

`func NewGetOAuthAuthorizeInfo200ResponseWithDefaults() *GetOAuthAuthorizeInfo200Response`

NewGetOAuthAuthorizeInfo200ResponseWithDefaults instantiates a new GetOAuthAuthorizeInfo200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetClientId

`func (o *GetOAuthAuthorizeInfo200Response) GetClientId() string`

GetClientId returns the ClientId field if non-nil, zero value otherwise.

### GetClientIdOk

`func (o *GetOAuthAuthorizeInfo200Response) GetClientIdOk() (*string, bool)`

GetClientIdOk returns a tuple with the ClientId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientId

`func (o *GetOAuthAuthorizeInfo200Response) SetClientId(v string)`

SetClientId sets ClientId field to given value.

### HasClientId

`func (o *GetOAuthAuthorizeInfo200Response) HasClientId() bool`

HasClientId returns a boolean if a field has been set.

### GetClientName

`func (o *GetOAuthAuthorizeInfo200Response) GetClientName() string`

GetClientName returns the ClientName field if non-nil, zero value otherwise.

### GetClientNameOk

`func (o *GetOAuthAuthorizeInfo200Response) GetClientNameOk() (*string, bool)`

GetClientNameOk returns a tuple with the ClientName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientName

`func (o *GetOAuthAuthorizeInfo200Response) SetClientName(v string)`

SetClientName sets ClientName field to given value.

### HasClientName

`func (o *GetOAuthAuthorizeInfo200Response) HasClientName() bool`

HasClientName returns a boolean if a field has been set.

### GetRedirectUri

`func (o *GetOAuthAuthorizeInfo200Response) GetRedirectUri() string`

GetRedirectUri returns the RedirectUri field if non-nil, zero value otherwise.

### GetRedirectUriOk

`func (o *GetOAuthAuthorizeInfo200Response) GetRedirectUriOk() (*string, bool)`

GetRedirectUriOk returns a tuple with the RedirectUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRedirectUri

`func (o *GetOAuthAuthorizeInfo200Response) SetRedirectUri(v string)`

SetRedirectUri sets RedirectUri field to given value.

### HasRedirectUri

`func (o *GetOAuthAuthorizeInfo200Response) HasRedirectUri() bool`

HasRedirectUri returns a boolean if a field has been set.

### GetScopes

`func (o *GetOAuthAuthorizeInfo200Response) GetScopes() []string`

GetScopes returns the Scopes field if non-nil, zero value otherwise.

### GetScopesOk

`func (o *GetOAuthAuthorizeInfo200Response) GetScopesOk() (*[]string, bool)`

GetScopesOk returns a tuple with the Scopes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScopes

`func (o *GetOAuthAuthorizeInfo200Response) SetScopes(v []string)`

SetScopes sets Scopes field to given value.

### HasScopes

`func (o *GetOAuthAuthorizeInfo200Response) HasScopes() bool`

HasScopes returns a boolean if a field has been set.

### GetUserEmail

`func (o *GetOAuthAuthorizeInfo200Response) GetUserEmail() string`

GetUserEmail returns the UserEmail field if non-nil, zero value otherwise.

### GetUserEmailOk

`func (o *GetOAuthAuthorizeInfo200Response) GetUserEmailOk() (*string, bool)`

GetUserEmailOk returns a tuple with the UserEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserEmail

`func (o *GetOAuthAuthorizeInfo200Response) SetUserEmail(v string)`

SetUserEmail sets UserEmail field to given value.

### HasUserEmail

`func (o *GetOAuthAuthorizeInfo200Response) HasUserEmail() bool`

HasUserEmail returns a boolean if a field has been set.

### GetActiveProjectId

`func (o *GetOAuthAuthorizeInfo200Response) GetActiveProjectId() string`

GetActiveProjectId returns the ActiveProjectId field if non-nil, zero value otherwise.

### GetActiveProjectIdOk

`func (o *GetOAuthAuthorizeInfo200Response) GetActiveProjectIdOk() (*string, bool)`

GetActiveProjectIdOk returns a tuple with the ActiveProjectId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActiveProjectId

`func (o *GetOAuthAuthorizeInfo200Response) SetActiveProjectId(v string)`

SetActiveProjectId sets ActiveProjectId field to given value.

### HasActiveProjectId

`func (o *GetOAuthAuthorizeInfo200Response) HasActiveProjectId() bool`

HasActiveProjectId returns a boolean if a field has been set.

### SetActiveProjectIdNil

`func (o *GetOAuthAuthorizeInfo200Response) SetActiveProjectIdNil(b bool)`

 SetActiveProjectIdNil sets the value for ActiveProjectId to be an explicit nil

### UnsetActiveProjectId
`func (o *GetOAuthAuthorizeInfo200Response) UnsetActiveProjectId()`

UnsetActiveProjectId ensures that no value is present for ActiveProjectId, not even an explicit nil
### GetProjects

`func (o *GetOAuthAuthorizeInfo200Response) GetProjects() []GetOAuthAuthorizeInfo200ResponseProjectsInner`

GetProjects returns the Projects field if non-nil, zero value otherwise.

### GetProjectsOk

`func (o *GetOAuthAuthorizeInfo200Response) GetProjectsOk() (*[]GetOAuthAuthorizeInfo200ResponseProjectsInner, bool)`

GetProjectsOk returns a tuple with the Projects field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjects

`func (o *GetOAuthAuthorizeInfo200Response) SetProjects(v []GetOAuthAuthorizeInfo200ResponseProjectsInner)`

SetProjects sets Projects field to given value.

### HasProjects

`func (o *GetOAuthAuthorizeInfo200Response) HasProjects() bool`

HasProjects returns a boolean if a field has been set.

### GetState

`func (o *GetOAuthAuthorizeInfo200Response) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *GetOAuthAuthorizeInfo200Response) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *GetOAuthAuthorizeInfo200Response) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *GetOAuthAuthorizeInfo200Response) HasState() bool`

HasState returns a boolean if a field has been set.

### SetStateNil

`func (o *GetOAuthAuthorizeInfo200Response) SetStateNil(b bool)`

 SetStateNil sets the value for State to be an explicit nil

### UnsetState
`func (o *GetOAuthAuthorizeInfo200Response) UnsetState()`

UnsetState ensures that no value is present for State, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


