# OAuthTokenRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**GrantType** | **string** | OAuth 2.0 grant type | 
**ClientId** | Pointer to **NullableString** | OAuth client identifier | [optional] 
**ClientSecret** | Pointer to **NullableString** | OAuth client secret (for confidential clients) | [optional] 
**Code** | Pointer to **NullableString** | Authorization code obtained from /oauth/authorize/approve | [optional] 
**RedirectUri** | Pointer to **NullableString** | Original redirection URI matching the authorization request | [optional] 
**CodeVerifier** | Pointer to **NullableString** | PKCE code verifier (RFC 7636) | [optional] 
**RefreshToken** | Pointer to **NullableString** | Refresh token for grant_type&#x3D;refresh_token | [optional] 
**Scope** | Pointer to **NullableString** | Requested scope | [optional] 

## Methods

### NewOAuthTokenRequest

`func NewOAuthTokenRequest(grantType string, ) *OAuthTokenRequest`

NewOAuthTokenRequest instantiates a new OAuthTokenRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewOAuthTokenRequestWithDefaults

`func NewOAuthTokenRequestWithDefaults() *OAuthTokenRequest`

NewOAuthTokenRequestWithDefaults instantiates a new OAuthTokenRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetGrantType

`func (o *OAuthTokenRequest) GetGrantType() string`

GetGrantType returns the GrantType field if non-nil, zero value otherwise.

### GetGrantTypeOk

`func (o *OAuthTokenRequest) GetGrantTypeOk() (*string, bool)`

GetGrantTypeOk returns a tuple with the GrantType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrantType

`func (o *OAuthTokenRequest) SetGrantType(v string)`

SetGrantType sets GrantType field to given value.


### GetClientId

`func (o *OAuthTokenRequest) GetClientId() string`

GetClientId returns the ClientId field if non-nil, zero value otherwise.

### GetClientIdOk

`func (o *OAuthTokenRequest) GetClientIdOk() (*string, bool)`

GetClientIdOk returns a tuple with the ClientId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientId

`func (o *OAuthTokenRequest) SetClientId(v string)`

SetClientId sets ClientId field to given value.

### HasClientId

`func (o *OAuthTokenRequest) HasClientId() bool`

HasClientId returns a boolean if a field has been set.

### SetClientIdNil

`func (o *OAuthTokenRequest) SetClientIdNil(b bool)`

 SetClientIdNil sets the value for ClientId to be an explicit nil

### UnsetClientId
`func (o *OAuthTokenRequest) UnsetClientId()`

UnsetClientId ensures that no value is present for ClientId, not even an explicit nil
### GetClientSecret

`func (o *OAuthTokenRequest) GetClientSecret() string`

GetClientSecret returns the ClientSecret field if non-nil, zero value otherwise.

### GetClientSecretOk

`func (o *OAuthTokenRequest) GetClientSecretOk() (*string, bool)`

GetClientSecretOk returns a tuple with the ClientSecret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientSecret

`func (o *OAuthTokenRequest) SetClientSecret(v string)`

SetClientSecret sets ClientSecret field to given value.

### HasClientSecret

`func (o *OAuthTokenRequest) HasClientSecret() bool`

HasClientSecret returns a boolean if a field has been set.

### SetClientSecretNil

`func (o *OAuthTokenRequest) SetClientSecretNil(b bool)`

 SetClientSecretNil sets the value for ClientSecret to be an explicit nil

### UnsetClientSecret
`func (o *OAuthTokenRequest) UnsetClientSecret()`

UnsetClientSecret ensures that no value is present for ClientSecret, not even an explicit nil
### GetCode

`func (o *OAuthTokenRequest) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *OAuthTokenRequest) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *OAuthTokenRequest) SetCode(v string)`

SetCode sets Code field to given value.

### HasCode

`func (o *OAuthTokenRequest) HasCode() bool`

HasCode returns a boolean if a field has been set.

### SetCodeNil

`func (o *OAuthTokenRequest) SetCodeNil(b bool)`

 SetCodeNil sets the value for Code to be an explicit nil

### UnsetCode
`func (o *OAuthTokenRequest) UnsetCode()`

