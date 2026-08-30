# RefreshToken200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AccessToken** | Pointer to **string** | New JWT access token for authenticating Bearer requests | [optional] 
**ExpiresAt** | Pointer to **int32** | Unix timestamp when the access token expires | [optional] 
**RefreshToken** | Pointer to **string** | New rotated refresh token for future refreshes | [optional] 
**RefreshExpiresAt** | Pointer to **int32** | Unix timestamp when the new refresh token expires | [optional] 

## Methods

### NewRefreshToken200Response

`func NewRefreshToken200Response() *RefreshToken200Response`

NewRefreshToken200Response instantiates a new RefreshToken200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRefreshToken200ResponseWithDefaults

`func NewRefreshToken200ResponseWithDefaults() *RefreshToken200Response`

NewRefreshToken200ResponseWithDefaults instantiates a new RefreshToken200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAccessToken

`func (o *RefreshToken200Response) GetAccessToken() string`

GetAccessToken returns the AccessToken field if non-nil, zero value otherwise.

### GetAccessTokenOk

`func (o *RefreshToken200Response) GetAccessTokenOk() (*string, bool)`

GetAccessTokenOk returns a tuple with the AccessToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessToken

`func (o *RefreshToken200Response) SetAccessToken(v string)`

SetAccessToken sets AccessToken field to given value.

### HasAccessToken

`func (o *RefreshToken200Response) HasAccessToken() bool`

HasAccessToken returns a boolean if a field has been set.

### GetExpiresAt

`func (o *RefreshToken200Response) GetExpiresAt() int32`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *RefreshToken200Response) GetExpiresAtOk() (*int32, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *RefreshToken200Response) SetExpiresAt(v int32)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *RefreshToken200Response) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### GetRefreshToken

`func (o *RefreshToken200Response) GetRefreshToken() string`

GetRefreshToken returns the RefreshToken field if non-nil, zero value otherwise.

### GetRefreshTokenOk

`func (o *RefreshToken200Response) GetRefreshTokenOk() (*string, bool)`

GetRefreshTokenOk returns a tuple with the RefreshToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRefreshToken

`func (o *RefreshToken200Response) SetRefreshToken(v string)`

SetRefreshToken sets RefreshToken field to given value.

### HasRefreshToken

`func (o *RefreshToken200Response) HasRefreshToken() bool`

HasRefreshToken returns a boolean if a field has been set.

### GetRefreshExpiresAt

`func (o *RefreshToken200Response) GetRefreshExpiresAt() int32`

GetRefreshExpiresAt returns the RefreshExpiresAt field if non-nil, zero value otherwise.

### GetRefreshExpiresAtOk

`func (o *RefreshToken200Response) GetRefreshExpiresAtOk() (*int32, bool)`

GetRefreshExpiresAtOk returns a tuple with the RefreshExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRefreshExpiresAt

`func (o *RefreshToken200Response) SetRefreshExpiresAt(v int32)`

SetRefreshExpiresAt sets RefreshExpiresAt field to given value.

### HasRefreshExpiresAt

`func (o *RefreshToken200Response) HasRefreshExpiresAt() bool`

HasRefreshExpiresAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


