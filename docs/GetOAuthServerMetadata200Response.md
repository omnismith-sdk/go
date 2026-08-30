# GetOAuthServerMetadata200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Issuer** | Pointer to **string** | Authorization server issuer URL | [optional] 
**AuthorizationEndpoint** | Pointer to **string** | Interactive user consent URL | [optional] 
**TokenEndpoint** | Pointer to **string** | Token issuance endpoint | [optional] 
**RegistrationEndpoint** | Pointer to **string** | Dynamic client registration endpoint (RFC 7591) | [optional] 
**RevocationEndpoint** | Pointer to **string** | Token revocation endpoint (RFC 7009) | [optional] 
**JwksUri** | Pointer to **string** | JSON Web Key Set URL (RFC 7517) | [optional] 
**ResponseTypesSupported** | Pointer to **[]string** |  | [optional] 
**GrantTypesSupported** | Pointer to **[]string** |  | [optional] 
**CodeChallengeMethodsSupported** | Pointer to **[]string** |  | [optional] 
**ScopesSupported** | Pointer to **[]string** |  | [optional] 
**TokenEndpointAuthMethodsSupported** | Pointer to **[]string** |  | [optional] 
**ServiceDocumentation** | Pointer to **string** | URL of documentation | [optional] 
**ClientUri** | Pointer to **string** | URL of the application homepage | [optional] 
**LogoUri** | Pointer to **string** | Logo image URL for the authorization server with transparent background | [optional] 

## Methods

### NewGetOAuthServerMetadata200Response

`func NewGetOAuthServerMetadata200Response() *GetOAuthServerMetadata200Response`

NewGetOAuthServerMetadata200Response instantiates a new GetOAuthServerMetadata200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetOAuthServerMetadata200ResponseWithDefaults

`func NewGetOAuthServerMetadata200ResponseWithDefaults() *GetOAuthServerMetadata200Response`

NewGetOAuthServerMetadata200ResponseWithDefaults instantiates a new GetOAuthServerMetadata200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIssuer

`func (o *GetOAuthServerMetadata200Response) GetIssuer() string`

GetIssuer returns the Issuer field if non-nil, zero value otherwise.

### GetIssuerOk

`func (o *GetOAuthServerMetadata200Response) GetIssuerOk() (*string, bool)`

GetIssuerOk returns a tuple with the Issuer field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssuer

`func (o *GetOAuthServerMetadata200Response) SetIssuer(v string)`

SetIssuer sets Issuer field to given value.

### HasIssuer

`func (o *GetOAuthServerMetadata200Response) HasIssuer() bool`

HasIssuer returns a boolean if a field has been set.

### GetAuthorizationEndpoint

`func (o *GetOAuthServerMetadata200Response) GetAuthorizationEndpoint() string`

GetAuthorizationEndpoint returns the AuthorizationEndpoint field if non-nil, zero value otherwise.

### GetAuthorizationEndpointOk

`func (o *GetOAuthServerMetadata200Response) GetAuthorizationEndpointOk() (*string, bool)`

GetAuthorizationEndpointOk returns a tuple with the AuthorizationEndpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthorizationEndpoint

`func (o *GetOAuthServerMetadata200Response) SetAuthorizationEndpoint(v string)`

SetAuthorizationEndpoint sets AuthorizationEndpoint field to given value.

### HasAuthorizationEndpoint

`func (o *GetOAuthServerMetadata200Response) HasAuthorizationEndpoint() bool`

HasAuthorizationEndpoint returns a boolean if a field has been set.

### GetTokenEndpoint

`func (o *GetOAuthServerMetadata200Response) GetTokenEndpoint() string`

GetTokenEndpoint returns the TokenEndpoint field if non-nil, zero value otherwise.

### GetTokenEndpointOk

`func (o *GetOAuthServerMetadata200Response) GetTokenEndpointOk() (*string, bool)`

GetTokenEndpointOk returns a tuple with the TokenEndpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenEndpoint

`func (o *GetOAuthServerMetadata200Response) SetTokenEndpoint(v string)`

SetTokenEndpoint sets TokenEndpoint field to given value.

### HasTokenEndpoint

`func (o *GetOAuthServerMetadata200Response) HasTokenEndpoint() bool`

HasTokenEndpoint returns a boolean if a field has been set.

### GetRegistrationEndpoint

`func (o *GetOAuthServerMetadata200Response) GetRegistrationEndpoint() string`