UnsetCode ensures that no value is present for Code, not even an explicit nil
### GetRedirectUri

`func (o *OAuthTokenRequest) GetRedirectUri() string`

GetRedirectUri returns the RedirectUri field if non-nil, zero value otherwise.

### GetRedirectUriOk

`func (o *OAuthTokenRequest) GetRedirectUriOk() (*string, bool)`

GetRedirectUriOk returns a tuple with the RedirectUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRedirectUri

`func (o *OAuthTokenRequest) SetRedirectUri(v string)`

SetRedirectUri sets RedirectUri field to given value.

### HasRedirectUri

`func (o *OAuthTokenRequest) HasRedirectUri() bool`

HasRedirectUri returns a boolean if a field has been set.

### SetRedirectUriNil

`func (o *OAuthTokenRequest) SetRedirectUriNil(b bool)`

 SetRedirectUriNil sets the value for RedirectUri to be an explicit nil

### UnsetRedirectUri
`func (o *OAuthTokenRequest) UnsetRedirectUri()`

UnsetRedirectUri ensures that no value is present for RedirectUri, not even an explicit nil
### GetCodeVerifier

`func (o *OAuthTokenRequest) GetCodeVerifier() string`

GetCodeVerifier returns the CodeVerifier field if non-nil, zero value otherwise.

### GetCodeVerifierOk

`func (o *OAuthTokenRequest) GetCodeVerifierOk() (*string, bool)`

GetCodeVerifierOk returns a tuple with the CodeVerifier field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCodeVerifier

`func (o *OAuthTokenRequest) SetCodeVerifier(v string)`

SetCodeVerifier sets CodeVerifier field to given value.

### HasCodeVerifier

`func (o *OAuthTokenRequest) HasCodeVerifier() bool`

HasCodeVerifier returns a boolean if a field has been set.

### SetCodeVerifierNil

`func (o *OAuthTokenRequest) SetCodeVerifierNil(b bool)`

 SetCodeVerifierNil sets the value for CodeVerifier to be an explicit nil

### UnsetCodeVerifier
`func (o *OAuthTokenRequest) UnsetCodeVerifier()`

UnsetCodeVerifier ensures that no value is present for CodeVerifier, not even an explicit nil
### GetRefreshToken

`func (o *OAuthTokenRequest) GetRefreshToken() string`

GetRefreshToken returns the RefreshToken field if non-nil, zero value otherwise.

### GetRefreshTokenOk

`func (o *OAuthTokenRequest) GetRefreshTokenOk() (*string, bool)`

GetRefreshTokenOk returns a tuple with the RefreshToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRefreshToken

`func (o *OAuthTokenRequest) SetRefreshToken(v string)`

SetRefreshToken sets RefreshToken field to given value.

### HasRefreshToken

`func (o *OAuthTokenRequest) HasRefreshToken() bool`

HasRefreshToken returns a boolean if a field has been set.

### SetRefreshTokenNil

`func (o *OAuthTokenRequest) SetRefreshTokenNil(b bool)`

 SetRefreshTokenNil sets the value for RefreshToken to be an explicit nil

### UnsetRefreshToken
`func (o *OAuthTokenRequest) UnsetRefreshToken()`

UnsetRefreshToken ensures that no value is present for RefreshToken, not even an explicit nil
### GetScope

`func (o *OAuthTokenRequest) GetScope() string`

GetScope returns the Scope field if non-nil, zero value otherwise.

### GetScopeOk

`func (o *OAuthTokenRequest) GetScopeOk() (*string, bool)`

GetScopeOk returns a tuple with the Scope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScope

`func (o *OAuthTokenRequest) SetScope(v string)`

SetScope sets Scope field to given value.

### HasScope

`func (o *OAuthTokenRequest) HasScope() bool`

HasScope returns a boolean if a field has been set.

### SetScopeNil

`func (o *OAuthTokenRequest) SetScopeNil(b bool)`

 SetScopeNil sets the value for Scope to be an explicit nil

### UnsetScope
`func (o *OAuthTokenRequest) UnsetScope()`

UnsetScope ensures that no value is present for Scope, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


