# RevokeOAuthTokenRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Token** | **string** | The token string that the client wants to revoke | 
**TokenTypeHint** | Pointer to **string** | Hint about the type of token submitted for revocation | [optional] 
**ClientId** | Pointer to **NullableString** | Client identifier | [optional] 

## Methods

### NewRevokeOAuthTokenRequest

`func NewRevokeOAuthTokenRequest(token string, ) *RevokeOAuthTokenRequest`

NewRevokeOAuthTokenRequest instantiates a new RevokeOAuthTokenRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRevokeOAuthTokenRequestWithDefaults

`func NewRevokeOAuthTokenRequestWithDefaults() *RevokeOAuthTokenRequest`

NewRevokeOAuthTokenRequestWithDefaults instantiates a new RevokeOAuthTokenRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetToken

`func (o *RevokeOAuthTokenRequest) GetToken() string`

GetToken returns the Token field if non-nil, zero value otherwise.

### GetTokenOk

`func (o *RevokeOAuthTokenRequest) GetTokenOk() (*string, bool)`

GetTokenOk returns a tuple with the Token field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToken

`func (o *RevokeOAuthTokenRequest) SetToken(v string)`

SetToken sets Token field to given value.


### GetTokenTypeHint

`func (o *RevokeOAuthTokenRequest) GetTokenTypeHint() string`

GetTokenTypeHint returns the TokenTypeHint field if non-nil, zero value otherwise.

### GetTokenTypeHintOk

`func (o *RevokeOAuthTokenRequest) GetTokenTypeHintOk() (*string, bool)`

GetTokenTypeHintOk returns a tuple with the TokenTypeHint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenTypeHint

`func (o *RevokeOAuthTokenRequest) SetTokenTypeHint(v string)`

SetTokenTypeHint sets TokenTypeHint field to given value.

### HasTokenTypeHint

`func (o *RevokeOAuthTokenRequest) HasTokenTypeHint() bool`

HasTokenTypeHint returns a boolean if a field has been set.

### GetClientId

`func (o *RevokeOAuthTokenRequest) GetClientId() string`

GetClientId returns the ClientId field if non-nil, zero value otherwise.

### GetClientIdOk

`func (o *RevokeOAuthTokenRequest) GetClientIdOk() (*string, bool)`

GetClientIdOk returns a tuple with the ClientId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientId

`func (o *RevokeOAuthTokenRequest) SetClientId(v string)`

SetClientId sets ClientId field to given value.

### HasClientId

`func (o *RevokeOAuthTokenRequest) HasClientId() bool`

HasClientId returns a boolean if a field has been set.

### SetClientIdNil

`func (o *RevokeOAuthTokenRequest) SetClientIdNil(b bool)`

 SetClientIdNil sets the value for ClientId to be an explicit nil

### UnsetClientId
`func (o *RevokeOAuthTokenRequest) UnsetClientId()`

UnsetClientId ensures that no value is present for ClientId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


