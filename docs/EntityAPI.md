# \EntityAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateEntity**](EntityAPI.md#CreateEntity) | **Post** /entities | Create a new entity
[**DeleteEntity**](EntityAPI.md#DeleteEntity) | **Delete** /entities/{id} | Delete an entity
[**ExportEntities**](EntityAPI.md#ExportEntities) | **Post** /entities/export/{template_id} | Export entities to CSV
[**GetEntity**](EntityAPI.md#GetEntity) | **Get** /entities/{id} | Get an entity
[**GetEntityChart**](EntityAPI.md#GetEntityChart) | **Get** /entities/{id}/chart | Get entity chart time-series data
[**GetEntityHistory**](EntityAPI.md#GetEntityHistory) | **Get** /entities/{id}/history | Get entity history
[**ImportEntities**](EntityAPI.md#ImportEntities) | **Post** /entities/import/{template_id} | Import entities from CSV
[**SearchEntities**](EntityAPI.md#SearchEntities) | **Post** /entities/search/{template_id} | Search entities
[**UpdateEntity**](EntityAPI.md#UpdateEntity) | **Put** /entities/{id} | Update an entity



## CreateEntity

> CreateAttributeItem201Response CreateEntity(ctx).CreateEntityRequest(createEntityRequest).Execute()

Create a new entity

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
	// response from `CreateEntity`: CreateAttributeItem201Response
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

[**CreateAttributeItem201Response**](CreateAttributeItem201Response.md)

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

Delete an entity

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

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
**id** | **string** |  | 

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
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportEntities

> *os.File ExportEntities(ctx, templateId).ExportEntitiesRequest(exportEntitiesRequest).SortField(sortField).SortDirection(sortDirection).Execute()

Export entities to CSV



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
	templateId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Template ID
	exportEntitiesRequest := *openapiclient.NewExportEntitiesRequest() // ExportEntitiesRequest | 
	sortField := "sortField_example" // string | Attribute ID to sort by (UUID) OR one of: id, created_at, updated_at, deleted_at (optional)
	sortDirection := "sortDirection_example" // string | Sort direction (only used when sort_field is provided) (optional) (default to "asc")

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
**templateId** | **string** | Template ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportEntitiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **exportEntitiesRequest** | [**ExportEntitiesRequest**](ExportEntitiesRequest.md) |  | 
 **sortField** | **string** | Attribute ID to sort by (UUID) OR one of: id, created_at, updated_at, deleted_at | 
 **sortDirection** | **string** | Sort direction (only used when sort_field is provided) | [default to &quot;asc&quot;]

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

> EntityResponse GetEntity(ctx, id).Execute()

Get an entity

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.GetEntity(context.Background(), id).Execute()
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
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetEntityRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


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
	id := "id_example" // string | Entity ID
	attributeIds := "attributeIds_example" // string | Comma-separated attribute IDs
	start := int32(56) // int32 | Start timestamp (Unix seconds)
	end := int32(56) // int32 | End timestamp (Unix seconds)
	aggregateFunc := "aggregateFunc_example" // string | Aggregate function (optional) (default to "avg")
	bucketWidth := "bucketWidth_example" // string | Time bucket width (PostgreSQL interval) (optional) (default to "1 hour")

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
**id** | **string** | Entity ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetEntityChartRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **attributeIds** | **string** | Comma-separated attribute IDs | 
 **start** | **int32** | Start timestamp (Unix seconds) | 
 **end** | **int32** | End timestamp (Unix seconds) | 
 **aggregateFunc** | **string** | Aggregate function | [default to &quot;avg&quot;]
 **bucketWidth** | **string** | Time bucket width (PostgreSQL interval) | [default to &quot;1 hour&quot;]

### Return type

[**GetEntityChart200Response**](GetEntityChart200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetEntityHistory

> GetEntityHistory200Response GetEntityHistory(ctx, id).Page(page).Limit(limit).SortBy(sortBy).SortDirection(sortDirection).Search(search).AttributeIds(attributeIds).Start(start).End(end).AuthorEmail(authorEmail).Execute()

Get entity history

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
	id := "id_example" // string | Entity ID
	page := int32(56) // int32 |  (optional) (default to 1)
	limit := int32(56) // int32 |  (optional) (default to 20)
	sortBy := "sortBy_example" // string |  (optional) (default to "created_at")
	sortDirection := "sortDirection_example" // string |  (optional) (default to "desc")
	search := "search_example" // string |  (optional)
	attributeIds := "attributeIds_example" // string |  (optional)
	start := time.Now() // time.Time | Filter logs created after this timestamp (optional)
	end := time.Now() // time.Time | Filter logs created before this timestamp (optional)
	authorEmail := "authorEmail_example" // string | Filter logs by author email (optional)

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
**id** | **string** | Entity ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetEntityHistoryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **page** | **int32** |  | [default to 1]
 **limit** | **int32** |  | [default to 20]
 **sortBy** | **string** |  | [default to &quot;created_at&quot;]
 **sortDirection** | **string** |  | [default to &quot;desc&quot;]
 **search** | **string** |  | 
 **attributeIds** | **string** |  | 
 **start** | **time.Time** | Filter logs created after this timestamp | 
 **end** | **time.Time** | Filter logs created before this timestamp | 
 **authorEmail** | **string** | Filter logs by author email | 

### Return type

[**GetEntityHistory200Response**](GetEntityHistory200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ImportEntities

> ImportEntities200Response ImportEntities(ctx, templateId).File(file).Execute()

Import entities from CSV



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
	templateId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Template ID
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
**templateId** | **string** | Template ID | 

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


## SearchEntities

> SearchEntities200Response SearchEntities(ctx, templateId).SearchEntitiesRequest(searchEntitiesRequest).Limit(limit).Offset(offset).SortField(sortField).SortDirection(sortDirection).Execute()

Search entities

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
	templateId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Template ID
	searchEntitiesRequest := *openapiclient.NewSearchEntitiesRequest() // SearchEntitiesRequest | 
	limit := int32(56) // int32 | Number of results (optional) (default to 50)
	offset := int32(56) // int32 | Pagination offset (optional) (default to 0)
	sortField := "sortField_example" // string | Attribute ID to sort by (UUID) OR one of: id, created_at, updated_at, deleted_at (optional)
	sortDirection := "sortDirection_example" // string | Sort direction (only used when sort_field is provided) (optional) (default to "asc")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityAPI.SearchEntities(context.Background(), templateId).SearchEntitiesRequest(searchEntitiesRequest).Limit(limit).Offset(offset).SortField(sortField).SortDirection(sortDirection).Execute()
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
**templateId** | **string** | Template ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiSearchEntitiesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **searchEntitiesRequest** | [**SearchEntitiesRequest**](SearchEntitiesRequest.md) |  | 
 **limit** | **int32** | Number of results | [default to 50]
 **offset** | **int32** | Pagination offset | [default to 0]
 **sortField** | **string** | Attribute ID to sort by (UUID) OR one of: id, created_at, updated_at, deleted_at | 
 **sortDirection** | **string** | Sort direction (only used when sort_field is provided) | [default to &quot;asc&quot;]

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


## UpdateEntity

> UpdateEntity(ctx, id).UpdateEntityRequest(updateEntityRequest).Execute()

Update an entity

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 
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
**id** | **string** |  | 

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

