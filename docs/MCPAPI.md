# \MCPAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateAttribute**](MCPAPI.md#CreateAttribute) | **Post** /attributes | Create a new attribute
[**CreateAttributeItem**](MCPAPI.md#CreateAttributeItem) | **Post** /attributes/{id}/items | Add a list item to an attribute
[**CreateAutomation**](MCPAPI.md#CreateAutomation) | **Post** /automation/automations | Create an automation rule
[**CreateDashboard**](MCPAPI.md#CreateDashboard) | **Post** /dashboards | Create a new dashboard
[**CreateDashboardBlock**](MCPAPI.md#CreateDashboardBlock) | **Post** /dashboards/{dashboardId}/blocks | Create a new block in a dashboard
[**CreateEntity**](MCPAPI.md#CreateEntity) | **Post** /entities | Create a new dynamic entity
[**CreateNotificationChannel**](MCPAPI.md#CreateNotificationChannel) | **Post** /automation/notification-channels | Create a notification channel
[**CreateTemplate**](MCPAPI.md#CreateTemplate) | **Post** /templates | Create a new template
[**CreateWorkspace**](MCPAPI.md#CreateWorkspace) | **Post** /workspaces | Create a new workspace
[**CreateWorkspaceView**](MCPAPI.md#CreateWorkspaceView) | **Post** /workspaces/{id}/views | Add a new view / pane to a workspace
[**DeleteAttribute**](MCPAPI.md#DeleteAttribute) | **Delete** /attributes/{id} | Delete an attribute
[**DeleteAttributeReferenceConfig**](MCPAPI.md#DeleteAttributeReferenceConfig) | **Delete** /attributes/{id}/reference | Delete reference configuration for an attribute
[**DeleteAutomation**](MCPAPI.md#DeleteAutomation) | **Delete** /automation/automations/{id} | Delete an automation
[**DeleteDashboard**](MCPAPI.md#DeleteDashboard) | **Delete** /dashboards/{id} | Delete a dashboard
[**DeleteDashboardBlock**](MCPAPI.md#DeleteDashboardBlock) | **Delete** /dashboards/{dashboardId}/blocks/{blockId} | Delete a dashboard block
[**DeleteEntity**](MCPAPI.md#DeleteEntity) | **Delete** /entities/{id} | Soft-delete an entity record
[**DeleteNotificationChannel**](MCPAPI.md#DeleteNotificationChannel) | **Delete** /automation/notification-channels/{id} | Delete a notification channel
[**DeleteTemplate**](MCPAPI.md#DeleteTemplate) | **Delete** /templates/{id} | Delete a template
[**DeleteWorkspace**](MCPAPI.md#DeleteWorkspace) | **Delete** /workspaces/{id} | Delete a workspace and its views
[**DeleteWorkspaceView**](MCPAPI.md#DeleteWorkspaceView) | **Delete** /workspaces/{id}/views/{viewId} | Delete a view / pane from a workspace
[**GetAttribute**](MCPAPI.md#GetAttribute) | **Get** /attributes/{id} | Get an attribute by ID
[**GetAttributeReferenceConfig**](MCPAPI.md#GetAttributeReferenceConfig) | **Get** /attributes/{id}/reference | Get reference configuration for an attribute
[**GetAutomation**](MCPAPI.md#GetAutomation) | **Get** /automation/automations/{id} | Get an automation by ID
[**GetDashboard**](MCPAPI.md#GetDashboard) | **Get** /dashboards/{id} | Get a dashboard by ID
[**GetDashboardBlock**](MCPAPI.md#GetDashboardBlock) | **Get** /dashboards/{dashboardId}/blocks/{blockId} | Get a dashboard block by ID
[**GetEntity**](MCPAPI.md#GetEntity) | **Get** /entities/{id} | Get an entity record by ID
[**GetEntityChart**](MCPAPI.md#GetEntityChart) | **Get** /entities/{id}/chart | Get entity chart time-series data
[**GetEntityHistory**](MCPAPI.md#GetEntityHistory) | **Get** /entities/{id}/history | Get entity dimension change history
[**GetMarketplaceBlueprint**](MCPAPI.md#GetMarketplaceBlueprint) | **Get** /marketplace/blueprints/{id} | Get marketplace blueprint details
[**GetNotificationChannel**](MCPAPI.md#GetNotificationChannel) | **Get** /automation/notification-channels/{id} | Get a notification channel by ID
[**GetProjectSchema**](MCPAPI.md#GetProjectSchema) | **Get** /discovery/project-schema | Get complete project schema graph
[**GetTemplate**](MCPAPI.md#GetTemplate) | **Get** /templates/{id} | Get a template by ID or slug
[**GetUsageInsights**](MCPAPI.md#GetUsageInsights) | **Get** /billing/usage/insights | Get current tier usage insights
[**GetWorkspace**](MCPAPI.md#GetWorkspace) | **Get** /workspaces/{id} | Get workspace details and its views
[**GetWorkspaceView**](MCPAPI.md#GetWorkspaceView) | **Get** /workspaces/{id}/views/{viewId} | Get details of a workspace view / pane
[**IngestEntityMetrics**](MCPAPI.md#IngestEntityMetrics) | **Post** /entities/{id}/metrics | Ingest high-frequency metric observations for an entity
[**InstallMarketplaceBlueprint**](MCPAPI.md#InstallMarketplaceBlueprint) | **Post** /marketplace/blueprints/{id}/install | Install a marketplace blueprint into a project
[**ListAttributeItems**](MCPAPI.md#ListAttributeItems) | **Get** /attributes/{id}/items | List items of an attribute
[**ListAttributes**](MCPAPI.md#ListAttributes) | **Get** /attributes | List all attributes
[**ListAuditLogs**](MCPAPI.md#ListAuditLogs) | **Get** /audit-logs | List project audit logs
[**ListAutomations**](MCPAPI.md#ListAutomations) | **Get** /automation/automations | List project automations
[**ListDashboardBlocks**](MCPAPI.md#ListDashboardBlocks) | **Get** /dashboards/{dashboardId}/blocks | List all blocks in a dashboard
[**ListDashboards**](MCPAPI.md#ListDashboards) | **Get** /dashboards | List all dashboards
[**ListNotificationChannels**](MCPAPI.md#ListNotificationChannels) | **Get** /automation/notification-channels | List notification channels
[**ListTemplateEntityCounts**](MCPAPI.md#ListTemplateEntityCounts) | **Get** /templates/entity-counts | List entity counts per template
[**ListTemplates**](MCPAPI.md#ListTemplates) | **Get** /templates | List all templates
[**ListWorkspaces**](MCPAPI.md#ListWorkspaces) | **Get** /workspaces | List all workspaces for current project
[**PatchAttribute**](MCPAPI.md#PatchAttribute) | **Patch** /attributes/{id} | Patch an attribute (granular partial update)
[**PatchTemplate**](MCPAPI.md#PatchTemplate) | **Patch** /templates/{id} | Patch a template (granular partial update)
[**ResolveDashboardBlock**](MCPAPI.md#ResolveDashboardBlock) | **Get** /dashboards/{dashboardId}/blocks/{blockId}/resolve | Resolve a dashboard block to its computed data
[**SearchEntities**](MCPAPI.md#SearchEntities) | **Post** /entities/search/{template_id} | Search entities with filtering, sorting, and pagination
[**SearchMarketplaceBlueprints**](MCPAPI.md#SearchMarketplaceBlueprints) | **Get** /marketplace/blueprints | Search marketplace blueprints
[**SetAttributeItems**](MCPAPI.md#SetAttributeItems) | **Put** /attributes/{id}/items | Set list items for an attribute (replaces all existing items)
[**SetAttributeReferenceConfig**](MCPAPI.md#SetAttributeReferenceConfig) | **Put** /attributes/{id}/reference | Set or update reference configuration for an attribute
[**TestNotificationChannel**](MCPAPI.md#TestNotificationChannel) | **Post** /automation/notification-channels/{id}/test | Send a test notification message
[**ToggleAutomation**](MCPAPI.md#ToggleAutomation) | **Patch** /automation/automations/{id}/toggle | Toggle automation enabled status
[**UpdateAttribute**](MCPAPI.md#UpdateAttribute) | **Put** /attributes/{id} | Update an attribute (full replacement)
[**UpdateAutomation**](MCPAPI.md#UpdateAutomation) | **Put** /automation/automations/{id} | Update an automation
[**UpdateDashboard**](MCPAPI.md#UpdateDashboard) | **Put** /dashboards/{id} | Update a dashboard
[**UpdateDashboardBlock**](MCPAPI.md#UpdateDashboardBlock) | **Put** /dashboards/{dashboardId}/blocks/{blockId} | Update a dashboard block
[**UpdateEntity**](MCPAPI.md#UpdateEntity) | **Patch** /entities/{id} | Update entity attribute values
[**UpdateNotificationChannel**](MCPAPI.md#UpdateNotificationChannel) | **Put** /automation/notification-channels/{id} | Update a notification channel
[**UpdateTemplate**](MCPAPI.md#UpdateTemplate) | **Put** /templates/{id} | Update a template (full replacement)
[**UpdateWorkspace**](MCPAPI.md#UpdateWorkspace) | **Put** /workspaces/{id} | Update workspace metadata and layout
[**UpdateWorkspaceView**](MCPAPI.md#UpdateWorkspaceView) | **Put** /workspaces/{id}/views/{viewId} | Update workspace view / pane filters, sort, display mode, or columns



## CreateAttribute

> CreateAttribute201Response CreateAttribute(ctx).CreateAttributeRequest(createAttributeRequest).Execute()

Create a new attribute



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
	createAttributeRequest := *openapiclient.NewCreateAttributeRequest("Product Color", int32(0), int32(0)) // CreateAttributeRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.CreateAttribute(context.Background()).CreateAttributeRequest(createAttributeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.CreateAttribute``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateAttribute`: CreateAttribute201Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.CreateAttribute`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateAttributeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createAttributeRequest** | [**CreateAttributeRequest**](CreateAttributeRequest.md) |  | 

### Return type

[**CreateAttribute201Response**](CreateAttribute201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateAttributeItem

> CreateAttributeItem201Response CreateAttributeItem(ctx, id).AddListItemRequest(addListItemRequest).Execute()

Add a list item to an attribute



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | UUID of the List-type attribute
	addListItemRequest := *openapiclient.NewAddListItemRequest("Green") // AddListItemRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.CreateAttributeItem(context.Background(), id).AddListItemRequest(addListItemRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.CreateAttributeItem``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateAttributeItem`: CreateAttributeItem201Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.CreateAttributeItem`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | UUID of the List-type attribute | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateAttributeItemRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **addListItemRequest** | [**AddListItemRequest**](AddListItemRequest.md) |  | 

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


## CreateAutomation

> CreateAutomation201Response CreateAutomation(ctx).CreateAutomationRequest(createAutomationRequest).Execute()

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.CreateAutomation(context.Background()).CreateAutomationRequest(createAutomationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.CreateAutomation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateAutomation`: CreateAutomation201Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.CreateAutomation`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateAutomationRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createAutomationRequest** | [**CreateAutomationRequest**](CreateAutomationRequest.md) |  | 

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


## CreateDashboard

> CreateDashboard201Response CreateDashboard(ctx).CreateDashboardRequest(createDashboardRequest).Execute()

Create a new dashboard



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
	createDashboardRequest := *openapiclient.NewCreateDashboardRequest("Infrastructure & Operations Hub") // CreateDashboardRequest | Dashboard creation payload

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.CreateDashboard(context.Background()).CreateDashboardRequest(createDashboardRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.CreateDashboard``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateDashboard`: CreateDashboard201Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.CreateDashboard`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateDashboardRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createDashboardRequest** | [**CreateDashboardRequest**](CreateDashboardRequest.md) | Dashboard creation payload | 

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


## CreateDashboardBlock

> CreateDashboardBlock201Response CreateDashboardBlock(ctx, dashboardId).CreateDashboardBlockRequest(createDashboardBlockRequest).Execute()

Create a new block in a dashboard



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
	dashboardId := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Target dashboard unique identifier (UUID)
	createDashboardBlockRequest := *openapiclient.NewCreateDashboardBlockRequest("chart", "CPU Utilization — Time Series") // CreateDashboardBlockRequest | Dashboard block creation payload

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.CreateDashboardBlock(context.Background(), dashboardId).CreateDashboardBlockRequest(createDashboardBlockRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.CreateDashboardBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateDashboardBlock`: CreateDashboardBlock201Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.CreateDashboardBlock`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dashboardId** | **string** | Target dashboard unique identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateDashboardBlockRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createDashboardBlockRequest** | [**CreateDashboardBlockRequest**](CreateDashboardBlockRequest.md) | Dashboard block creation payload | 

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


## CreateEntity

> CreateEntity201Response CreateEntity(ctx).CreateEntityRequest(createEntityRequest).Execute()

Create a new dynamic entity



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
	createEntityRequest := *openapiclient.NewCreateEntityRequest() // CreateEntityRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.CreateEntity(context.Background()).CreateEntityRequest(createEntityRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.CreateEntity``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateEntity`: CreateEntity201Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.CreateEntity`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateEntityRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createEntityRequest** | [**CreateEntityRequest**](CreateEntityRequest.md) |  | 

### Return type

[**CreateEntity201Response**](CreateEntity201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateNotificationChannel

> CreateNotificationChannel201Response CreateNotificationChannel(ctx).CreateNotificationChannelRequest(createNotificationChannelRequest).Execute()

Create a notification channel



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
	createNotificationChannelRequest := *openapiclient.NewCreateNotificationChannelRequest("telegram", "Alerts Bot", *openapiclient.NewCreateNotificationChannelRequestCredentials()) // CreateNotificationChannelRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.CreateNotificationChannel(context.Background()).CreateNotificationChannelRequest(createNotificationChannelRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.CreateNotificationChannel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateNotificationChannel`: CreateNotificationChannel201Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.CreateNotificationChannel`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateNotificationChannelRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createNotificationChannelRequest** | [**CreateNotificationChannelRequest**](CreateNotificationChannelRequest.md) |  | 

### Return type

[**CreateNotificationChannel201Response**](CreateNotificationChannel201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateTemplate

> CreateTemplate201Response CreateTemplate(ctx).CreateTemplateRequest(createTemplateRequest).Execute()

Create a new template



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
	createTemplateRequest := *openapiclient.NewCreateTemplateRequest("Product SKU") // CreateTemplateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.CreateTemplate(context.Background()).CreateTemplateRequest(createTemplateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.CreateTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTemplate`: CreateTemplate201Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.CreateTemplate`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateTemplateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createTemplateRequest** | [**CreateTemplateRequest**](CreateTemplateRequest.md) |  | 

### Return type

[**CreateTemplate201Response**](CreateTemplate201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


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
	resp, r, err := apiClient.MCPAPI.CreateWorkspace(context.Background()).CreateWorkspaceRequest(createWorkspaceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.CreateWorkspace``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateWorkspace`: CreateDashboard201Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.CreateWorkspace`: %v\n", resp)
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
	resp, r, err := apiClient.MCPAPI.CreateWorkspaceView(context.Background(), id).CreateWorkspaceViewRequest(createWorkspaceViewRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.CreateWorkspaceView``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateWorkspaceView`: CreateDashboardBlock201Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.CreateWorkspaceView`: %v\n", resp)
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


## DeleteAttribute

> DeleteAttribute(ctx, id).Execute()

Delete an attribute



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | UUID of the attribute to delete

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.DeleteAttribute(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.DeleteAttribute``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | UUID of the attribute to delete | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAttributeRequest struct via the builder pattern


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


## DeleteAttributeReferenceConfig

> DeleteAttributeReferenceConfig(ctx, id).Execute()

Delete reference configuration for an attribute



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | UUID of the Reference attribute

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.DeleteAttributeReferenceConfig(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.DeleteAttributeReferenceConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | UUID of the Reference attribute | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAttributeReferenceConfigRequest struct via the builder pattern


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
	openapiclient "github.com/omnismith-sdk/go"
)

func main() {
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60001" // string | Unique automation UUID to delete

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.DeleteAutomation(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.DeleteAutomation``: %v\n", err)
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


## DeleteDashboard

> DeleteDashboard(ctx, id).Execute()

Delete a dashboard



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
	id := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Dashboard unique identifier (UUID) to delete

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.DeleteDashboard(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.DeleteDashboard``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Dashboard unique identifier (UUID) to delete | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDashboardRequest struct via the builder pattern


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


## DeleteDashboardBlock

> DeleteDashboardBlock(ctx, dashboardId, blockId).Execute()

Delete a dashboard block



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
	dashboardId := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Parent dashboard unique identifier (UUID)
	blockId := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6c" // string | Dashboard block unique identifier (UUID) to delete

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.DeleteDashboardBlock(context.Background(), dashboardId, blockId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.DeleteDashboardBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dashboardId** | **string** | Parent dashboard unique identifier (UUID) | 
**blockId** | **string** | Dashboard block unique identifier (UUID) to delete | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteDashboardBlockRequest struct via the builder pattern


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


## DeleteEntity

> DeleteEntity(ctx, id).Execute()

Soft-delete an entity record



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | Unique entity identifier (UUID) to soft-delete

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.DeleteEntity(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.DeleteEntity``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique entity identifier (UUID) to soft-delete | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteEntityRequest struct via the builder pattern


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


## DeleteNotificationChannel

> DeleteNotificationChannel(ctx, id).Execute()

Delete a notification channel



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
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60002" // string | Unique notification channel UUID to delete

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.DeleteNotificationChannel(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.DeleteNotificationChannel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique notification channel UUID to delete | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteNotificationChannelRequest struct via the builder pattern


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


## DeleteTemplate

> DeleteTemplate(ctx, id).Execute()

Delete a template



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010010" // string | UUID or unique slug of the template to delete

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.DeleteTemplate(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.DeleteTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | UUID or unique slug of the template to delete | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteTemplateRequest struct via the builder pattern


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
	r, err := apiClient.MCPAPI.DeleteWorkspace(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.DeleteWorkspace``: %v\n", err)
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
	r, err := apiClient.MCPAPI.DeleteWorkspaceView(context.Background(), id, viewId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.DeleteWorkspaceView``: %v\n", err)
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


## GetAttribute

> AttributeResponse GetAttribute(ctx, id).Execute()

Get an attribute by ID



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | UUID of the attribute to fetch

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.GetAttribute(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetAttribute``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAttribute`: AttributeResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetAttribute`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | UUID of the attribute to fetch | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAttributeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**AttributeResponse**](AttributeResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetAttributeReferenceConfig

> ReferenceConfigResponse GetAttributeReferenceConfig(ctx, id).Execute()

Get reference configuration for an attribute



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | UUID of the Reference attribute

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.GetAttributeReferenceConfig(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetAttributeReferenceConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAttributeReferenceConfig`: ReferenceConfigResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetAttributeReferenceConfig`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | UUID of the Reference attribute | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAttributeReferenceConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ReferenceConfigResponse**](ReferenceConfigResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

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
	openapiclient "github.com/omnismith-sdk/go"
)

func main() {
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60001" // string | Unique automation UUID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.GetAutomation(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetAutomation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAutomation`: AutomationResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetAutomation`: %v\n", resp)
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


## GetDashboard

> DashboardResponse GetDashboard(ctx, id).Execute()

Get a dashboard by ID



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
	id := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Dashboard unique identifier (UUID)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.GetDashboard(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetDashboard``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDashboard`: DashboardResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetDashboard`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Dashboard unique identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDashboardRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**DashboardResponse**](DashboardResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetDashboardBlock

> DashboardBlockResponse GetDashboardBlock(ctx, dashboardId, blockId).Execute()

Get a dashboard block by ID



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
	dashboardId := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Parent dashboard unique identifier (UUID)
	blockId := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6c" // string | Dashboard block unique identifier (UUID)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.GetDashboardBlock(context.Background(), dashboardId, blockId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetDashboardBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDashboardBlock`: DashboardBlockResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetDashboardBlock`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dashboardId** | **string** | Parent dashboard unique identifier (UUID) | 
**blockId** | **string** | Dashboard block unique identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetDashboardBlockRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**DashboardBlockResponse**](DashboardBlockResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetEntity

> EntityResponse GetEntity(ctx, id).AttributeKey(attributeKey).Execute()

Get an entity record by ID



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | Unique entity identifier (UUID)
	attributeKey := "slug" // string | Format for attribute_values dictionary keys: \"id\" for attribute UUIDs or \"slug\" for human-readable attribute slugs (optional) (default to "id")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.GetEntity(context.Background(), id).AttributeKey(attributeKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetEntity``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetEntity`: EntityResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetEntity`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique entity identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetEntityRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **attributeKey** | **string** | Format for attribute_values dictionary keys: \&quot;id\&quot; for attribute UUIDs or \&quot;slug\&quot; for human-readable attribute slugs | [default to &quot;id&quot;]

### Return type

[**EntityResponse**](EntityResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetEntityChart

> GetEntityChart200Response GetEntityChart(ctx, id).AttributeIds(attributeIds).Start(start).End(end).AggregateFunc(aggregateFunc).BucketWidth(bucketWidth).Execute()

Get entity chart time-series data



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | Unique entity identifier (UUID)
	attributeIds := "018b2f1b-8c1a-75b3-8000-7f0000010010,018b2f1b-8c1a-75b3-8000-7f0000010011" // string | Comma-separated metric attribute UUIDs to aggregate
	start := int32(1774396800) // int32 | Start timestamp as Unix epoch in seconds
	end := int32(1774483200) // int32 | End timestamp as Unix epoch in seconds
	aggregateFunc := "avg" // string | Aggregation function applied within each bucket (optional) (default to "avg")
	bucketWidth := "1 hour" // string | Time bucket width interval (e.g. 1 minute, 5 minutes, 1 hour, 1 day) (optional) (default to "1 hour")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.GetEntityChart(context.Background(), id).AttributeIds(attributeIds).Start(start).End(end).AggregateFunc(aggregateFunc).BucketWidth(bucketWidth).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetEntityChart``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetEntityChart`: GetEntityChart200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetEntityChart`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique entity identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetEntityChartRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **attributeIds** | **string** | Comma-separated metric attribute UUIDs to aggregate | 
 **start** | **int32** | Start timestamp as Unix epoch in seconds | 
 **end** | **int32** | End timestamp as Unix epoch in seconds | 
 **aggregateFunc** | **string** | Aggregation function applied within each bucket | [default to &quot;avg&quot;]
 **bucketWidth** | **string** | Time bucket width interval (e.g. 1 minute, 5 minutes, 1 hour, 1 day) | [default to &quot;1 hour&quot;]

### Return type

[**GetEntityChart200Response**](GetEntityChart200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetEntityHistory

> GetEntityHistory200Response GetEntityHistory(ctx, id).Page(page).Limit(limit).SortBy(sortBy).SortDirection(sortDirection).Search(search).AttributeIds(attributeIds).Start(start).End(end).AuthorEmail(authorEmail).Execute()

Get entity dimension change history



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/omnismith-sdk/go"
)

func main() {
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | Unique entity identifier (UUID)
	page := int32(1) // int32 | 1-based page number for pagination (optional) (default to 1)
	limit := int32(20) // int32 | Number of history records per page (1-100) (optional) (default to 20)
	sortBy := "created_at" // string | Field to sort change logs by (optional) (default to "created_at")
	sortDirection := "desc" // string | Sort direction: \"asc\" (ascending) or \"desc\" (descending) (optional) (default to "desc")
	search := "Electronics" // string | Free-text search filter matching against old and new attribute values (optional)
	attributeIds := "018b2f1b-8c1a-75b3-8000-7f0000010002,018b2f1b-8c1a-75b3-8000-7f0000010003" // string | Comma-separated attribute UUIDs to filter change history (optional)
	start := time.Now() // time.Time | Filter change records occurring on or after this timestamp (ISO 8601 or YYYY-MM-DD HH:MM:SS format) (optional)
	end := time.Now() // time.Time | Filter change records occurring on or before this timestamp (ISO 8601 or YYYY-MM-DD HH:MM:SS format) (optional)
	authorEmail := "demo@omnismith.io" // string | Filter change records by author or actor email (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.GetEntityHistory(context.Background(), id).Page(page).Limit(limit).SortBy(sortBy).SortDirection(sortDirection).Search(search).AttributeIds(attributeIds).Start(start).End(end).AuthorEmail(authorEmail).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetEntityHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetEntityHistory`: GetEntityHistory200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetEntityHistory`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique entity identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetEntityHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** | 1-based page number for pagination | [default to 1]
 **limit** | **int32** | Number of history records per page (1-100) | [default to 20]
 **sortBy** | **string** | Field to sort change logs by | [default to &quot;created_at&quot;]
 **sortDirection** | **string** | Sort direction: \&quot;asc\&quot; (ascending) or \&quot;desc\&quot; (descending) | [default to &quot;desc&quot;]
 **search** | **string** | Free-text search filter matching against old and new attribute values | 
 **attributeIds** | **string** | Comma-separated attribute UUIDs to filter change history | 
 **start** | **time.Time** | Filter change records occurring on or after this timestamp (ISO 8601 or YYYY-MM-DD HH:MM:SS format) | 
 **end** | **time.Time** | Filter change records occurring on or before this timestamp (ISO 8601 or YYYY-MM-DD HH:MM:SS format) | 
 **authorEmail** | **string** | Filter change records by author or actor email | 

### Return type

[**GetEntityHistory200Response**](GetEntityHistory200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetMarketplaceBlueprint

> GetMarketplaceBlueprint200Response GetMarketplaceBlueprint(ctx, id).Execute()

Get marketplace blueprint details



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
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60003" // string | Unique marketplace blueprint UUID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.GetMarketplaceBlueprint(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetMarketplaceBlueprint``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMarketplaceBlueprint`: GetMarketplaceBlueprint200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetMarketplaceBlueprint`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique marketplace blueprint UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetMarketplaceBlueprintRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**GetMarketplaceBlueprint200Response**](GetMarketplaceBlueprint200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetNotificationChannel

> NotificationChannelResponse GetNotificationChannel(ctx, id).Execute()

Get a notification channel by ID



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
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60002" // string | Unique notification channel UUID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.GetNotificationChannel(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetNotificationChannel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetNotificationChannel`: NotificationChannelResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetNotificationChannel`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique notification channel UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetNotificationChannelRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**NotificationChannelResponse**](NotificationChannelResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetProjectSchema

> ProjectSchemaResponse GetProjectSchema(ctx).Execute()

Get complete project schema graph



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
	resp, r, err := apiClient.MCPAPI.GetProjectSchema(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetProjectSchema``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetProjectSchema`: ProjectSchemaResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetProjectSchema`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetProjectSchemaRequest struct via the builder pattern


### Return type

[**ProjectSchemaResponse**](ProjectSchemaResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTemplate

> TemplateResponse GetTemplate(ctx, id).Execute()

Get a template by ID or slug



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010010" // string | UUID or unique slug of the template to retrieve

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.GetTemplate(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTemplate`: TemplateResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetTemplate`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | UUID or unique slug of the template to retrieve | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTemplateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**TemplateResponse**](TemplateResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetUsageInsights

> UsageInsightsResponse GetUsageInsights(ctx).Execute()

Get current tier usage insights



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
	resp, r, err := apiClient.MCPAPI.GetUsageInsights(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetUsageInsights``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetUsageInsights`: UsageInsightsResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetUsageInsights`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetUsageInsightsRequest struct via the builder pattern


### Return type

[**UsageInsightsResponse**](UsageInsightsResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
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
	resp, r, err := apiClient.MCPAPI.GetWorkspace(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetWorkspace``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetWorkspace`: WorkspaceDetailsResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetWorkspace`: %v\n", resp)
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
	resp, r, err := apiClient.MCPAPI.GetWorkspaceView(context.Background(), id, viewId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.GetWorkspaceView``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetWorkspaceView`: WorkspaceViewResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.GetWorkspaceView`: %v\n", resp)
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


## IngestEntityMetrics

> IngestEntityMetrics(ctx, id).IngestMetricsRequest(ingestMetricsRequest).Execute()

Ingest high-frequency metric observations for an entity



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | Unique entity identifier (UUID)
	ingestMetricsRequest := *openapiclient.NewIngestMetricsRequest() // IngestMetricsRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.IngestEntityMetrics(context.Background(), id).IngestMetricsRequest(ingestMetricsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.IngestEntityMetrics``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique entity identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiIngestEntityMetricsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **ingestMetricsRequest** | [**IngestMetricsRequest**](IngestMetricsRequest.md) |  | 

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


## InstallMarketplaceBlueprint

> InstallMarketplaceBlueprint(ctx, id).InstallMarketplaceBlueprintRequest(installMarketplaceBlueprintRequest).Execute()

Install a marketplace blueprint into a project



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
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60003" // string | Unique UUID of the blueprint to install
	installMarketplaceBlueprintRequest := *openapiclient.NewInstallMarketplaceBlueprintRequest("01912ecb-4654-7890-a1b2-c3d4e5f60011") // InstallMarketplaceBlueprintRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.InstallMarketplaceBlueprint(context.Background(), id).InstallMarketplaceBlueprintRequest(installMarketplaceBlueprintRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.InstallMarketplaceBlueprint``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique UUID of the blueprint to install | 

### Other Parameters

Other parameters are passed through a pointer to a apiInstallMarketplaceBlueprintRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **installMarketplaceBlueprintRequest** | [**InstallMarketplaceBlueprintRequest**](InstallMarketplaceBlueprintRequest.md) |  | 

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


## ListAttributeItems

> ListAttributeItems200Response ListAttributeItems(ctx, id).Execute()

List items of an attribute



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | UUID of the List-type attribute

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.ListAttributeItems(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.ListAttributeItems``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAttributeItems`: ListAttributeItems200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.ListAttributeItems`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | UUID of the List-type attribute | 

### Other Parameters

Other parameters are passed through a pointer to a apiListAttributeItemsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ListAttributeItems200Response**](ListAttributeItems200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListAttributes

> ListAttributes200Response ListAttributes(ctx).Execute()

List all attributes



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
	resp, r, err := apiClient.MCPAPI.ListAttributes(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.ListAttributes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAttributes`: ListAttributes200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.ListAttributes`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListAttributesRequest struct via the builder pattern


### Return type

[**ListAttributes200Response**](ListAttributes200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListAuditLogs

> ListAuditLogs200Response ListAuditLogs(ctx).Page(page).Limit(limit).SortBy(sortBy).SortDirection(sortDirection).Search(search).EventType(eventType).ResourceType(resourceType).ResourceId(resourceId).AuthorEmail(authorEmail).Start(start).End(end).Execute()

List project audit logs



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
    "time"
	openapiclient "github.com/omnismith-sdk/go"
)

func main() {
	page := int32(1) // int32 | 1-based page number for pagination (optional) (default to 1)
	limit := int32(20) // int32 | Number of audit log records per page (1-100) (optional) (default to 20)
	sortBy := "occurred_at" // string | Field to sort audit log entries by (optional) (default to "occurred_at")
	sortDirection := "desc" // string | Sort direction: \"asc\" (ascending) or \"desc\" (descending) (optional) (default to "desc")
	search := "entity.created" // string | Text search filter across event_type, resource_type, resource_id, author_email, and value (optional)
	eventType := "entity.created" // string | Filter by single or comma-separated event types (e.g. \"entity.created,entity.updated\") (optional)
	resourceType := "entity" // string | Filter by single or comma-separated resource types (e.g. \"entity,template,attribute\") (optional)
	resourceId := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | Filter by exact resource unique identifier (UUID) (optional)
	authorEmail := "demo@omnismith.io" // string | Filter by actor or author email address (optional)
	start := time.Now() // time.Time | Filter audit records occurring on or after this timestamp (ISO 8601 format) (optional)
	end := time.Now() // time.Time | Filter audit records occurring on or before this timestamp (ISO 8601 format) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.ListAuditLogs(context.Background()).Page(page).Limit(limit).SortBy(sortBy).SortDirection(sortDirection).Search(search).EventType(eventType).ResourceType(resourceType).ResourceId(resourceId).AuthorEmail(authorEmail).Start(start).End(end).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.ListAuditLogs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAuditLogs`: ListAuditLogs200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.ListAuditLogs`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListAuditLogsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int32** | 1-based page number for pagination | [default to 1]
 **limit** | **int32** | Number of audit log records per page (1-100) | [default to 20]
 **sortBy** | **string** | Field to sort audit log entries by | [default to &quot;occurred_at&quot;]
 **sortDirection** | **string** | Sort direction: \&quot;asc\&quot; (ascending) or \&quot;desc\&quot; (descending) | [default to &quot;desc&quot;]
 **search** | **string** | Text search filter across event_type, resource_type, resource_id, author_email, and value | 
 **eventType** | **string** | Filter by single or comma-separated event types (e.g. \&quot;entity.created,entity.updated\&quot;) | 
 **resourceType** | **string** | Filter by single or comma-separated resource types (e.g. \&quot;entity,template,attribute\&quot;) | 
 **resourceId** | **string** | Filter by exact resource unique identifier (UUID) | 
 **authorEmail** | **string** | Filter by actor or author email address | 
 **start** | **time.Time** | Filter audit records occurring on or after this timestamp (ISO 8601 format) | 
 **end** | **time.Time** | Filter audit records occurring on or before this timestamp (ISO 8601 format) | 

### Return type

[**ListAuditLogs200Response**](ListAuditLogs200Response.md)

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
	templateId := "01912ecb-4654-7890-a1b2-c3d4e5f60088" // string | Filter automations scoped to a specific entity template UUID (optional)
	isEnabled := true // bool | Filter automations by active enabled status (true for active rules, false for paused rules) (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.ListAutomations(context.Background()).TemplateId(templateId).IsEnabled(isEnabled).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.ListAutomations``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAutomations`: []AutomationResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.ListAutomations`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListAutomationsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
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


## ListDashboardBlocks

> ListDashboardBlocks200Response ListDashboardBlocks(ctx, dashboardId).Execute()

List all blocks in a dashboard



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
	dashboardId := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Parent dashboard unique identifier (UUID)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.ListDashboardBlocks(context.Background(), dashboardId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.ListDashboardBlocks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDashboardBlocks`: ListDashboardBlocks200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.ListDashboardBlocks`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dashboardId** | **string** | Parent dashboard unique identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiListDashboardBlocksRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ListDashboardBlocks200Response**](ListDashboardBlocks200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListDashboards

> ListDashboards200Response ListDashboards(ctx).Execute()

List all dashboards



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
	resp, r, err := apiClient.MCPAPI.ListDashboards(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.ListDashboards``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDashboards`: ListDashboards200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.ListDashboards`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListDashboardsRequest struct via the builder pattern


### Return type

[**ListDashboards200Response**](ListDashboards200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListNotificationChannels

> ListNotificationChannels200Response ListNotificationChannels(ctx).Execute()

List notification channels



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
	resp, r, err := apiClient.MCPAPI.ListNotificationChannels(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.ListNotificationChannels``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListNotificationChannels`: ListNotificationChannels200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.ListNotificationChannels`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListNotificationChannelsRequest struct via the builder pattern


### Return type

[**ListNotificationChannels200Response**](ListNotificationChannels200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTemplateEntityCounts

> ListTemplateEntityCounts200Response ListTemplateEntityCounts(ctx).Execute()

List entity counts per template



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
	resp, r, err := apiClient.MCPAPI.ListTemplateEntityCounts(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.ListTemplateEntityCounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTemplateEntityCounts`: ListTemplateEntityCounts200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.ListTemplateEntityCounts`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListTemplateEntityCountsRequest struct via the builder pattern


### Return type

[**ListTemplateEntityCounts200Response**](ListTemplateEntityCounts200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTemplates

> ListTemplates200Response ListTemplates(ctx).Execute()

List all templates



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
	resp, r, err := apiClient.MCPAPI.ListTemplates(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.ListTemplates``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTemplates`: ListTemplates200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.ListTemplates`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListTemplatesRequest struct via the builder pattern


### Return type

[**ListTemplates200Response**](ListTemplates200Response.md)

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
	resp, r, err := apiClient.MCPAPI.ListWorkspaces(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.ListWorkspaces``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListWorkspaces`: ListWorkspaces200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.ListWorkspaces`: %v\n", resp)
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


## PatchAttribute

> PatchAttribute(ctx, id).PatchAttributeRequest(patchAttributeRequest).Execute()

Patch an attribute (granular partial update)



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | UUID of the attribute to patch
	patchAttributeRequest := *openapiclient.NewPatchAttributeRequest() // PatchAttributeRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.PatchAttribute(context.Background(), id).PatchAttributeRequest(patchAttributeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.PatchAttribute``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | UUID of the attribute to patch | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchAttributeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **patchAttributeRequest** | [**PatchAttributeRequest**](PatchAttributeRequest.md) |  | 

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


## PatchTemplate

> PatchTemplate(ctx, id).PatchTemplateRequest(patchTemplateRequest).Execute()

Patch a template (granular partial update)



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010010" // string | UUID or unique slug of the template to patch
	patchTemplateRequest := *openapiclient.NewPatchTemplateRequest() // PatchTemplateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.PatchTemplate(context.Background(), id).PatchTemplateRequest(patchTemplateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.PatchTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | UUID or unique slug of the template to patch | 

### Other Parameters

Other parameters are passed through a pointer to a apiPatchTemplateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **patchTemplateRequest** | [**PatchTemplateRequest**](PatchTemplateRequest.md) |  | 

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


## ResolveDashboardBlock

> ResolvedBlockResponse ResolveDashboardBlock(ctx, dashboardId, blockId).Execute()

Resolve a dashboard block to its computed data



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
	dashboardId := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Parent dashboard unique identifier (UUID)
	blockId := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6c" // string | Dashboard block unique identifier (UUID) to resolve and compute

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.ResolveDashboardBlock(context.Background(), dashboardId, blockId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.ResolveDashboardBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ResolveDashboardBlock`: ResolvedBlockResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.ResolveDashboardBlock`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dashboardId** | **string** | Parent dashboard unique identifier (UUID) | 
**blockId** | **string** | Dashboard block unique identifier (UUID) to resolve and compute | 

### Other Parameters

Other parameters are passed through a pointer to a apiResolveDashboardBlockRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**ResolvedBlockResponse**](ResolvedBlockResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SearchEntities

> SearchEntities200Response SearchEntities(ctx, templateId).SearchEntitiesRequest(searchEntitiesRequest).Limit(limit).Offset(offset).SortField(sortField).SortDirection(sortDirection).AttributeKey(attributeKey).Execute()

Search entities with filtering, sorting, and pagination



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
	templateId := "product_catalog" // string | Template UUID or human-readable template slug
	searchEntitiesRequest := *openapiclient.NewSearchEntitiesRequest() // SearchEntitiesRequest | 
	limit := int32(50) // int32 | Maximum number of entity records to return (1-100) (optional) (default to 50)
	offset := int32(0) // int32 | Zero-based pagination offset (optional) (default to 0)
	sortField := "created_at" // string | Attribute UUID, attribute slug, or standard field (id, created_at, updated_at, deleted_at) to sort by (optional)
	sortDirection := "desc" // string | Sort direction: \"asc\" (ascending) or \"desc\" (descending) (optional) (default to "asc")
	attributeKey := "slug" // string | Format for attribute_values dictionary keys: \"id\" for attribute UUIDs or \"slug\" for human-readable attribute slugs (optional) (default to "id")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.SearchEntities(context.Background(), templateId).SearchEntitiesRequest(searchEntitiesRequest).Limit(limit).Offset(offset).SortField(sortField).SortDirection(sortDirection).AttributeKey(attributeKey).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.SearchEntities``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SearchEntities`: SearchEntities200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.SearchEntities`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | Template UUID or human-readable template slug | 

### Other Parameters

Other parameters are passed through a pointer to a apiSearchEntitiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **searchEntitiesRequest** | [**SearchEntitiesRequest**](SearchEntitiesRequest.md) |  | 
 **limit** | **int32** | Maximum number of entity records to return (1-100) | [default to 50]
 **offset** | **int32** | Zero-based pagination offset | [default to 0]
 **sortField** | **string** | Attribute UUID, attribute slug, or standard field (id, created_at, updated_at, deleted_at) to sort by | 
 **sortDirection** | **string** | Sort direction: \&quot;asc\&quot; (ascending) or \&quot;desc\&quot; (descending) | [default to &quot;asc&quot;]
 **attributeKey** | **string** | Format for attribute_values dictionary keys: \&quot;id\&quot; for attribute UUIDs or \&quot;slug\&quot; for human-readable attribute slugs | [default to &quot;id&quot;]

### Return type

[**SearchEntities200Response**](SearchEntities200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SearchMarketplaceBlueprints

> SearchMarketplaceBlueprints200Response SearchMarketplaceBlueprints(ctx).Search(search).Keywords(keywords).Limit(limit).Offset(offset).SortBy(sortBy).SortDirection(sortDirection).Featured(featured).Execute()

Search marketplace blueprints



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
	search := "crm pipeline" // string | Free-text search filter across blueprint title and description (optional)
	keywords := "crm,sales,leads" // string | Comma-separated keywords or tags to filter blueprints (optional)
	limit := int32(20) // int32 | Number of blueprint records to return per page (max 100) (optional) (default to 20)
	offset := int32(0) // int32 | Number of blueprint records to skip for pagination (optional) (default to 0)
	sortBy := "installs" // string | Field to sort blueprint results by (optional) (default to "created_at")
	sortDirection := "desc" // string | Sort direction order (ascending or descending) (optional) (default to "desc")
	featured := true // bool | Filter to return only curated and featured marketplace blueprints (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.SearchMarketplaceBlueprints(context.Background()).Search(search).Keywords(keywords).Limit(limit).Offset(offset).SortBy(sortBy).SortDirection(sortDirection).Featured(featured).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.SearchMarketplaceBlueprints``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SearchMarketplaceBlueprints`: SearchMarketplaceBlueprints200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.SearchMarketplaceBlueprints`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSearchMarketplaceBlueprintsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **search** | **string** | Free-text search filter across blueprint title and description | 
 **keywords** | **string** | Comma-separated keywords or tags to filter blueprints | 
 **limit** | **int32** | Number of blueprint records to return per page (max 100) | [default to 20]
 **offset** | **int32** | Number of blueprint records to skip for pagination | [default to 0]
 **sortBy** | **string** | Field to sort blueprint results by | [default to &quot;created_at&quot;]
 **sortDirection** | **string** | Sort direction order (ascending or descending) | [default to &quot;desc&quot;]
 **featured** | **bool** | Filter to return only curated and featured marketplace blueprints | 

### Return type

[**SearchMarketplaceBlueprints200Response**](SearchMarketplaceBlueprints200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SetAttributeItems

> SetAttributeItems(ctx, id).SetListItemsRequest(setListItemsRequest).Execute()

Set list items for an attribute (replaces all existing items)



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | UUID of the List-type attribute
	setListItemsRequest := *openapiclient.NewSetListItemsRequest([]openapiclient.ListItemInput{*openapiclient.NewListItemInput("Red")}) // SetListItemsRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.SetAttributeItems(context.Background(), id).SetListItemsRequest(setListItemsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.SetAttributeItems``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | UUID of the List-type attribute | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetAttributeItemsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **setListItemsRequest** | [**SetListItemsRequest**](SetListItemsRequest.md) |  | 

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


## SetAttributeReferenceConfig

> SetAttributeReferenceConfig(ctx, id).SetReferenceConfigRequest(setReferenceConfigRequest).Execute()

Set or update reference configuration for an attribute



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | UUID of the Reference attribute
	setReferenceConfigRequest := *openapiclient.NewSetReferenceConfigRequest("018b2f1b-8c1a-75b3-8000-7f0000010002", "018b2f1b-8c1a-75b3-8000-7f0000010003") // SetReferenceConfigRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.SetAttributeReferenceConfig(context.Background(), id).SetReferenceConfigRequest(setReferenceConfigRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.SetAttributeReferenceConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | UUID of the Reference attribute | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetAttributeReferenceConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **setReferenceConfigRequest** | [**SetReferenceConfigRequest**](SetReferenceConfigRequest.md) |  | 

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


## TestNotificationChannel

> TestNotificationChannel200Response TestNotificationChannel(ctx, id).TestNotificationChannelRequest(testNotificationChannelRequest).Execute()

Send a test notification message



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
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60002" // string | Unique notification channel UUID to test
	testNotificationChannelRequest := *openapiclient.NewTestNotificationChannelRequest() // TestNotificationChannelRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.TestNotificationChannel(context.Background(), id).TestNotificationChannelRequest(testNotificationChannelRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.TestNotificationChannel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TestNotificationChannel`: TestNotificationChannel200Response
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.TestNotificationChannel`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique notification channel UUID to test | 

### Other Parameters

Other parameters are passed through a pointer to a apiTestNotificationChannelRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **testNotificationChannelRequest** | [**TestNotificationChannelRequest**](TestNotificationChannelRequest.md) |  | 

### Return type

[**TestNotificationChannel200Response**](TestNotificationChannel200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
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
	openapiclient "github.com/omnismith-sdk/go"
)

func main() {
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60001" // string | Unique automation UUID to toggle
	toggleAutomationRequest := *openapiclient.NewToggleAutomationRequest(true) // ToggleAutomationRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MCPAPI.ToggleAutomation(context.Background(), id).ToggleAutomationRequest(toggleAutomationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.ToggleAutomation``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ToggleAutomation`: AutomationResponse
	fmt.Fprintf(os.Stdout, "Response from `MCPAPI.ToggleAutomation`: %v\n", resp)
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


## UpdateAttribute

> UpdateAttribute(ctx, id).UpdateAttributeRequest(updateAttributeRequest).Execute()

Update an attribute (full replacement)



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | UUID of the attribute to update
	updateAttributeRequest := *openapiclient.NewUpdateAttributeRequest("Product Color Variant") // UpdateAttributeRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.UpdateAttribute(context.Background(), id).UpdateAttributeRequest(updateAttributeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.UpdateAttribute``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | UUID of the attribute to update | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateAttributeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateAttributeRequest** | [**UpdateAttributeRequest**](UpdateAttributeRequest.md) |  | 

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
	openapiclient "github.com/omnismith-sdk/go"
)

func main() {
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60001" // string | Unique automation UUID to update
	updateAutomationRequest := *openapiclient.NewUpdateAutomationRequest() // UpdateAutomationRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.UpdateAutomation(context.Background(), id).UpdateAutomationRequest(updateAutomationRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.UpdateAutomation``: %v\n", err)
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


## UpdateDashboard

> UpdateDashboard(ctx, id).UpdateDashboardRequest(updateDashboardRequest).Execute()

Update a dashboard



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
	id := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Dashboard unique identifier (UUID) to update
	updateDashboardRequest := *openapiclient.NewUpdateDashboardRequest() // UpdateDashboardRequest | Dashboard update payload

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.UpdateDashboard(context.Background(), id).UpdateDashboardRequest(updateDashboardRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.UpdateDashboard``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Dashboard unique identifier (UUID) to update | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateDashboardRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateDashboardRequest** | [**UpdateDashboardRequest**](UpdateDashboardRequest.md) | Dashboard update payload | 

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


## UpdateDashboardBlock

> UpdateDashboardBlock(ctx, dashboardId, blockId).UpdateDashboardBlockRequest(updateDashboardBlockRequest).Execute()

Update a dashboard block



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
	dashboardId := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6b" // string | Parent dashboard unique identifier (UUID)
	blockId := "0190a1b2-c3d4-7e8f-9a0b-1c2d3e4f5a6c" // string | Dashboard block unique identifier (UUID) to update
	updateDashboardBlockRequest := *openapiclient.NewUpdateDashboardBlockRequest() // UpdateDashboardBlockRequest | Dashboard block update payload

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.UpdateDashboardBlock(context.Background(), dashboardId, blockId).UpdateDashboardBlockRequest(updateDashboardBlockRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.UpdateDashboardBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dashboardId** | **string** | Parent dashboard unique identifier (UUID) | 
**blockId** | **string** | Dashboard block unique identifier (UUID) to update | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateDashboardBlockRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateDashboardBlockRequest** | [**UpdateDashboardBlockRequest**](UpdateDashboardBlockRequest.md) | Dashboard block update payload | 

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


## UpdateEntity

> UpdateEntity(ctx, id).UpdateEntityRequest(updateEntityRequest).Execute()

Update entity attribute values



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010000" // string | Unique entity identifier (UUID)
	updateEntityRequest := *openapiclient.NewUpdateEntityRequest() // UpdateEntityRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.UpdateEntity(context.Background(), id).UpdateEntityRequest(updateEntityRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.UpdateEntity``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique entity identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateEntityRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateEntityRequest** | [**UpdateEntityRequest**](UpdateEntityRequest.md) |  | 

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


## UpdateNotificationChannel

> UpdateNotificationChannel(ctx, id).UpdateNotificationChannelRequest(updateNotificationChannelRequest).Execute()

Update a notification channel



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
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60002" // string | Unique notification channel UUID to update
	updateNotificationChannelRequest := *openapiclient.NewUpdateNotificationChannelRequest() // UpdateNotificationChannelRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.UpdateNotificationChannel(context.Background(), id).UpdateNotificationChannelRequest(updateNotificationChannelRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.UpdateNotificationChannel``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique notification channel UUID to update | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateNotificationChannelRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateNotificationChannelRequest** | [**UpdateNotificationChannelRequest**](UpdateNotificationChannelRequest.md) |  | 

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


## UpdateTemplate

> UpdateTemplate(ctx, id).UpdateTemplateRequest(updateTemplateRequest).Execute()

Update a template (full replacement)



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
	id := "018b2f1b-8c1a-75b3-8000-7f0000010010" // string | UUID or unique slug of the template to update
	updateTemplateRequest := *openapiclient.NewUpdateTemplateRequest("Product SKU") // UpdateTemplateRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MCPAPI.UpdateTemplate(context.Background(), id).UpdateTemplateRequest(updateTemplateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.UpdateTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | UUID or unique slug of the template to update | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateTemplateRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateTemplateRequest** | [**UpdateTemplateRequest**](UpdateTemplateRequest.md) |  | 

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
	r, err := apiClient.MCPAPI.UpdateWorkspace(context.Background(), id).UpdateWorkspaceRequest(updateWorkspaceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.UpdateWorkspace``: %v\n", err)
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
	r, err := apiClient.MCPAPI.UpdateWorkspaceView(context.Background(), id, viewId).UpdateWorkspaceViewRequest(updateWorkspaceViewRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MCPAPI.UpdateWorkspaceView``: %v\n", err)
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

