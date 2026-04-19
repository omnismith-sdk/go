# \AutomationAutomationsAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateAutomation**](AutomationAutomationsAPI.md#CreateAutomation) | **Post** /automation/automations | Create a new automation
[**DeleteAutomation**](AutomationAutomationsAPI.md#DeleteAutomation) | **Delete** /automation/automations/{id} | Delete an automation
[**GetAutomation**](AutomationAutomationsAPI.md#GetAutomation) | **Get** /automation/automations/{id} | Get an automation by ID
[**ListAutomationExecutions**](AutomationAutomationsAPI.md#ListAutomationExecutions) | **Get** /automation/automations/{id}/executions | List automation executions
[**ListAutomations**](AutomationAutomationsAPI.md#ListAutomations) | **Get** /automation/automations | List automations
[**ToggleAutomation**](AutomationAutomationsAPI.md#ToggleAutomation) | **Patch** /automation/automations/{id}/toggle | Toggle automation enabled status
[**UpdateAutomation**](AutomationAutomationsAPI.md#UpdateAutomation) | **Put** /automation/automations/{id} | Update an automation



## CreateAutomation

> CreateAttributeItem201Response CreateAutomation(ctx).CreateAutomationRequest(createAutomationRequest).Execute()

Create a new automation

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
	createAutomationRequest := *openapiclient.NewCreateAutomationRequest("Notify on status change", *openapiclient.NewCreateAutomationRequestTrigger("on_attribute_changed"), []openapiclient.CreateAutomationRequestConditionsInner{*openapiclient.NewCreateAutomationRequestConditionsInner("AttributeId_example", "eq", "current")}, []openapiclient.CreateAutomationRequestActionsInner{*openapiclient.NewCreateAutomationRequestActionsInner("telegram", map[string]interface{}(123))}) // CreateAutomationRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutomationAutomationsAPI.CreateAutomation(context.Background()).CreateAutomationRequest(createAutomationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutomationAutomationsAPI.CreateAutomation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateAutomation`: CreateAttributeItem201Response
	fmt.Fprintf(os.Stdout, "Response from `AutomationAutomationsAPI.CreateAutomation`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createAutomationRequest** | [**CreateAutomationRequest**](CreateAutomationRequest.md) |  | 

### Return type

[**CreateAttributeItem201Response**](CreateAttributeItem201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteAutomation

> DeleteAutomation(ctx, id).Execute()

Delete an automation

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AutomationAutomationsAPI.DeleteAutomation(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutomationAutomationsAPI.DeleteAutomation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

 (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetAutomation

> AutomationResponse GetAutomation(ctx, id).Execute()

Get an automation by ID

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutomationAutomationsAPI.GetAutomation(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutomationAutomationsAPI.GetAutomation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAutomation`: AutomationResponse
	fmt.Fprintf(os.Stdout, "Response from `AutomationAutomationsAPI.GetAutomation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**AutomationResponse**](AutomationResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListAutomationExecutions

> ListAutomationExecutions200Response ListAutomationExecutions(ctx, id).Limit(limit).Offset(offset).Status(status).Execute()

List automation executions

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Automation ID
	limit := int32(56) // int32 | Number of results (optional) (default to 20)
	offset := int32(56) // int32 | Pagination offset (optional) (default to 0)
	status := "status_example" // string | Filter by status (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutomationAutomationsAPI.ListAutomationExecutions(context.Background(), id).Limit(limit).Offset(offset).Status(status).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutomationAutomationsAPI.ListAutomationExecutions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAutomationExecutions`: ListAutomationExecutions200Response
	fmt.Fprintf(os.Stdout, "Response from `AutomationAutomationsAPI.ListAutomationExecutions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Automation ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiListAutomationExecutionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **limit** | **int32** | Number of results | [default to 20]
 **offset** | **int32** | Pagination offset | [default to 0]
 **status** | **string** | Filter by status | 

### Return type

[**ListAutomationExecutions200Response**](ListAutomationExecutions200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListAutomations

> []AutomationResponse ListAutomations(ctx).TemplateId(templateId).IsEnabled(isEnabled).Execute()

List automations

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
	templateId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Filter by template ID (optional)
	isEnabled := true // bool | Filter by enabled status (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutomationAutomationsAPI.ListAutomations(context.Background()).TemplateId(templateId).IsEnabled(isEnabled).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutomationAutomationsAPI.ListAutomations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAutomations`: []AutomationResponse
	fmt.Fprintf(os.Stdout, "Response from `AutomationAutomationsAPI.ListAutomations`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListAutomationsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **templateId** | **string** | Filter by template ID | 
 **isEnabled** | **bool** | Filter by enabled status | 

### Return type

[**[]AutomationResponse**](AutomationResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ToggleAutomation

> AutomationResponse ToggleAutomation(ctx, id).ToggleAutomationRequest(toggleAutomationRequest).Execute()

Toggle automation enabled status

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 
	toggleAutomationRequest := *openapiclient.NewToggleAutomationRequest(true) // ToggleAutomationRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutomationAutomationsAPI.ToggleAutomation(context.Background(), id).ToggleAutomationRequest(toggleAutomationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutomationAutomationsAPI.ToggleAutomation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ToggleAutomation`: AutomationResponse
	fmt.Fprintf(os.Stdout, "Response from `AutomationAutomationsAPI.ToggleAutomation`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiToggleAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **toggleAutomationRequest** | [**ToggleAutomationRequest**](ToggleAutomationRequest.md) |  | 

### Return type

[**AutomationResponse**](AutomationResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateAutomation

> UpdateAutomation(ctx, id).UpdateAutomationRequest(updateAutomationRequest).Execute()

Update an automation

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 
	updateAutomationRequest := *openapiclient.NewUpdateAutomationRequest() // UpdateAutomationRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AutomationAutomationsAPI.UpdateAutomation(context.Background(), id).UpdateAutomationRequest(updateAutomationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutomationAutomationsAPI.UpdateAutomation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateAutomationRequest** | [**UpdateAutomationRequest**](UpdateAutomationRequest.md) |  | 

### Return type

 (empty response body)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

