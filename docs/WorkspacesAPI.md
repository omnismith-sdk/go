# \WorkspacesAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateWorkspace**](WorkspacesAPI.md#CreateWorkspace) | **Post** /workspaces | Create a new workspace
[**CreateWorkspaceView**](WorkspacesAPI.md#CreateWorkspaceView) | **Post** /workspaces/{id}/views | Add a new view / pane to a workspace
[**DeleteWorkspace**](WorkspacesAPI.md#DeleteWorkspace) | **Delete** /workspaces/{id} | Delete a workspace and its views
[**DeleteWorkspaceView**](WorkspacesAPI.md#DeleteWorkspaceView) | **Delete** /workspaces/{id}/views/{viewId} | Delete a view / pane from a workspace
[**DuplicateWorkspace**](WorkspacesAPI.md#DuplicateWorkspace) | **Post** /workspaces/{id}/duplicate | Duplicate an existing workspace and its views
[**GetWorkspace**](WorkspacesAPI.md#GetWorkspace) | **Get** /workspaces/{id} | Get workspace details and its views
[**GetWorkspaceView**](WorkspacesAPI.md#GetWorkspaceView) | **Get** /workspaces/{id}/views/{viewId} | Get details of a workspace view / pane
[**ListTemplateViews**](WorkspacesAPI.md#ListTemplateViews) | **Get** /workspaces/template/{templateId} | List saved views for a specific template across workspaces
[**ListWorkspaces**](WorkspacesAPI.md#ListWorkspaces) | **Get** /workspaces | List all workspaces for current project
[**ReorderWorkspaceViews**](WorkspacesAPI.md#ReorderWorkspaceViews) | **Put** /workspaces/{id}/reorder-views | Reorder views inside a workspace
[**SetDefaultWorkspace**](WorkspacesAPI.md#SetDefaultWorkspace) | **Post** /workspaces/{id}/default | Set workspace as the default workspace
[**UpdateWorkspace**](WorkspacesAPI.md#UpdateWorkspace) | **Put** /workspaces/{id} | Update workspace metadata and layout
[**UpdateWorkspaceView**](WorkspacesAPI.md#UpdateWorkspaceView) | **Put** /workspaces/{id}/views/{viewId} | Update workspace view / pane filters, sort, display mode, or columns



## CreateWorkspace

> CreateDashboard201Response CreateWorkspace(ctx).CreateWorkspaceRequest(createWorkspaceRequest).Execute()

Create a new workspace



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
	createWorkspaceRequest := *openapiclient.NewCreateWorkspaceRequest("Operations Hub") // CreateWorkspaceRequest | Workspace creation payload

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.CreateWorkspace(context.Background()).CreateWorkspaceRequest(createWorkspaceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.CreateWorkspace``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateWorkspace`: CreateDashboard201Response
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.CreateWorkspace`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateWorkspaceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createWorkspaceRequest** | [**CreateWorkspaceRequest**](CreateWorkspaceRequest.md) | Workspace creation payload | 

### Return type

[**CreateDashboard201Response**](CreateDashboard201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateWorkspaceView

> CreateDashboardBlock201Response CreateWorkspaceView(ctx, id).CreateWorkspaceViewRequest(createWorkspaceViewRequest).Execute()

Add a new view / pane to a workspace



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
	id := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Target workspace unique identifier (UUID)
	createWorkspaceViewRequest := *openapiclient.NewCreateWorkspaceViewRequest("0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b", "Active Gateways") // CreateWorkspaceViewRequest | Workspace view creation payload

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.CreateWorkspaceView(context.Background(), id).CreateWorkspaceViewRequest(createWorkspaceViewRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.CreateWorkspaceView``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateWorkspaceView`: CreateDashboardBlock201Response
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.CreateWorkspaceView`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Target workspace unique identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateWorkspaceViewRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createWorkspaceViewRequest** | [**CreateWorkspaceViewRequest**](CreateWorkspaceViewRequest.md) | Workspace view creation payload | 

### Return type

[**CreateDashboardBlock201Response**](CreateDashboardBlock201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteWorkspace

> DeleteWorkspace(ctx, id).Execute()

Delete a workspace and its views



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
	id := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Workspace unique identifier (UUID) to delete

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.WorkspacesAPI.DeleteWorkspace(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.DeleteWorkspace``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Workspace unique identifier (UUID) to delete | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteWorkspaceRequest struct via the builder pattern


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


## DeleteWorkspaceView

> DeleteWorkspaceView(ctx, id, viewId).Execute()

Delete a view / pane from a workspace



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
	id := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Workspace unique identifier (UUID)
	viewId := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6c" // string | Workspace view unique identifier (UUID) to delete

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.WorkspacesAPI.DeleteWorkspaceView(context.Background(), id, viewId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.DeleteWorkspaceView``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Workspace unique identifier (UUID) | 
**viewId** | **string** | Workspace view unique identifier (UUID) to delete | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteWorkspaceViewRequest struct via the builder pattern


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


## DuplicateWorkspace

> DuplicateWorkspace201Response DuplicateWorkspace(ctx, id).DuplicateWorkspaceRequest(duplicateWorkspaceRequest).Execute()

Duplicate an existing workspace and its views



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
	id := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Source workspace unique identifier (UUID) to clone
	duplicateWorkspaceRequest := *openapiclient.NewDuplicateWorkspaceRequest() // DuplicateWorkspaceRequest | Optional configuration for the duplicated workspace (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.DuplicateWorkspace(context.Background(), id).DuplicateWorkspaceRequest(duplicateWorkspaceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.DuplicateWorkspace``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DuplicateWorkspace`: DuplicateWorkspace201Response
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.DuplicateWorkspace`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Source workspace unique identifier (UUID) to clone | 

### Other Parameters

Other parameters are passed through a pointer to a apiDuplicateWorkspaceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **duplicateWorkspaceRequest** | [**DuplicateWorkspaceRequest**](DuplicateWorkspaceRequest.md) | Optional configuration for the duplicated workspace | 

### Return type

[**DuplicateWorkspace201Response**](DuplicateWorkspace201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetWorkspace

> WorkspaceDetailsResponse GetWorkspace(ctx, id).Execute()

Get workspace details and its views



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
	id := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Workspace unique identifier (UUID)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.GetWorkspace(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.GetWorkspace``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetWorkspace`: WorkspaceDetailsResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.GetWorkspace`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Workspace unique identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetWorkspaceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**WorkspaceDetailsResponse**](WorkspaceDetailsResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetWorkspaceView

> WorkspaceViewResponse GetWorkspaceView(ctx, id, viewId).Execute()

Get details of a workspace view / pane



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
	id := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Workspace unique identifier (UUID)
	viewId := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6c" // string | Workspace view unique identifier (UUID)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.GetWorkspaceView(context.Background(), id, viewId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.GetWorkspaceView``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetWorkspaceView`: WorkspaceViewResponse
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.GetWorkspaceView`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Workspace unique identifier (UUID) | 
**viewId** | **string** | Workspace view unique identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetWorkspaceViewRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**WorkspaceViewResponse**](WorkspaceViewResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTemplateViews

> ListTemplateViews200Response ListTemplateViews(ctx, templateId).Execute()

List saved views for a specific template across workspaces



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
	templateId := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Schema template unique identifier (UUID)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkspacesAPI.ListTemplateViews(context.Background(), templateId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.ListTemplateViews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTemplateViews`: ListTemplateViews200Response
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.ListTemplateViews`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | Schema template unique identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiListTemplateViewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ListTemplateViews200Response**](ListTemplateViews200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListWorkspaces

> ListWorkspaces200Response ListWorkspaces(ctx).Execute()

List all workspaces for current project



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
	resp, r, err := apiClient.WorkspacesAPI.ListWorkspaces(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.ListWorkspaces``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListWorkspaces`: ListWorkspaces200Response
	fmt.Fprintf(os.Stdout, "Response from `WorkspacesAPI.ListWorkspaces`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListWorkspacesRequest struct via the builder pattern


### Return type

[**ListWorkspaces200Response**](ListWorkspaces200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ReorderWorkspaceViews

> ReorderWorkspaceViews(ctx, id).ReorderWorkspaceViewsRequest(reorderWorkspaceViewsRequest).Execute()

Reorder views inside a workspace



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
	id := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Workspace unique identifier (UUID)
	reorderWorkspaceViewsRequest := *openapiclient.NewReorderWorkspaceViewsRequest([]string{"ViewIds_example"}) // ReorderWorkspaceViewsRequest | Payload containing ordered view IDs

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.WorkspacesAPI.ReorderWorkspaceViews(context.Background(), id).ReorderWorkspaceViewsRequest(reorderWorkspaceViewsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.ReorderWorkspaceViews``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Workspace unique identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiReorderWorkspaceViewsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **reorderWorkspaceViewsRequest** | [**ReorderWorkspaceViewsRequest**](ReorderWorkspaceViewsRequest.md) | Payload containing ordered view IDs | 

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


## SetDefaultWorkspace

> SetDefaultWorkspace(ctx, id).Execute()

Set workspace as the default workspace



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
	id := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Workspace unique identifier (UUID) to designate as default

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.WorkspacesAPI.SetDefaultWorkspace(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.SetDefaultWorkspace``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Workspace unique identifier (UUID) to designate as default | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetDefaultWorkspaceRequest struct via the builder pattern


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


## UpdateWorkspace

> UpdateWorkspace(ctx, id).UpdateWorkspaceRequest(updateWorkspaceRequest).Execute()

Update workspace metadata and layout



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
	id := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Workspace unique identifier (UUID) to update
	updateWorkspaceRequest := *openapiclient.NewUpdateWorkspaceRequest() // UpdateWorkspaceRequest | Workspace update payload

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.WorkspacesAPI.UpdateWorkspace(context.Background(), id).UpdateWorkspaceRequest(updateWorkspaceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.UpdateWorkspace``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Workspace unique identifier (UUID) to update | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateWorkspaceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateWorkspaceRequest** | [**UpdateWorkspaceRequest**](UpdateWorkspaceRequest.md) | Workspace update payload | 

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


## UpdateWorkspaceView

> UpdateWorkspaceView(ctx, id, viewId).UpdateWorkspaceViewRequest(updateWorkspaceViewRequest).Execute()

Update workspace view / pane filters, sort, display mode, or columns



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
	id := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Workspace unique identifier (UUID)
	viewId := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6c" // string | Workspace view unique identifier (UUID) to update
	updateWorkspaceViewRequest := *openapiclient.NewUpdateWorkspaceViewRequest() // UpdateWorkspaceViewRequest | Workspace view update payload

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.WorkspacesAPI.UpdateWorkspaceView(context.Background(), id, viewId).UpdateWorkspaceViewRequest(updateWorkspaceViewRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkspacesAPI.UpdateWorkspaceView``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Workspace unique identifier (UUID) | 
**viewId** | **string** | Workspace view unique identifier (UUID) to update | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateWorkspaceViewRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateWorkspaceViewRequest** | [**UpdateWorkspaceViewRequest**](UpdateWorkspaceViewRequest.md) | Workspace view update payload | 

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

