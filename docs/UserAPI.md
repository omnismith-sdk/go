# \UserAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ConfirmUserEmail**](UserAPI.md#ConfirmUserEmail) | **Get** /users/confirm-email | Confirm a user&#39;s email address using a confirmation token
[**RegisterUser**](UserAPI.md#RegisterUser) | **Post** /users/register | Register a new user
[**ResendConfirmationEmail**](UserAPI.md#ResendConfirmationEmail) | **Post** /users/resend-confirmation | Resend the email confirmation link



## ConfirmUserEmail

> ConfirmUserEmail200Response ConfirmUserEmail(ctx).Token(token).Execute()

Confirm a user's email address using a confirmation token

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	token := "token_example" // string | The email confirmation token

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UserAPI.ConfirmUserEmail(context.Background()).Token(token).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UserAPI.ConfirmUserEmail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ConfirmUserEmail`: ConfirmUserEmail200Response
	fmt.Fprintf(os.Stdout, "Response from `UserAPI.ConfirmUserEmail`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiConfirmUserEmailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **string** | The email confirmation token | 

### Return type

[**ConfirmUserEmail200Response**](ConfirmUserEmail200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RegisterUser

> CreateAttributeItem201Response RegisterUser(ctx).RegisterUserRequest(registerUserRequest).Execute()

Register a new user

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	registerUserRequest := *openapiclient.NewRegisterUserRequest("user@example.com", "securePassword123") // RegisterUserRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UserAPI.RegisterUser(context.Background()).RegisterUserRequest(registerUserRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UserAPI.RegisterUser``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RegisterUser`: CreateAttributeItem201Response
	fmt.Fprintf(os.Stdout, "Response from `UserAPI.RegisterUser`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRegisterUserRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registerUserRequest** | [**RegisterUserRequest**](RegisterUserRequest.md) |  | 

### Return type

[**CreateAttributeItem201Response**](CreateAttributeItem201Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ResendConfirmationEmail

> ResendConfirmationEmail200Response ResendConfirmationEmail(ctx).ResendConfirmationEmailRequest(resendConfirmationEmailRequest).Execute()

Resend the email confirmation link

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	resendConfirmationEmailRequest := *openapiclient.NewResendConfirmationEmailRequest("user@example.com") // ResendConfirmationEmailRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.UserAPI.ResendConfirmationEmail(context.Background()).ResendConfirmationEmailRequest(resendConfirmationEmailRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `UserAPI.ResendConfirmationEmail``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ResendConfirmationEmail`: ResendConfirmationEmail200Response
	fmt.Fprintf(os.Stdout, "Response from `UserAPI.ResendConfirmationEmail`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiResendConfirmationEmailRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **resendConfirmationEmailRequest** | [**ResendConfirmationEmailRequest**](ResendConfirmationEmailRequest.md) |  | 

### Return type

[**ResendConfirmationEmail200Response**](ResendConfirmationEmail200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

