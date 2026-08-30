# \AuditLogAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListAuditLogs**](AuditLogAPI.md#ListAuditLogs) | **Get** /audit-logs | List project audit logs



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
	resp, r, err := apiClient.AuditLogAPI.ListAuditLogs(context.Background()).Page(page).Limit(limit).SortBy(sortBy).SortDirection(sortDirection).Search(search).EventType(eventType).ResourceType(resourceType).ResourceId(resourceId).AuthorEmail(authorEmail).Start(start).End(end).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AuditLogAPI.ListAuditLogs``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAuditLogs`: ListAuditLogs200Response
	fmt.Fprintf(os.Stdout, "Response from `AuditLogAPI.ListAuditLogs`: %v\n", resp)
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

