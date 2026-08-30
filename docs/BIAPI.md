# \BIAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetBiSchema**](BIAPI.md#GetBiSchema) | **Get** /bi/schema | Get BI schema catalog
[**ListBiTemplateRows**](BIAPI.md#ListBiTemplateRows) | **Post** /bi/templates/{template_id}/rows | List flattened template rows for BI integration
[**ListBiTemplateTimeSeries**](BIAPI.md#ListBiTemplateTimeSeries) | **Post** /bi/templates/{template_id}/time-series | List aggregated time-series rows for BI integration



## GetBiSchema

> BiSchemaResponse GetBiSchema(ctx).Execute()

Get BI schema catalog



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
	resp, r, err := apiClient.BIAPI.GetBiSchema(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BIAPI.GetBiSchema``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetBiSchema`: BiSchemaResponse
	fmt.Fprintf(os.Stdout, "Response from `BIAPI.GetBiSchema`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetBiSchemaRequest struct via the builder pattern


### Return type

[**BiSchemaResponse**](BiSchemaResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListBiTemplateRows

> BiTemplateRowsResponse ListBiTemplateRows(ctx, templateId).BiListTemplateRowsRequest(biListTemplateRowsRequest).Limit(limit).Offset(offset).SortField(sortField).SortDirection(sortDirection).Execute()

List flattened template rows for BI integration



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
	templateId := "018b2f1b-8c1a-75b3-8000-7f0000010001" // string | Unique identifier (UUID) of the template schema to query
	biListTemplateRowsRequest := *openapiclient.NewBiListTemplateRowsRequest() // BiListTemplateRowsRequest | 
	limit := int32(50) // int32 | Maximum number of rows to return per page (1-100) (optional) (default to 50)
	offset := int32(0) // int32 | Zero-based pagination offset (optional) (default to 0)
	sortField := "created_at" // string | Attribute UUID, slug, or standard field (id, created_at, updated_at, deleted_at) to sort by (optional)
	sortDirection := "desc" // string | Sort direction: \"asc\" (ascending) or \"desc\" (descending) (optional) (default to "asc")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BIAPI.ListBiTemplateRows(context.Background(), templateId).BiListTemplateRowsRequest(biListTemplateRowsRequest).Limit(limit).Offset(offset).SortField(sortField).SortDirection(sortDirection).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BIAPI.ListBiTemplateRows``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListBiTemplateRows`: BiTemplateRowsResponse
	fmt.Fprintf(os.Stdout, "Response from `BIAPI.ListBiTemplateRows`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | Unique identifier (UUID) of the template schema to query | 

### Other Parameters

Other parameters are passed through a pointer to a apiListBiTemplateRowsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **biListTemplateRowsRequest** | [**BiListTemplateRowsRequest**](BiListTemplateRowsRequest.md) |  | 
 **limit** | **int32** | Maximum number of rows to return per page (1-100) | [default to 50]
 **offset** | **int32** | Zero-based pagination offset | [default to 0]
 **sortField** | **string** | Attribute UUID, slug, or standard field (id, created_at, updated_at, deleted_at) to sort by | 
 **sortDirection** | **string** | Sort direction: \&quot;asc\&quot; (ascending) or \&quot;desc\&quot; (descending) | [default to &quot;asc&quot;]

### Return type

[**BiTemplateRowsResponse**](BiTemplateRowsResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListBiTemplateTimeSeries

> BiTimeSeriesResponse ListBiTemplateTimeSeries(ctx, templateId).AttributeIds(attributeIds).Start(start).End(end).BiListTemplateRowsRequest(biListTemplateRowsRequest).AggregateFunc(aggregateFunc).BucketWidth(bucketWidth).Execute()

List aggregated time-series rows for BI integration



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
	templateId := "018b2f1b-8c1a-75b3-8000-7f0000010001" // string | Unique identifier (UUID) of the template schema
	attributeIds := "018b2f1b-8c1a-75b3-8000-7f0000010010,018b2f1b-8c1a-75b3-8000-7f0000010011" // string | Comma-separated metric attribute UUIDs to aggregate
	start := int32(1774396800) // int32 | Start timestamp as Unix epoch in seconds
	end := int32(1774483200) // int32 | End timestamp as Unix epoch in seconds
	biListTemplateRowsRequest := *openapiclient.NewBiListTemplateRowsRequest() // BiListTemplateRowsRequest | 
	aggregateFunc := "avg" // string | Aggregation function applied within each time bucket (optional) (default to "avg")
	bucketWidth := "1 hour" // string | Time bucket width interval (e.g. 1 minute, 5 minutes, 1 hour, 1 day) (optional) (default to "1 hour")

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.BIAPI.ListBiTemplateTimeSeries(context.Background(), templateId).AttributeIds(attributeIds).Start(start).End(end).BiListTemplateRowsRequest(biListTemplateRowsRequest).AggregateFunc(aggregateFunc).BucketWidth(bucketWidth).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `BIAPI.ListBiTemplateTimeSeries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListBiTemplateTimeSeries`: BiTimeSeriesResponse
	fmt.Fprintf(os.Stdout, "Response from `BIAPI.ListBiTemplateTimeSeries`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | Unique identifier (UUID) of the template schema | 

### Other Parameters

Other parameters are passed through a pointer to a apiListBiTemplateTimeSeriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **attributeIds** | **string** | Comma-separated metric attribute UUIDs to aggregate | 
 **start** | **int32** | Start timestamp as Unix epoch in seconds | 
 **end** | **int32** | End timestamp as Unix epoch in seconds | 
 **biListTemplateRowsRequest** | [**BiListTemplateRowsRequest**](BiListTemplateRowsRequest.md) |  | 
 **aggregateFunc** | **string** | Aggregation function applied within each time bucket | [default to &quot;avg&quot;]
 **bucketWidth** | **string** | Time bucket width interval (e.g. 1 minute, 5 minutes, 1 hour, 1 day) | [default to &quot;1 hour&quot;]

### Return type

[**BiTimeSeriesResponse**](BiTimeSeriesResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

