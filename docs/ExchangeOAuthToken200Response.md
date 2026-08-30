# ExchangeOAuthToken200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccessToken** | Pointer to **string** | RS256 JWT access token | [optional] 
**TokenType** | Pointer to **string** | Token type (Bearer) | [optional] 
**ExpiresIn** | Pointer to **int32** | Access token lifetime in seconds | [optional] 
**RefreshToken** | Pointer to **NullableString** | Rotating refresh token for renewing credentials | [optional] 
**Scope** | Pointer to **string** | Granted scope strings | [optional] 

## Methods

### NewExchangeOAuthToken200Response

`func NewExchangeOAuthToken200Response() *ExchangeOAuthToken200Response`

NewExchangeOAuthToken200Response instantiates a new ExchangeOAuthToken200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExchangeOAuthToken200ResponseWithDefaults

`func NewExchangeOAuthToken200ResponseWithDefaults() *ExchangeOAuthToken200Response`

NewExchangeOAuthToken200ResponseWithDefaults instantiates a new ExchangeOAuthToken200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccessToken

`func (o *ExchangeOAuthToken200Response) GetAccessToken() string`

GetAccessToken returns the AccessToken field if non-nil, zero value otherwise.

### GetAccessTokenOk

`func (o *ExchangeOAuthToken200Response) GetAccessTokenOk() (*string, bool)`

GetAccessTokenOk returns a tuple with the AccessToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessToken

`func (o *ExchangeOAuthToken200Response) SetAccessToken(v string)`

SetAccessToken sets AccessToken field to given value.

### HasAccessToken

`func (o *ExchangeOAuthToken200Response) HasAccessToken() bool`

HasAccessToken returns a boolean if a field has been set.

### GetTokenType

`func (o *ExchangeOAuthToken200Response) GetTokenType() string`

GetTokenType returns the TokenType field if non-nil, zero value otherwise.

### GetTokenTypeOk

`func (o *ExchangeOAuthToken200Response) GetTokenTypeOk() (*string, bool)`

GetTokenTypeOk returns a tuple with the TokenType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenType

`func (o *ExchangeOAuthToken200Response) SetTokenType(v string)`

SetTokenType sets TokenType field to given value.

### HasTokenType

`func (o *ExchangeOAuthToken200Response) HasTokenType() bool`

HasTokenType returns a boolean if a field has been set.

### GetExpiresIn

`func (o *ExchangeOAuthToken200Response) GetExpiresIn() int32`

GetExpiresIn returns the ExpiresIn field if non-nil, zero value otherwise.

### GetExpiresInOk

`func (o *ExchangeOAuthToken200Response) GetExpiresInOk() (*int32, bool)`

GetExpiresInOk returns a tuple with the ExpiresIn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresIn

`func (o *ExchangeOAuthToken200Response) SetExpiresIn(v int32)`

SetExpiresIn sets ExpiresIn field to given value.

### HasExpiresIn

`func (o *ExchangeOAuthToken200Response) HasExpiresIn() bool`

HasExpiresIn returns a boolean if a field has been set.

### GetRefreshToken

`func (o *ExchangeOAuthToken200Response) GetRefreshToken() string`

GetRefreshToken returns the RefreshToken field if non-nil, zero value otherwise.

### GetRefreshTokenOk

`func (o *ExchangeOAuthToken200Response) GetRefreshTokenOk() (*string, bool)`

GetRefreshTokenOk returns a tuple with the RefreshToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRefreshToken

`func (o *ExchangeOAuthToken200Response) SetRefreshToken(v string)`

SetRefreshToken sets RefreshToken field to given value.

### HasRefreshToken

`func (o *ExchangeOAuthToken200Response) HasRefreshToken() bool`

HasRefreshToken returns a boolean if a field has been set.

### SetRefreshTokenNil

`func (o *ExchangeOAuthToken200Response) SetRefreshTokenNil(b bool)`

 SetRefreshTokenNil sets the value for RefreshToken to be an explicit nil

### UnsetRefreshToken
`func (o *ExchangeOAuthToken200Response) UnsetRefreshToken()`

UnsetRefreshToken ensures that no value is present for RefreshToken, not even an explicit nil
### GetScope

`func (o *ExchangeOAuthToken200Response) GetScope() string`

GetScope returns the Scope field if non-nil, zero value otherwise.

### GetScopeOk

`func (o *ExchangeOAuthToken200Response) GetScopeOk() (*string, bool)`

GetScopeOk returns a tuple with the Scope field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScope

`func (o *ExchangeOAuthToken200Response) SetScope(v string)`

SetScope sets Scope field to given value.

### HasScope

`func (o *ExchangeOAuthToken200Response) HasScope() bool`

HasScope returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