GetRegistrationEndpoint returns the RegistrationEndpoint field if non-nil, zero value otherwise.

### GetRegistrationEndpointOk

`func (o *GetOAuthServerMetadata200Response) GetRegistrationEndpointOk() (*string, bool)`

GetRegistrationEndpointOk returns a tuple with the RegistrationEndpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRegistrationEndpoint

`func (o *GetOAuthServerMetadata200Response) SetRegistrationEndpoint(v string)`

SetRegistrationEndpoint sets RegistrationEndpoint field to given value.

### HasRegistrationEndpoint

`func (o *GetOAuthServerMetadata200Response) HasRegistrationEndpoint() bool`

HasRegistrationEndpoint returns a boolean if a field has been set.

### GetRevocationEndpoint

`func (o *GetOAuthServerMetadata200Response) GetRevocationEndpoint() string`

GetRevocationEndpoint returns the RevocationEndpoint field if non-nil, zero value otherwise.

### GetRevocationEndpointOk

`func (o *GetOAuthServerMetadata200Response) GetRevocationEndpointOk() (*string, bool)`

GetRevocationEndpointOk returns a tuple with the RevocationEndpoint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRevocationEndpoint

`func (o *GetOAuthServerMetadata200Response) SetRevocationEndpoint(v string)`

SetRevocationEndpoint sets RevocationEndpoint field to given value.

### HasRevocationEndpoint

`func (o *GetOAuthServerMetadata200Response) HasRevocationEndpoint() bool`

HasRevocationEndpoint returns a boolean if a field has been set.

### GetJwksUri

`func (o *GetOAuthServerMetadata200Response) GetJwksUri() string`

GetJwksUri returns the JwksUri field if non-nil, zero value otherwise.

### GetJwksUriOk

`func (o *GetOAuthServerMetadata200Response) GetJwksUriOk() (*string, bool)`

GetJwksUriOk returns a tuple with the JwksUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetJwksUri

`func (o *GetOAuthServerMetadata200Response) SetJwksUri(v string)`

SetJwksUri sets JwksUri field to given value.

### HasJwksUri

`func (o *GetOAuthServerMetadata200Response) HasJwksUri() bool`

HasJwksUri returns a boolean if a field has been set.

### GetResponseTypesSupported

`func (o *GetOAuthServerMetadata200Response) GetResponseTypesSupported() []string`

GetResponseTypesSupported returns the ResponseTypesSupported field if non-nil, zero value otherwise.

### GetResponseTypesSupportedOk

`func (o *GetOAuthServerMetadata200Response) GetResponseTypesSupportedOk() (*[]string, bool)`

GetResponseTypesSupportedOk returns a tuple with the ResponseTypesSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResponseTypesSupported

`func (o *GetOAuthServerMetadata200Response) SetResponseTypesSupported(v []string)`

SetResponseTypesSupported sets ResponseTypesSupported field to given value.

### HasResponseTypesSupported

`func (o *GetOAuthServerMetadata200Response) HasResponseTypesSupported() bool`

HasResponseTypesSupported returns a boolean if a field has been set.

### GetGrantTypesSupported

`func (o *GetOAuthServerMetadata200Response) GetGrantTypesSupported() []string`

GetGrantTypesSupported returns the GrantTypesSupported field if non-nil, zero value otherwise.

### GetGrantTypesSupportedOk

`func (o *GetOAuthServerMetadata200Response) GetGrantTypesSupportedOk() (*[]string, bool)`

GetGrantTypesSupportedOk returns a tuple with the GrantTypesSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrantTypesSupported

`func (o *GetOAuthServerMetadata200Response) SetGrantTypesSupported(v []string)`

SetGrantTypesSupported sets GrantTypesSupported field to given value.

### HasGrantTypesSupported

`func (o *GetOAuthServerMetadata200Response) HasGrantTypesSupported() bool`

HasGrantTypesSupported returns a boolean if a field has been set.

### GetCodeChallengeMethodsSupported

`func (o *GetOAuthServerMetadata200Response) GetCodeChallengeMethodsSupported() []string`

GetCodeChallengeMethodsSupported returns the CodeChallengeMethodsSupported field if non-nil, zero value otherwise.

### GetCodeChallengeMethodsSupportedOk

`func (o *GetOAuthServerMetadata200Response) GetCodeChallengeMethodsSupportedOk() (*[]string, bool)`

GetCodeChallengeMethodsSupportedOk returns a tuple with the CodeChallengeMethodsSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCodeChallengeMethodsSupported

