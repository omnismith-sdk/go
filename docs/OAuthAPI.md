# \OAuthAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ApproveOAuthAuthorization**](OAuthAPI.md#ApproveOAuthAuthorization) | **Post** /oauth/authorize/approve | Approve OAuth Authorization Consent
[**ExchangeOAuthToken**](OAuthAPI.md#ExchangeOAuthToken) | **Post** /oauth/token | Exchange OAuth 2.0 Token
[**GetJwks**](OAuthAPI.md#GetJwks) | **Get** /.well-known/jwks.json | Get JSON Web Key Set
[**GetOAuthAuthorizeInfo**](OAuthAPI.md#GetOAuthAuthorizeInfo) | **Get** /oauth/authorize/info | Get OAuth Authorization Consent Screen Info
[**GetOAuthServerMetadata**](OAuthAPI.md#GetOAuthServerMetadata) | **Get** /.well-known/oauth-authorization-server | Get OAuth Authorization Server Metadata
[**RegisterOAuthClient**](OAuthAPI.md#RegisterOAuthClient) | **Post** /oauth/register | Register Dynamic OAuth Client
[**RevokeOAuthToken**](OAuthAPI.md#RevokeOAuthToken) | **Post** /oauth/revoke | Revoke OAuth Token



## ApproveOAuthAuthorization

> ApproveOAuthAuthorization200Response ApproveOAuthAuthorization(ctx).ApproveOAuthAuthorizationRequest(approveOAuthAuthorizationRequest).Execute()

Approve OAuth Authorization Consent



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/omnismith-sdk/go"
)

func main() {
	approveOAuthAuthorizationRequest := *openapiclient.NewApproveOAuthAuthorizationRequest("omni_client_0195a8f2c3e471238000000000000001", "https://claude.ai/api/mcp/oauth_callback", "0195a8f2-c3e4-7123-8000-000000000001", "E9Melhoa2OwvFrGMTJguCH5SZXgk6uKUaz312M20O48") // ApproveOAuthAuthorizationRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.ApproveOAuthAuthorization(context.Background()).ApproveOAuthAuthorizationRequest(approveOAuthAuthorizationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.ApproveOAuthAuthorization``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ApproveOAuthAuthorization`: ApproveOAuthAuthorization200Response
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.ApproveOAuthAuthorization`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiApproveOAuthAuthorizationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **approveOAuthAuthorizationRequest** | [**ApproveOAuthAuthorizationRequest**](ApproveOAuthAuthorizationRequest.md) |  | 

### Return type

[**ApproveOAuthAuthorization200Response**](ApproveOAuthAuthorization200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExchangeOAuthToken

> ExchangeOAuthToken200Response ExchangeOAuthToken(ctx).OAuthTokenRequest(oAuthTokenRequest).Execute()

Exchange OAuth 2.0 Token



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/omnismith-sdk/go"
)

func main() {
	oAuthTokenRequest := *openapiclient.NewOAuthTokenRequest("authorization_code") // OAuthTokenRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.ExchangeOAuthToken(context.Background()).OAuthTokenRequest(oAuthTokenRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.ExchangeOAuthToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExchangeOAuthToken`: ExchangeOAuthToken200Response
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.ExchangeOAuthToken`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiExchangeOAuthTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **oAuthTokenRequest** | [**OAuthTokenRequest**](OAuthTokenRequest.md) |  | 

### Return type

[**ExchangeOAuthToken200Response**](ExchangeOAuthToken200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetJwks

> GetJwks200Response GetJwks(ctx).Execute()

Get JSON Web Key Set



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/omnismith-sdk/go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.GetJwks(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.GetJwks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetJwks`: GetJwks200Response
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.GetJwks`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetJwksRequest struct via the builder pattern


### Return type

[**GetJwks200Response**](GetJwks200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetOAuthAuthorizeInfo

> GetOAuthAuthorizeInfo200Response GetOAuthAuthorizeInfo(ctx).ClientId(clientId).RedirectUri(redirectUri).ResponseType(responseType).Scope(scope).CodeChallenge(codeChallenge).CodeChallengeMethod(codeChallengeMethod).State(state).Execute()

Get OAuth Authorization Consent Screen Info



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/omnismith-sdk/go"
)

func main() {
	clientId := "omni_client_0195a8f2c3e471238000000000000001" // string | Registered OAuth client identifier
	redirectUri := "https://claude.ai/api/mcp/oauth_callback" // string | Target redirection URI matching registered client URIs
	responseType := "code" // string | OAuth response type (must be \"code\") (default to "code")
	scope := "omnismith:all" // string | Space-delimited requested scopes (optional)
	codeChallenge := "E9Melhoa2OwvFrGMTJguCH5SZXgk6uKUaz312M20O48" // string | PKCE code challenge string (RFC 7636) (optional)
	codeChallengeMethod := "S256" // string | PKCE code challenge transformation method (optional) (default to "S256")
	state := "state_xyz123" // string | Opaque client state parameter for CSRF mitigation (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.GetOAuthAuthorizeInfo(context.Background()).ClientId(clientId).RedirectUri(redirectUri).ResponseType(responseType).Scope(scope).CodeChallenge(codeChallenge).CodeChallengeMethod(codeChallengeMethod).State(state).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.GetOAuthAuthorizeInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetOAuthAuthorizeInfo`: GetOAuthAuthorizeInfo200Response
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.GetOAuthAuthorizeInfo`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGetOAuthAuthorizeInfoRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **clientId** | **string** | Registered OAuth client identifier | 
 **redirectUri** | **string** | Target redirection URI matching registered client URIs | 
 **responseType** | **string** | OAuth response type (must be \&quot;code\&quot;) | [default to &quot;code&quot;]
 **scope** | **string** | Space-delimited requested scopes | 
 **codeChallenge** | **string** | PKCE code challenge string (RFC 7636) | 
 **codeChallengeMethod** | **string** | PKCE code challenge transformation method | [default to &quot;S256&quot;]
 **state** | **string** | Opaque client state parameter for CSRF mitigation | 

### Return type

[**GetOAuthAuthorizeInfo200Response**](GetOAuthAuthorizeInfo200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetOAuthServerMetadata

> GetOAuthServerMetadata200Response GetOAuthServerMetadata(ctx).Execute()

Get OAuth Authorization Server Metadata



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/omnismith-sdk/go"
)

func main() {

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.GetOAuthServerMetadata(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.GetOAuthServerMetadata``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetOAuthServerMetadata`: GetOAuthServerMetadata200Response
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.GetOAuthServerMetadata`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetOAuthServerMetadataRequest struct via the builder pattern


### Return type

[**GetOAuthServerMetadata200Response**](GetOAuthServerMetadata200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RegisterOAuthClient

> RegisterOAuthClient201Response RegisterOAuthClient(ctx).RegisterOAuthClientRequest(registerOAuthClientRequest).Execute()

Register Dynamic OAuth Client



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/omnismith-sdk/go"
)

func main() {
	registerOAuthClientRequest := *openapiclient.NewRegisterOAuthClientRequest("Claude Desktop", []string{"RedirectUris_example"}) // RegisterOAuthClientRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.RegisterOAuthClient(context.Background()).RegisterOAuthClientRequest(registerOAuthClientRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.RegisterOAuthClient``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RegisterOAuthClient`: RegisterOAuthClient201Response
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.RegisterOAuthClient`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRegisterOAuthClientRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registerOAuthClientRequest** | [**RegisterOAuthClientRequest**](RegisterOAuthClientRequest.md) |  | 

### Return type

[**RegisterOAuthClient201Response**](RegisterOAuthClient201Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RevokeOAuthToken

> RevokeOAuthToken200Response RevokeOAuthToken(ctx).RevokeOAuthTokenRequest(revokeOAuthTokenRequest).Execute()

Revoke OAuth Token



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/omnismith-sdk/go"
)

func main() {
	revokeOAuthTokenRequest := *openapiclient.NewRevokeOAuthTokenRequest("omni_ort_0195a8f2c3e471238000000000000004") // RevokeOAuthTokenRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.OAuthAPI.RevokeOAuthToken(context.Background()).RevokeOAuthTokenRequest(revokeOAuthTokenRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `OAuthAPI.RevokeOAuthToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RevokeOAuthToken`: RevokeOAuthToken200Response
	fmt.Fprintf(os.Stdout, "Response from `OAuthAPI.RevokeOAuthToken`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRevokeOAuthTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **revokeOAuthTokenRequest** | [**RevokeOAuthTokenRequest**](RevokeOAuthTokenRequest.md) |  | 

### Return type

[**RevokeOAuthToken200Response**](RevokeOAuthToken200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

