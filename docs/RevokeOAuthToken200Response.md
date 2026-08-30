# RevokeOAuthToken200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Revoked** | Pointer to **bool** | Whether the token is no longer active | [optional] 

## Methods

### NewRevokeOAuthToken200Response

`func NewRevokeOAuthToken200Response() *RevokeOAuthToken200Response`

NewRevokeOAuthToken200Response instantiates a new RevokeOAuthToken200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRevokeOAuthToken200ResponseWithDefaults

`func NewRevokeOAuthToken200ResponseWithDefaults() *RevokeOAuthToken200Response`

NewRevokeOAuthToken200ResponseWithDefaults instantiates a new RevokeOAuthToken200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetRevoked

`func (o *RevokeOAuthToken200Response) GetRevoked() bool`

GetRevoked returns the Revoked field if non-nil, zero value otherwise.

### GetRevokedOk

`func (o *RevokeOAuthToken200Response) GetRevokedOk() (*bool, bool)`

GetRevokedOk returns a tuple with the Revoked field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRevoked

`func (o *RevokeOAuthToken200Response) SetRevoked(v bool)`

SetRevoked sets Revoked field to given value.

### HasRevoked

`func (o *RevokeOAuthToken200Response) HasRevoked() bool`

HasRevoked returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