`func (o *GetOAuthServerMetadata200Response) SetCodeChallengeMethodsSupported(v []string)`

SetCodeChallengeMethodsSupported sets CodeChallengeMethodsSupported field to given value.

### HasCodeChallengeMethodsSupported

`func (o *GetOAuthServerMetadata200Response) HasCodeChallengeMethodsSupported() bool`

HasCodeChallengeMethodsSupported returns a boolean if a field has been set.

### GetScopesSupported

`func (o *GetOAuthServerMetadata200Response) GetScopesSupported() []string`

GetScopesSupported returns the ScopesSupported field if non-nil, zero value otherwise.

### GetScopesSupportedOk

`func (o *GetOAuthServerMetadata200Response) GetScopesSupportedOk() (*[]string, bool)`

GetScopesSupportedOk returns a tuple with the ScopesSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetScopesSupported

`func (o *GetOAuthServerMetadata200Response) SetScopesSupported(v []string)`

SetScopesSupported sets ScopesSupported field to given value.

### HasScopesSupported

`func (o *GetOAuthServerMetadata200Response) HasScopesSupported() bool`

HasScopesSupported returns a boolean if a field has been set.

### GetTokenEndpointAuthMethodsSupported

`func (o *GetOAuthServerMetadata200Response) GetTokenEndpointAuthMethodsSupported() []string`

GetTokenEndpointAuthMethodsSupported returns the TokenEndpointAuthMethodsSupported field if non-nil, zero value otherwise.

### GetTokenEndpointAuthMethodsSupportedOk

`func (o *GetOAuthServerMetadata200Response) GetTokenEndpointAuthMethodsSupportedOk() (*[]string, bool)`

GetTokenEndpointAuthMethodsSupportedOk returns a tuple with the TokenEndpointAuthMethodsSupported field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTokenEndpointAuthMethodsSupported

`func (o *GetOAuthServerMetadata200Response) SetTokenEndpointAuthMethodsSupported(v []string)`

SetTokenEndpointAuthMethodsSupported sets TokenEndpointAuthMethodsSupported field to given value.

### HasTokenEndpointAuthMethodsSupported

`func (o *GetOAuthServerMetadata200Response) HasTokenEndpointAuthMethodsSupported() bool`

HasTokenEndpointAuthMethodsSupported returns a boolean if a field has been set.

### GetServiceDocumentation

`func (o *GetOAuthServerMetadata200Response) GetServiceDocumentation() string`

GetServiceDocumentation returns the ServiceDocumentation field if non-nil, zero value otherwise.

### GetServiceDocumentationOk

`func (o *GetOAuthServerMetadata200Response) GetServiceDocumentationOk() (*string, bool)`

GetServiceDocumentationOk returns a tuple with the ServiceDocumentation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetServiceDocumentation

`func (o *GetOAuthServerMetadata200Response) SetServiceDocumentation(v string)`

SetServiceDocumentation sets ServiceDocumentation field to given value.

### HasServiceDocumentation

`func (o *GetOAuthServerMetadata200Response) HasServiceDocumentation() bool`

HasServiceDocumentation returns a boolean if a field has been set.

### GetClientUri

`func (o *GetOAuthServerMetadata200Response) GetClientUri() string`

GetClientUri returns the ClientUri field if non-nil, zero value otherwise.

### GetClientUriOk

`func (o *GetOAuthServerMetadata200Response) GetClientUriOk() (*string, bool)`

GetClientUriOk returns a tuple with the ClientUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetClientUri

`func (o *GetOAuthServerMetadata200Response) SetClientUri(v string)`

SetClientUri sets ClientUri field to given value.

### HasClientUri

`func (o *GetOAuthServerMetadata200Response) HasClientUri() bool`

HasClientUri returns a boolean if a field has been set.

### GetLogoUri

`func (o *GetOAuthServerMetadata200Response) GetLogoUri() string`

GetLogoUri returns the LogoUri field if non-nil, zero value otherwise.

### GetLogoUriOk

`func (o *GetOAuthServerMetadata200Response) GetLogoUriOk() (*string, bool)`

GetLogoUriOk returns a tuple with the LogoUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLogoUri

`func (o *GetOAuthServerMetadata200Response) SetLogoUri(v string)`

SetLogoUri sets LogoUri field to given value.

### HasLogoUri

`func (o *GetOAuthServerMetadata200Response) HasLogoUri() bool`

HasLogoUri returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


