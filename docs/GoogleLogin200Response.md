# GoogleLogin200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccessToken** | Pointer to **string** | JWT access token for authenticating Bearer requests | [optional] 
**ExpiresAt** | Pointer to **int32** | Unix timestamp when the access token expires | [optional] 
**RefreshToken** | Pointer to **string** | Refresh token for rotating access tokens | [optional] 
**RefreshExpiresAt** | Pointer to **int32** | Unix timestamp when the refresh token expires | [optional] 

## Methods

### NewGoogleLogin200Response

`func NewGoogleLogin200Response() *GoogleLogin200Response`

NewGoogleLogin200Response instantiates a new GoogleLogin200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGoogleLogin200ResponseWithDefaults

`func NewGoogleLogin200ResponseWithDefaults() *GoogleLogin200Response`

NewGoogleLogin200ResponseWithDefaults instantiates a new GoogleLogin200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccessToken

`func (o *GoogleLogin200Response) GetAccessToken() string`

GetAccessToken returns the AccessToken field if non-nil, zero value otherwise.

### GetAccessTokenOk

`func (o *GoogleLogin200Response) GetAccessTokenOk() (*string, bool)`

GetAccessTokenOk returns a tuple with the AccessToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessToken

`func (o *GoogleLogin200Response) SetAccessToken(v string)`

SetAccessToken sets AccessToken field to given value.

### HasAccessToken

`func (o *GoogleLogin200Response) HasAccessToken() bool`

HasAccessToken returns a boolean if a field has been set.

### GetExpiresAt

`func (o *GoogleLogin200Response) GetExpiresAt() int32`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *GoogleLogin200Response) GetExpiresAtOk() (*int32, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *GoogleLogin200Response) SetExpiresAt(v int32)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *GoogleLogin200Response) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### GetRefreshToken

`func (o *GoogleLogin200Response) GetRefreshToken() string`

GetRefreshToken returns the RefreshToken field if non-nil, zero value otherwise.

### GetRefreshTokenOk

`func (o *GoogleLogin200Response) GetRefreshTokenOk() (*string, bool)`

GetRefreshTokenOk returns a tuple with the RefreshToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRefreshToken

`func (o *GoogleLogin200Response) SetRefreshToken(v string)`

SetRefreshToken sets RefreshToken field to given value.

### HasRefreshToken

`func (o *GoogleLogin200Response) HasRefreshToken() bool`

HasRefreshToken returns a boolean if a field has been set.

### GetRefreshExpiresAt

`func (o *GoogleLogin200Response) GetRefreshExpiresAt() int32`

GetRefreshExpiresAt returns the RefreshExpiresAt field if non-nil, zero value otherwise.

### GetRefreshExpiresAtOk

`func (o *GoogleLogin200Response) GetRefreshExpiresAtOk() (*int32, bool)`

GetRefreshExpiresAtOk returns a tuple with the RefreshExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRefreshExpiresAt

`func (o *GoogleLogin200Response) SetRefreshExpiresAt(v int32)`

SetRefreshExpiresAt sets RefreshExpiresAt field to given value.

### HasRefreshExpiresAt

`func (o *GoogleLogin200Response) HasRefreshExpiresAt() bool`

HasRefreshExpiresAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


