# RegisterOAuthClientRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ClientName** | **string** | Human-readable client application name | 
**RedirectUris** | **[]string** | Array of authorized redirection URI strings for callback verification | 
**GrantTypes** | Pointer to **[]string** | Authorized OAuth grant types for this client | [optional] 
**ResponseTypes** | Pointer to **[]string** | Authorized OAuth response types for this client | [optional] 
**TokenEndpointAuthMethod** | Pointer to **string** | Client authentication method used when calling the token endpoint | [optional] 

## Methods

### NewRegisterOAuthClientRequest

`func NewRegisterOAuthClientRequest(clientName string, redirectUris []string, ) *RegisterOAuthClientRequest`

NewRegisterOAuthClientRequest instantiates a new RegisterOAuthClientRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRegisterOAuthClientRequestWithDefaults

`func NewRegisterOAuthClientRequestWithDefaults() *RegisterOAuthClientRequest`

NewRegisterOAuthClientRequestWithDefaults instantiates a new RegisterOAuthClientRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetClientName

`func (o *RegisterOAuthClientRequest) GetClientName() string`

GetClientName returns the ClientName field if non-nil, zero value otherwise.

### GetClientNameOk

`func (o *RegisterOAuthClientRequest) GetClientNameOk() (*string, bool)`

GetClientNameOk returns a tuple with the ClientName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientName

`func (o *RegisterOAuthClientRequest) SetClientName(v string)`

SetClientName sets ClientName field to given value.


### GetRedirectUris

`func (o *RegisterOAuthClientRequest) GetRedirectUris() []string`

GetRedirectUris returns the RedirectUris field if non-nil, zero value otherwise.

### GetRedirectUrisOk

`func (o *RegisterOAuthClientRequest) GetRedirectUrisOk() (*[]string, bool)`

GetRedirectUrisOk returns a tuple with the RedirectUris field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRedirectUris

`func (o *RegisterOAuthClientRequest) SetRedirectUris(v []string)`

SetRedirectUris sets RedirectUris field to given value.


### GetGrantTypes

`func (o *RegisterOAuthClientRequest) GetGrantTypes() []string`

GetGrantTypes returns the GrantTypes field if non-nil, zero value otherwise.

### GetGrantTypesOk

`func (o *RegisterOAuthClientRequest) GetGrantTypesOk() (*[]string, bool)`

GetGrantTypesOk returns a tuple with the GrantTypes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrantTypes

`func (o *RegisterOAuthClientRequest) SetGrantTypes(v []string)`

SetGrantTypes sets GrantTypes field to given value.

### HasGrantTypes

`func (o *RegisterOAuthClientRequest) HasGrantTypes() bool`

HasGrantTypes returns a boolean if a field has been set.

### GetResponseTypes

`func (o *RegisterOAuthClientRequest) GetResponseTypes() []string`

GetResponseTypes returns the ResponseTypes field if non-nil, zero value otherwise.

### GetResponseTypesOk

`func (o *RegisterOAuthClientRequest) GetResponseTypesOk() (*[]string, bool)`

GetResponseTypesOk returns a tuple with the ResponseTypes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseTypes

`func (o *RegisterOAuthClientRequest) SetResponseTypes(v []string)`

SetResponseTypes sets ResponseTypes field to given value.

### HasResponseTypes

`func (o *RegisterOAuthClientRequest) HasResponseTypes() bool`

HasResponseTypes returns a boolean if a field has been set.

### GetTokenEndpointAuthMethod

`func (o *RegisterOAuthClientRequest) GetTokenEndpointAuthMethod() string`

GetTokenEndpointAuthMethod returns the TokenEndpointAuthMethod field if non-nil, zero value otherwise.

### GetTokenEndpointAuthMethodOk

`func (o *RegisterOAuthClientRequest) GetTokenEndpointAuthMethodOk() (*string, bool)`

GetTokenEndpointAuthMethodOk returns a tuple with the TokenEndpointAuthMethod field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenEndpointAuthMethod

`func (o *RegisterOAuthClientRequest) SetTokenEndpointAuthMethod(v string)`

SetTokenEndpointAuthMethod sets TokenEndpointAuthMethod field to given value.

### HasTokenEndpointAuthMethod

`func (o *RegisterOAuthClientRequest) HasTokenEndpointAuthMethod() bool`

HasTokenEndpointAuthMethod returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


