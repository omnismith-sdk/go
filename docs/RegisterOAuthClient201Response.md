# RegisterOAuthClient201Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ClientId** | Pointer to **string** | Generated unique client identifier | [optional] 
**ClientSecret** | Pointer to **NullableString** | Client secret for confidential clients (null for public clients) | [optional] 
**ClientName** | Pointer to **string** | Registered application name | [optional] 
**RedirectUris** | Pointer to **[]string** | Authorized redirection URIs | [optional] 
**GrantTypes** | Pointer to **[]string** | Permitted grant types | [optional] 
**ResponseTypes** | Pointer to **[]string** | Permitted response types | [optional] 
**TokenEndpointAuthMethod** | Pointer to **string** | Authentication method required at token endpoint | [optional] 
**ClientIdIssuedAt** | Pointer to **int32** | Unix timestamp when client was registered | [optional] 

## Methods

### NewRegisterOAuthClient201Response

`func NewRegisterOAuthClient201Response() *RegisterOAuthClient201Response`

NewRegisterOAuthClient201Response instantiates a new RegisterOAuthClient201Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRegisterOAuthClient201ResponseWithDefaults

`func NewRegisterOAuthClient201ResponseWithDefaults() *RegisterOAuthClient201Response`

NewRegisterOAuthClient201ResponseWithDefaults instantiates a new RegisterOAuthClient201Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetClientId

`func (o *RegisterOAuthClient201Response) GetClientId() string`

GetClientId returns the ClientId field if non-nil, zero value otherwise.

### GetClientIdOk

`func (o *RegisterOAuthClient201Response) GetClientIdOk() (*string, bool)`

GetClientIdOk returns a tuple with the ClientId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientId

`func (o *RegisterOAuthClient201Response) SetClientId(v string)`

SetClientId sets ClientId field to given value.

### HasClientId

`func (o *RegisterOAuthClient201Response) HasClientId() bool`

HasClientId returns a boolean if a field has been set.

### GetClientSecret

`func (o *RegisterOAuthClient201Response) GetClientSecret() string`

GetClientSecret returns the ClientSecret field if non-nil, zero value otherwise.

### GetClientSecretOk

`func (o *RegisterOAuthClient201Response) GetClientSecretOk() (*string, bool)`

GetClientSecretOk returns a tuple with the ClientSecret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientSecret

`func (o *RegisterOAuthClient201Response) SetClientSecret(v string)`

SetClientSecret sets ClientSecret field to given value.

### HasClientSecret

`func (o *RegisterOAuthClient201Response) HasClientSecret() bool`

HasClientSecret returns a boolean if a field has been set.

### SetClientSecretNil

`func (o *RegisterOAuthClient201Response) SetClientSecretNil(b bool)`

 SetClientSecretNil sets the value for ClientSecret to be an explicit nil

### UnsetClientSecret
`func (o *RegisterOAuthClient201Response) UnsetClientSecret()`

UnsetClientSecret ensures that no value is present for ClientSecret, not even an explicit nil
### GetClientName

`func (o *RegisterOAuthClient201Response) GetClientName() string`

GetClientName returns the ClientName field if non-nil, zero value otherwise.

### GetClientNameOk

`func (o *RegisterOAuthClient201Response) GetClientNameOk() (*string, bool)`

GetClientNameOk returns a tuple with the ClientName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientName

`func (o *RegisterOAuthClient201Response) SetClientName(v string)`

SetClientName sets ClientName field to given value.

### HasClientName

`func (o *RegisterOAuthClient201Response) HasClientName() bool`

HasClientName returns a boolean if a field has been set.

### GetRedirectUris

`func (o *RegisterOAuthClient201Response) GetRedirectUris() []string`

GetRedirectUris returns the RedirectUris field if non-nil, zero value otherwise.

### GetRedirectUrisOk

`func (o *RegisterOAuthClient201Response) GetRedirectUrisOk() (*[]string, bool)`

GetRedirectUrisOk returns a tuple with the RedirectUris field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRedirectUris

`func (o *RegisterOAuthClient201Response) SetRedirectUris(v []string)`

SetRedirectUris sets RedirectUris field to given value.

### HasRedirectUris

`func (o *RegisterOAuthClient201Response) HasRedirectUris() bool`

HasRedirectUris returns a boolean if a field has been set.

### GetGrantTypes

`func (o *RegisterOAuthClient201Response) GetGrantTypes() []string`

GetGrantTypes returns the GrantTypes field if non-nil, zero value otherwise.

### GetGrantTypesOk

`func (o *RegisterOAuthClient201Response) GetGrantTypesOk() (*[]string, bool)`

GetGrantTypesOk returns a tuple with the GrantTypes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrantTypes

`func (o *RegisterOAuthClient201Response) SetGrantTypes(v []string)`

SetGrantTypes sets GrantTypes field to given value.

### HasGrantTypes

`func (o *RegisterOAuthClient201Response) HasGrantTypes() bool`

HasGrantTypes returns a boolean if a field has been set.

### GetResponseTypes

`func (o *RegisterOAuthClient201Response) GetResponseTypes() []string`

GetResponseTypes returns the ResponseTypes field if non-nil, zero value otherwise.

### GetResponseTypesOk

`func (o *RegisterOAuthClient201Response) GetResponseTypesOk() (*[]string, bool)`

GetResponseTypesOk returns a tuple with the ResponseTypes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseTypes

`func (o *RegisterOAuthClient201Response) SetResponseTypes(v []string)`

SetResponseTypes sets ResponseTypes field to given value.

### HasResponseTypes

`func (o *RegisterOAuthClient201Response) HasResponseTypes() bool`

HasResponseTypes returns a boolean if a field has been set.

### GetTokenEndpointAuthMethod

`func (o *RegisterOAuthClient201Response) GetTokenEndpointAuthMethod() string`

GetTokenEndpointAuthMethod returns the TokenEndpointAuthMethod field if non-nil, zero value otherwise.

### GetTokenEndpointAuthMethodOk

`func (o *RegisterOAuthClient201Response) GetTokenEndpointAuthMethodOk() (*string, bool)`

GetTokenEndpointAuthMethodOk returns a tuple with the TokenEndpointAuthMethod field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenEndpointAuthMethod

`func (o *RegisterOAuthClient201Response) SetTokenEndpointAuthMethod(v string)`

SetTokenEndpointAuthMethod sets TokenEndpointAuthMethod field to given value.

### HasTokenEndpointAuthMethod

`func (o *RegisterOAuthClient201Response) HasTokenEndpointAuthMethod() bool`

HasTokenEndpointAuthMethod returns a boolean if a field has been set.

### GetClientIdIssuedAt

`func (o *RegisterOAuthClient201Response) GetClientIdIssuedAt() int32`

GetClientIdIssuedAt returns the ClientIdIssuedAt field if non-nil, zero value otherwise.

### GetClientIdIssuedAtOk

`func (o *RegisterOAuthClient201Response) GetClientIdIssuedAtOk() (*int32, bool)`

GetClientIdIssuedAtOk returns a tuple with the ClientIdIssuedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientIdIssuedAt

`func (o *RegisterOAuthClient201Response) SetClientIdIssuedAt(v int32)`

SetClientIdIssuedAt sets ClientIdIssuedAt field to given value.

### HasClientIdIssuedAt

`func (o *RegisterOAuthClient201Response) HasClientIdIssuedAt() bool`

HasClientIdIssuedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


