# \EntityAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AggregateEntities**](EntityAPI.md#AggregateEntities) | **Post** /entities/aggregate/{template_id} | Count, sum, average, min or max entities, optionally grouped by attributes
[**BatchExecuteEntityAction**](EntityAPI.md#BatchExecuteEntityAction) | **Post** /entities/batch/actions/{slug} | Execute an action on a selection of entities
[**BatchWriteEntities**](EntityAPI.md#BatchWriteEntities) | **Post** /entities/batch | Apply a batch of mixed entity creates, updates, replaces, and deletes
[**CreateEntity**](EntityAPI.md#CreateEntity) | **Post** /entities/template/{template} | Create a new dynamic entity
[**DeleteEntity**](EntityAPI.md#DeleteEntity) | **Delete** /entities/{id} | Soft-delete an entity record
[**ExecuteEntityAction**](EntityAPI.md#ExecuteEntityAction) | **Post** /entities/{id}/actions/{slug} | Execute an action on an entity
[**ExportEntities**](EntityAPI.md#ExportEntities) | **Post** /entities/export/{template_id} | Export entities to structured CSV file
[**GetEntity**](EntityAPI.md#GetEntity) | **Get** /entities/{id} | Get an entity record by ID
[**GetEntityChart**](EntityAPI.md#GetEntityChart) | **Get** /entities/{id}/chart | Get entity chart time-series data
[**GetEntityHistory**](EntityAPI.md#GetEntityHistory) | **Get** /entities/{id}/history | Get entity dimension change history
[**ImportEntities**](EntityAPI.md#ImportEntities) | **Post** /entities/import/{template_id} | Import entities from structured CSV file
[**IngestEntityMetrics**](EntityAPI.md#IngestEntityMetrics) | **Post** /entities/{id}/metrics | Ingest high-frequency metric observations for an entity
[**ListEntityActions**](EntityAPI.md#ListEntityActions) | **Get** /entities/{id}/actions | List the actions available on an entity
[**ReplaceEntity**](EntityAPI.md#ReplaceEntity) | **Put** /entities/{id} | Replace all non-metric attributes of an entity
[**SearchEntities**](EntityAPI.md#SearchEntities) | **Post** /entities/search/{template_id} | Search entities with filtering, sorting, and pagination
[**SemanticSearchEntities**](EntityAPI.md#SemanticSearchEntities) | **Post** /entities/semantic-search | Perform semantic vector similarity search on entities
[**UpdateEntity**](EntityAPI.md#UpdateEntity) | **Patch** /entities/{id} | Update entity attribute values



## AggregateEntities

> AggregateEntities200Response AggregateEntities(ctx, templateId).AggregateEntitiesRequest(aggregateEntitiesRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Count, sum, average, min or max entities, optionally grouped by attributes



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
	templateId := "tenant_user" // string | Template UUID or human-readable template slug
	aggregateEntitiesRequest := *openapiclient.NewAggregateEntitiesRequest([]openapiclient.AggregateEntitiesRequestAggregationsInner{*openapiclient.NewAggregateEntitiesRequestAggregationsInner("sum")}) // AggregateEntitiesRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.AggregateEntities(context.Background(), templateId).AggregateEntitiesRequest(aggregateEntitiesRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.AggregateEntities``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AggregateEntities`: AggregateEntities200Response
	fmt.Fprintf(os.Stdout, "Response from `EntityAPI.AggregateEntities`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | Template UUID or human-readable template slug | 

### Other Parameters

Other parameters are passed through a pointer to a apiAggregateEntitiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **aggregateEntitiesRequest** | [**AggregateEntitiesRequest**](AggregateEntitiesRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**AggregateEntities200Response**](AggregateEntities200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BatchExecuteEntityAction

> BatchExecuteEntityActionResponse BatchExecuteEntityAction(ctx, slug).BatchExecuteEntityActionRequest(batchExecuteEntityActionRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Execute an action on a selection of entities



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
	slug := "confirm_attendance" // string | Action slug, as listed by `GET /templates/{templateId}/actions` or `GET /entities/{id}/actions`
	batchExecuteEntityActionRequest := *openapiclient.NewBatchExecuteEntityActionRequest([]string{"EntityIds_example"}) // BatchExecuteEntityActionRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.BatchExecuteEntityAction(context.Background(), slug).BatchExecuteEntityActionRequest(batchExecuteEntityActionRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.BatchExecuteEntityAction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BatchExecuteEntityAction`: BatchExecuteEntityActionResponse
	fmt.Fprintf(os.Stdout, "Response from `EntityAPI.BatchExecuteEntityAction`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**slug** | **string** | Action slug, as listed by &#x60;GET /templates/{templateId}/actions&#x60; or &#x60;GET /entities/{id}/actions&#x60; | 

### Other Parameters

Other parameters are passed through a pointer to a apiBatchExecuteEntityActionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **batchExecuteEntityActionRequest** | [**BatchExecuteEntityActionRequest**](BatchExecuteEntityActionRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**BatchExecuteEntityActionResponse**](BatchExecuteEntityActionResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BatchWriteEntities

> BatchWriteEntitiesResponse BatchWriteEntities(ctx).BatchWriteEntitiesRequest(batchWriteEntitiesRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Apply a batch of mixed entity creates, updates, replaces, and deletes



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
	batchWriteEntitiesRequest := *openapiclient.NewBatchWriteEntitiesRequest([]openapiclient.BatchOperationInput{*openapiclient.NewBatchOperationInput("update")}) // BatchWriteEntitiesRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.BatchWriteEntities(context.Background()).BatchWriteEntitiesRequest(batchWriteEntitiesRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.BatchWriteEntities``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BatchWriteEntities`: BatchWriteEntitiesResponse
	fmt.Fprintf(os.Stdout, "Response from `EntityAPI.BatchWriteEntities`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiBatchWriteEntitiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **batchWriteEntitiesRequest** | [**BatchWriteEntitiesRequest**](BatchWriteEntitiesRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**BatchWriteEntitiesResponse**](BatchWriteEntitiesResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateEntity

> CreateEntity201Response CreateEntity(ctx, template).XOmnismithProjectId(xOmnismithProjectId).CreateEntityRequest(createEntityRequest).Execute()

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
	template := "article" // string | Template UUID or human-readable slug
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)
	createEntityRequest := *openapiclient.NewCreateEntityRequest(map[string]EntityAttributesInputValue{"key": *openapiclient.NewEntityAttributesInputValue(float32(1), "Op_example")}) // CreateEntityRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.CreateEntity(context.Background(), template).XOmnismithProjectId(xOmnismithProjectId).CreateEntityRequest(createEntityRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.CreateEntity``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateEntity`: CreateEntity201Response
	fmt.Fprintf(os.Stdout, "Response from `EntityAPI.CreateEntity`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**template** | **string** | Template UUID or human-readable slug | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateEntityRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 
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


## DeleteEntity

> DeleteEntity(ctx, id).XOmnismithProjectId(xOmnismithProjectId).Execute()

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
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.EntityAPI.DeleteEntity(context.Background(), id).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.DeleteEntity``: %v\n", err)
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


## ExecuteEntityAction

> ExecuteEntityActionResponse ExecuteEntityAction(ctx, id, slug).XOmnismithProjectId(xOmnismithProjectId).ExecuteEntityActionRequest(executeEntityActionRequest).Execute()

Execute an action on an entity



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
	slug := "confirm_attendance" // string | Action slug, as listed by `GET /entities/{id}/actions`
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)
	executeEntityActionRequest := *openapiclient.NewExecuteEntityActionRequest() // ExecuteEntityActionRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.ExecuteEntityAction(context.Background(), id, slug).XOmnismithProjectId(xOmnismithProjectId).ExecuteEntityActionRequest(executeEntityActionRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.ExecuteEntityAction``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExecuteEntityAction`: ExecuteEntityActionResponse
	fmt.Fprintf(os.Stdout, "Response from `EntityAPI.ExecuteEntityAction`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique entity identifier (UUID) | 
**slug** | **string** | Action slug, as listed by &#x60;GET /entities/{id}/actions&#x60; | 

### Other Parameters

Other parameters are passed through a pointer to a apiExecuteEntityActionRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 
 **executeEntityActionRequest** | [**ExecuteEntityActionRequest**](ExecuteEntityActionRequest.md) |  | 

### Return type

[**ExecuteEntityActionResponse**](ExecuteEntityActionResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportEntities

> *os.File ExportEntities(ctx, templateId).ExportEntitiesRequest(exportEntitiesRequest).XOmnismithProjectId(xOmnismithProjectId).SortField(sortField).SortDirection(sortDirection).Execute()

Export entities to structured CSV file



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
	templateId := "018b2f1b-8c1a-75b3-8000-7f0000010001" // string | Unique identifier (UUID) of the template schema to export
	exportEntitiesRequest := *openapiclient.NewExportEntitiesRequest() // ExportEntitiesRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)
	sortField := "created_at" // string | Attribute UUID, attribute slug, or standard field (id, created_at, updated_at, deleted_at) to sort by (optional)
	sortDirection := "asc" // string | Sort direction: \"asc\" (ascending) or \"desc\" (descending) (optional) (default to "asc")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.ExportEntities(context.Background(), templateId).ExportEntitiesRequest(exportEntitiesRequest).XOmnismithProjectId(xOmnismithProjectId).SortField(sortField).SortDirection(sortDirection).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.ExportEntities``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportEntities`: *os.File
	fmt.Fprintf(os.Stdout, "Response from `EntityAPI.ExportEntities`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | Unique identifier (UUID) of the template schema to export | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportEntitiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **exportEntitiesRequest** | [**ExportEntitiesRequest**](ExportEntitiesRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 
 **sortField** | **string** | Attribute UUID, attribute slug, or standard field (id, created_at, updated_at, deleted_at) to sort by | 
 **sortDirection** | **string** | Sort direction: \&quot;asc\&quot; (ascending) or \&quot;desc\&quot; (descending) | [default to &quot;asc&quot;]

### Return type

[***os.File**](*os.File.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: text/csv, application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetEntity

> EntityResponse GetEntity(ctx, id).XOmnismithProjectId(xOmnismithProjectId).Verbose(verbose).Fields(fields).Execute()

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
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)
	verbose := false // bool | When true, attribute_values is an array of EntityAttributeValue items with attribute id, slug, raw value, resolved custom_value and reference_entity_id. When false (default), attribute_values is a compact object mapping attribute slug to display value, with the ids behind list, reference and file labels in list_item_ids, reference_entity_ids and file_ids. (optional) (default to false)
	fields := []string{"Inner_example"} // []string | Comma-separated list of attribute slugs, attribute UUIDs, or root fields to project (e.g. \"title,status\"). When specified, only the requested attributes are fetched and returned in attribute_values, avoiding database hydration for unneeded attributes and significantly reducing response payload size. If omitted, all attributes defined on the template are returned. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.GetEntity(context.Background(), id).XOmnismithProjectId(xOmnismithProjectId).Verbose(verbose).Fields(fields).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.GetEntity``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetEntity`: EntityResponse
	fmt.Fprintf(os.Stdout, "Response from `EntityAPI.GetEntity`: %v\n", resp)
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

 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 
 **verbose** | **bool** | When true, attribute_values is an array of EntityAttributeValue items with attribute id, slug, raw value, resolved custom_value and reference_entity_id. When false (default), attribute_values is a compact object mapping attribute slug to display value, with the ids behind list, reference and file labels in list_item_ids, reference_entity_ids and file_ids. | [default to false]
 **fields** | **[]string** | Comma-separated list of attribute slugs, attribute UUIDs, or root fields to project (e.g. \&quot;title,status\&quot;). When specified, only the requested attributes are fetched and returned in attribute_values, avoiding database hydration for unneeded attributes and significantly reducing response payload size. If omitted, all attributes defined on the template are returned. | 

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

> GetEntityChart200Response GetEntityChart(ctx, id).AttributeIds(attributeIds).Start(start).End(end).XOmnismithProjectId(xOmnismithProjectId).AggregateFunc(aggregateFunc).BucketWidth(bucketWidth).Execute()

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
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)
	aggregateFunc := "avg" // string | Aggregation function applied within each bucket (optional) (default to "avg")
	bucketWidth := "1 hour" // string | Time bucket width interval (e.g. 1 minute, 5 minutes, 1 hour, 1 day) (optional) (default to "1 hour")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.GetEntityChart(context.Background(), id).AttributeIds(attributeIds).Start(start).End(end).XOmnismithProjectId(xOmnismithProjectId).AggregateFunc(aggregateFunc).BucketWidth(bucketWidth).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.GetEntityChart``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetEntityChart`: GetEntityChart200Response
	fmt.Fprintf(os.Stdout, "Response from `EntityAPI.GetEntityChart`: %v\n", resp)
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
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 
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

> GetEntityHistory200Response GetEntityHistory(ctx, id).XOmnismithProjectId(xOmnismithProjectId).Page(page).Limit(limit).SortBy(sortBy).SortDirection(sortDirection).Search(search).AttributeIds(attributeIds).Start(start).End(end).AuthorEmail(authorEmail).Execute()

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
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)
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
	resp, r, err := apiClient.EntityAPI.GetEntityHistory(context.Background(), id).XOmnismithProjectId(xOmnismithProjectId).Page(page).Limit(limit).SortBy(sortBy).SortDirection(sortDirection).Search(search).AttributeIds(attributeIds).Start(start).End(end).AuthorEmail(authorEmail).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.GetEntityHistory``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetEntityHistory`: GetEntityHistory200Response
	fmt.Fprintf(os.Stdout, "Response from `EntityAPI.GetEntityHistory`: %v\n", resp)
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

 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 
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


## ImportEntities

> ImportEntities200Response ImportEntities(ctx, templateId).File(file).XOmnismithProjectId(xOmnismithProjectId).Execute()

Import entities from structured CSV file



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
	templateId := "018b2f1b-8c1a-75b3-8000-7f0000010001" // string | Unique identifier (UUID) of the template schema to import entities into
	file := os.NewFile(1234, "some_file") // *os.File | CSV file exported from the export endpoint or matching its format
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.ImportEntities(context.Background(), templateId).File(file).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.ImportEntities``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ImportEntities`: ImportEntities200Response
	fmt.Fprintf(os.Stdout, "Response from `EntityAPI.ImportEntities`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | Unique identifier (UUID) of the template schema to import entities into | 

### Other Parameters

Other parameters are passed through a pointer to a apiImportEntitiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **file** | ***os.File** | CSV file exported from the export endpoint or matching its format | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**ImportEntities200Response**](ImportEntities200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## IngestEntityMetrics

> IngestEntityMetrics(ctx, id).IngestMetricsRequest(ingestMetricsRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

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
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.EntityAPI.IngestEntityMetrics(context.Background(), id).IngestMetricsRequest(ingestMetricsRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.IngestEntityMetrics``: %v\n", err)
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


## ListEntityActions

> ListEntityActions200Response ListEntityActions(ctx, id).XOmnismithProjectId(xOmnismithProjectId).Execute()

List the actions available on an entity



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
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.ListEntityActions(context.Background(), id).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.ListEntityActions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListEntityActions`: ListEntityActions200Response
	fmt.Fprintf(os.Stdout, "Response from `EntityAPI.ListEntityActions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique entity identifier (UUID) | 

### Other Parameters

Other parameters are passed through a pointer to a apiListEntityActionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**ListEntityActions200Response**](ListEntityActions200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ReplaceEntity

> ReplaceEntity(ctx, id).ReplaceEntityRequest(replaceEntityRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Replace all non-metric attributes of an entity



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
	replaceEntityRequest := *openapiclient.NewReplaceEntityRequest(map[string]EntityAttributesInputValue{"key": *openapiclient.NewEntityAttributesInputValue(float32(1), "Op_example")}) // ReplaceEntityRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.EntityAPI.ReplaceEntity(context.Background(), id).ReplaceEntityRequest(replaceEntityRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.ReplaceEntity``: %v\n", err)
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

Other parameters are passed through a pointer to a apiReplaceEntityRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **replaceEntityRequest** | [**ReplaceEntityRequest**](ReplaceEntityRequest.md) |  | 
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


## SearchEntities

> SearchEntities200Response SearchEntities(ctx, templateId).SearchEntitiesRequest(searchEntitiesRequest).XOmnismithProjectId(xOmnismithProjectId).Limit(limit).Offset(offset).SortField(sortField).SortDirection(sortDirection).Execute()

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
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)
	limit := int32(50) // int32 | Maximum number of entity records to return (1-100) (optional) (default to 50)
	offset := int32(0) // int32 | Zero-based pagination offset (optional) (default to 0)
	sortField := "created_at" // string | Attribute UUID, attribute slug, or standard field (id, created_at, updated_at, deleted_at) to sort by (optional)
	sortDirection := "desc" // string | Sort direction: \"asc\" (ascending) or \"desc\" (descending) (optional) (default to "asc")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.SearchEntities(context.Background(), templateId).SearchEntitiesRequest(searchEntitiesRequest).XOmnismithProjectId(xOmnismithProjectId).Limit(limit).Offset(offset).SortField(sortField).SortDirection(sortDirection).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.SearchEntities``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SearchEntities`: SearchEntities200Response
	fmt.Fprintf(os.Stdout, "Response from `EntityAPI.SearchEntities`: %v\n", resp)
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
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 
 **limit** | **int32** | Maximum number of entity records to return (1-100) | [default to 50]
 **offset** | **int32** | Zero-based pagination offset | [default to 0]
 **sortField** | **string** | Attribute UUID, attribute slug, or standard field (id, created_at, updated_at, deleted_at) to sort by | 
 **sortDirection** | **string** | Sort direction: \&quot;asc\&quot; (ascending) or \&quot;desc\&quot; (descending) | [default to &quot;asc&quot;]

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


## SemanticSearchEntities

> []SemanticSearchResultItem SemanticSearchEntities(ctx).SemanticSearchEntitiesRequest(semanticSearchEntitiesRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Perform semantic vector similarity search on entities



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
	semanticSearchEntitiesRequest := *openapiclient.NewSemanticSearchEntitiesRequest([]float32{float32(0.0123)}) // SemanticSearchEntitiesRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.SemanticSearchEntities(context.Background()).SemanticSearchEntitiesRequest(semanticSearchEntitiesRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.SemanticSearchEntities``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SemanticSearchEntities`: []SemanticSearchResultItem
	fmt.Fprintf(os.Stdout, "Response from `EntityAPI.SemanticSearchEntities`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSemanticSearchEntitiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **semanticSearchEntitiesRequest** | [**SemanticSearchEntitiesRequest**](SemanticSearchEntitiesRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**[]SemanticSearchResultItem**](SemanticSearchResultItem.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateEntity

> UpdateEntity(ctx, id).UpdateEntityRequest(updateEntityRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

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
	updateEntityRequest := *openapiclient.NewUpdateEntityRequest(map[string]EntityAttributesInputValue{"key": *openapiclient.NewEntityAttributesInputValue(float32(1), "Op_example")}) // UpdateEntityRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.EntityAPI.UpdateEntity(context.Background(), id).UpdateEntityRequest(updateEntityRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.UpdateEntity``: %v\n", err)
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

