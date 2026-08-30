# \AuthAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetMyPermissions**](AuthAPI.md#GetMyPermissions) | **Get** /auth/me/permissions | Get current user role permissions
[**GoogleLogin**](AuthAPI.md#GoogleLogin) | **Post** /auth/google-login | Authenticate or register with Google Sign-In
[**GoogleLoginRedirect**](AuthAPI.md#GoogleLoginRedirect) | **Post** /auth/google-login-redirect | Google OAuth callback redirect handler
[**ListSessions**](AuthAPI.md#ListSessions) | **Get** /auth/sessions | List active and historical user sessions
[**Login**](AuthAPI.md#Login) | **Post** /auth/login | Authenticate user with email and password
[**RefreshToken**](AuthAPI.md#RefreshToken) | **Post** /auth/refresh | Rotate refresh token and issue new access token
[**RevokeSession**](AuthAPI.md#RevokeSession) | **Delete** /auth/sessions/{id} | Revoke an active login session
[**SwitchProject**](AuthAPI.md#SwitchProject) | **Post** /auth/switch-project | Switch active project context



## GetMyPermissions

> GetMyPermissions200Response GetMyPermissions(ctx).Execute()

Get current user role permissions



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
	resp, r, err := apiClient.AuthAPI.GetMyPermissions(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.GetMyPermissions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMyPermissions`: GetMyPermissions200Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.GetMyPermissions`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetMyPermissionsRequest struct via the builder pattern


### Return type

[**GetMyPermissions200Response**](GetMyPermissions200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GoogleLogin

> GoogleLogin200Response GoogleLogin(ctx).GoogleLoginRequest(googleLoginRequest).Execute()

Authenticate or register with Google Sign-In



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
	googleLoginRequest := *openapiclient.NewGoogleLoginRequest("eyJhbGciOiJSUzI1NiIsImtpZCI6Ij...") // GoogleLoginRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.GoogleLogin(context.Background()).GoogleLoginRequest(googleLoginRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.GoogleLogin``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GoogleLogin`: GoogleLogin200Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.GoogleLogin`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleLoginRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **googleLoginRequest** | [**GoogleLoginRequest**](GoogleLoginRequest.md) |  | 

### Return type

[**GoogleLogin200Response**](GoogleLogin200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GoogleLoginRedirect

> GoogleLoginRedirect(ctx).Credential(credential).GCsrfToken(gCsrfToken).Execute()

Google OAuth callback redirect handler



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
	credential := "credential_example" // string | Google ID token credential issued by Google Identity Services
	gCsrfToken := "gCsrfToken_example" // string | CSRF token provided by Google Identity Services (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AuthAPI.GoogleLoginRedirect(context.Background()).Credential(credential).GCsrfToken(gCsrfToken).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.GoogleLoginRedirect``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiGoogleLoginRedirectRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **credential** | **string** | Google ID token credential issued by Google Identity Services | 
 **gCsrfToken** | **string** | CSRF token provided by Google Identity Services | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListSessions

> ListSessions200Response ListSessions(ctx).Execute()

List active and historical user sessions



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
	resp, r, err := apiClient.AuthAPI.ListSessions(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.ListSessions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListSessions`: ListSessions200Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.ListSessions`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListSessionsRequest struct via the builder pattern


### Return type

[**ListSessions200Response**](ListSessions200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## Login

> GoogleLogin200Response Login(ctx).LoginRequest(loginRequest).Execute()

Authenticate user with email and password



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
	loginRequest := *openapiclient.NewLoginRequest("demo@omnismith.io", "omni_live_secret_demo_password") // LoginRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.Login(context.Background()).LoginRequest(loginRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.Login``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `Login`: GoogleLogin200Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.Login`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiLoginRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **loginRequest** | [**LoginRequest**](LoginRequest.md) |  | 

### Return type

[**GoogleLogin200Response**](GoogleLogin200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RefreshToken

> RefreshToken200Response RefreshToken(ctx).RefreshTokenRequest(refreshTokenRequest).Execute()

Rotate refresh token and issue new access token



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
	refreshTokenRequest := *openapiclient.NewRefreshTokenRequest("dGhpcyBpcyBhIHNhbXBsZSByZWZyZXNoIHRva2VuIGJhc2U2NA") // RefreshTokenRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.RefreshToken(context.Background()).RefreshTokenRequest(refreshTokenRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.RefreshToken``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RefreshToken`: RefreshToken200Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.RefreshToken`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRefreshTokenRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **refreshTokenRequest** | [**RefreshTokenRequest**](RefreshTokenRequest.md) |  | 

### Return type

[**RefreshToken200Response**](RefreshToken200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RevokeSession

> RevokeSession(ctx, id).Execute()

Revoke an active login session



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
	id := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7a" // string | Unique UUID identifier of the session to revoke

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AuthAPI.RevokeSession(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.RevokeSession``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique UUID identifier of the session to revoke | 

### Other Parameters

Other parameters are passed through a pointer to a apiRevokeSessionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SwitchProject

> SwitchProject200Response SwitchProject(ctx).SwitchProjectRequest(switchProjectRequest).Execute()

Switch active project context



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
	switchProjectRequest := *openapiclient.NewSwitchProjectRequest("018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7a") // SwitchProjectRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AuthAPI.SwitchProject(context.Background()).SwitchProjectRequest(switchProjectRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuthAPI.SwitchProject``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SwitchProject`: SwitchProject200Response
	fmt.Fprintf(os.Stdout, "Response from `AuthAPI.SwitchProject`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSwitchProjectRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **switchProjectRequest** | [**SwitchProjectRequest**](SwitchProjectRequest.md) |  | 

### Return type

[**SwitchProject200Response**](SwitchProject200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

