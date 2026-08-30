# \EntityAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateEntity**](EntityAPI.md#CreateEntity) | **Post** /entities | Create a new dynamic entity
[**DeleteEntity**](EntityAPI.md#DeleteEntity) | **Delete** /entities/{id} | Soft-delete an entity record
[**ExportEntities**](EntityAPI.md#ExportEntities) | **Post** /entities/export/{template_id} | Export entities to structured CSV file
[**GetEntity**](EntityAPI.md#GetEntity) | **Get** /entities/{id} | Get an entity record by ID
[**GetEntityChart**](EntityAPI.md#GetEntityChart) | **Get** /entities/{id}/chart | Get entity chart time-series data
[**GetEntityHistory**](EntityAPI.md#GetEntityHistory) | **Get** /entities/{id}/history | Get entity dimension change history
[**ImportEntities**](EntityAPI.md#ImportEntities) | **Post** /entities/import/{template_id} | Import entities from structured CSV file
[**IngestEntityMetrics**](EntityAPI.md#IngestEntityMetrics) | **Post** /entities/{id}/metrics | Ingest high-frequency metric observations for an entity
[**SearchEntities**](EntityAPI.md#SearchEntities) | **Post** /entities/search/{template_id} | Search entities with filtering, sorting, and pagination
[**SemanticSearchEntities**](EntityAPI.md#SemanticSearchEntities) | **Post** /entities/semantic-search | Perform semantic vector similarity search on entities
[**UpdateEntity**](EntityAPI.md#UpdateEntity) | **Patch** /entities/{id} | Update entity attribute values



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
	resp, r, err := apiClient.EntityAPI.CreateEntity(context.Background()).CreateEntityRequest(createEntityRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityAPI.CreateEntity``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateEntity`: CreateEntity201Response
	fmt.Fprintf(os.Stdout, "Response from `EntityAPI.CreateEntity`: %v\n", resp)
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
	r, err := apiClient.EntityAPI.DeleteEntity(context.Background(), id).Execute()
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


## ExportEntities

> *os.File ExportEntities(ctx, templateId).ExportEntitiesRequest(exportEntitiesRequest).SortField(sortField).SortDirection(sortDirection).Execute()

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
	sortField := "created_at" // string | Attribute UUID, attribute slug, or standard field (id, created_at, updated_at, deleted_at) to sort by (optional)
	sortDirection := "asc" // string | Sort direction: \"asc\" (ascending) or \"desc\" (descending) (optional) (default to "asc")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.ExportEntities(context.Background(), templateId).ExportEntitiesRequest(exportEntitiesRequest).SortField(sortField).SortDirection(sortDirection).Execute()
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
	resp, r, err := apiClient.EntityAPI.GetEntity(context.Background(), id).AttributeKey(attributeKey).Execute()
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
	resp, r, err := apiClient.EntityAPI.GetEntityChart(context.Background(), id).AttributeIds(attributeIds).Start(start).End(end).AggregateFunc(aggregateFunc).BucketWidth(bucketWidth).Execute()
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
	resp, r, err := apiClient.EntityAPI.GetEntityHistory(context.Background(), id).Page(page).Limit(limit).SortBy(sortBy).SortDirection(sortDirection).Search(search).AttributeIds(attributeIds).Start(start).End(end).AuthorEmail(authorEmail).Execute()
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

> ImportEntities200Response ImportEntities(ctx, templateId).File(file).Execute()

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.ImportEntities(context.Background(), templateId).File(file).Execute()
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
	r, err := apiClient.EntityAPI.IngestEntityMetrics(context.Background(), id).IngestMetricsRequest(ingestMetricsRequest).Execute()
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
	resp, r, err := apiClient.EntityAPI.SearchEntities(context.Background(), templateId).SearchEntitiesRequest(searchEntitiesRequest).Limit(limit).Offset(offset).SortField(sortField).SortDirection(sortDirection).AttributeKey(attributeKey).Execute()
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


## SemanticSearchEntities

> []SemanticSearchResultItem SemanticSearchEntities(ctx).SemanticSearchEntitiesRequest(semanticSearchEntitiesRequest).Execute()

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.SemanticSearchEntities(context.Background()).SemanticSearchEntitiesRequest(semanticSearchEntitiesRequest).Execute()
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
	r, err := apiClient.EntityAPI.UpdateEntity(context.Background(), id).UpdateEntityRequest(updateEntityRequest).Execute()
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

