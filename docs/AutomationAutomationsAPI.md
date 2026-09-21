# \AutomationAutomationsAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateAutomation**](AutomationAutomationsAPI.md#CreateAutomation) | **Post** /automation/automations | Create an automation rule
[**DeleteAutomation**](AutomationAutomationsAPI.md#DeleteAutomation) | **Delete** /automation/automations/{id} | Delete an automation
[**GetAutomation**](AutomationAutomationsAPI.md#GetAutomation) | **Get** /automation/automations/{id} | Get an automation by ID
[**ListAutomationExecutions**](AutomationAutomationsAPI.md#ListAutomationExecutions) | **Get** /automation/automations/{id}/executions | List automation execution logs
[**ListAutomations**](AutomationAutomationsAPI.md#ListAutomations) | **Get** /automation/automations | List project automations
[**ToggleAutomation**](AutomationAutomationsAPI.md#ToggleAutomation) | **Patch** /automation/automations/{id}/toggle | Toggle automation enabled status
[**UpdateAutomation**](AutomationAutomationsAPI.md#UpdateAutomation) | **Put** /automation/automations/{id} | Update an automation



## CreateAutomation

> CreateAutomation201Response CreateAutomation(ctx).CreateAutomationRequest(createAutomationRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Create an automation rule



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
	createAutomationRequest := *openapiclient.NewCreateAutomationRequest("Notify on status change", *openapiclient.NewCreateAutomationRequestTrigger("on_attribute_changed"), []openapiclient.CreateAutomationRequestConditionsInner{*openapiclient.NewCreateAutomationRequestConditionsInner("01912ecb-4654-7890-a1b2-c3d4e5f60077", "eq", "current")}, []openapiclient.CreateAutomationRequestActionsInner{*openapiclient.NewCreateAutomationRequestActionsInner("telegram", map[string]interface{}(123))}) // CreateAutomationRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutomationAutomationsAPI.CreateAutomation(context.Background()).CreateAutomationRequest(createAutomationRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutomationAutomationsAPI.CreateAutomation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateAutomation`: CreateAutomation201Response
	fmt.Fprintf(os.Stdout, "Response from `AutomationAutomationsAPI.CreateAutomation`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createAutomationRequest** | [**CreateAutomationRequest**](CreateAutomationRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**CreateAutomation201Response**](CreateAutomation201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteAutomation

> DeleteAutomation(ctx, id).XOmnismithProjectId(xOmnismithProjectId).Execute()

Delete an automation



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
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60001" // string | Unique automation UUID to delete
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AutomationAutomationsAPI.DeleteAutomation(context.Background(), id).XOmnismithProjectId(xOmnismithProjectId).Execute()
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
**id** | **string** | Unique automation UUID to delete | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

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


## GetAutomation

> AutomationResponse GetAutomation(ctx, id).XOmnismithProjectId(xOmnismithProjectId).Execute()

Get an automation by ID



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
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60001" // string | Unique automation UUID
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutomationAutomationsAPI.GetAutomation(context.Background(), id).XOmnismithProjectId(xOmnismithProjectId).Execute()
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
**id** | **string** | Unique automation UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

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

> ListAutomationExecutions200Response ListAutomationExecutions(ctx, id).XOmnismithProjectId(xOmnismithProjectId).Limit(limit).Offset(offset).Status(status).Execute()

List automation execution logs



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
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60001" // string | Automation UUID to fetch execution history for
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)
	limit := int32(20) // int32 | Maximum number of execution log entries to return per page (optional) (default to 20)
	offset := int32(0) // int32 | Number of execution log records to skip for pagination (optional) (default to 0)
	status := "success" // string | Filter execution logs by execution outcome status (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutomationAutomationsAPI.ListAutomationExecutions(context.Background(), id).XOmnismithProjectId(xOmnismithProjectId).Limit(limit).Offset(offset).Status(status).Execute()
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
**id** | **string** | Automation UUID to fetch execution history for | 

### Other Parameters

Other parameters are passed through a pointer to a apiListAutomationExecutionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 
 **limit** | **int32** | Maximum number of execution log entries to return per page | [default to 20]
 **offset** | **int32** | Number of execution log records to skip for pagination | [default to 0]
 **status** | **string** | Filter execution logs by execution outcome status | 

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

> []AutomationResponse ListAutomations(ctx).XOmnismithProjectId(xOmnismithProjectId).TemplateId(templateId).IsEnabled(isEnabled).Execute()

List project automations



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
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)
	templateId := "01912ecb-4654-7890-a1b2-c3d4e5f60088" // string | Filter automations scoped to a specific entity template UUID (optional)
	isEnabled := true // bool | Filter automations by active enabled status (true for active rules, false for paused rules) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutomationAutomationsAPI.ListAutomations(context.Background()).XOmnismithProjectId(xOmnismithProjectId).TemplateId(templateId).IsEnabled(isEnabled).Execute()
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
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 
 **templateId** | **string** | Filter automations scoped to a specific entity template UUID | 
 **isEnabled** | **bool** | Filter automations by active enabled status (true for active rules, false for paused rules) | 

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

> AutomationResponse ToggleAutomation(ctx, id).ToggleAutomationRequest(toggleAutomationRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Toggle automation enabled status



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
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60001" // string | Unique automation UUID to toggle
	toggleAutomationRequest := *openapiclient.NewToggleAutomationRequest(true) // ToggleAutomationRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutomationAutomationsAPI.ToggleAutomation(context.Background(), id).ToggleAutomationRequest(toggleAutomationRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
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
**id** | **string** | Unique automation UUID to toggle | 

### Other Parameters

Other parameters are passed through a pointer to a apiToggleAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **toggleAutomationRequest** | [**ToggleAutomationRequest**](ToggleAutomationRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

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

> UpdateAutomation(ctx, id).UpdateAutomationRequest(updateAutomationRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Update an automation



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
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60001" // string | Unique automation UUID to update
	updateAutomationRequest := *openapiclient.NewUpdateAutomationRequest() // UpdateAutomationRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AutomationAutomationsAPI.UpdateAutomation(context.Background(), id).UpdateAutomationRequest(updateAutomationRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
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
**id** | **string** | Unique automation UUID to update | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateAutomationRequest** | [**UpdateAutomationRequest**](UpdateAutomationRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

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

