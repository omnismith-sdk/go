# \AuditLogAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListAuditLogs**](AuditLogAPI.md#ListAuditLogs) | **Get** /audit-logs | List project audit logs



## ListAuditLogs

> ListAuditLogs200Response ListAuditLogs(ctx).XOmnismithProjectId(xOmnismithProjectId).Page(page).Limit(limit).SortBy(sortBy).SortDirection(sortDirection).Search(search).EventType(eventType).ResourceType(resourceType).ResourceId(resourceId).AuthorEmail(authorEmail).Start(start).End(end).Execute()

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
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)
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
	resp, r, err := apiClient.AuditLogAPI.ListAuditLogs(context.Background()).XOmnismithProjectId(xOmnismithProjectId).Page(page).Limit(limit).SortBy(sortBy).SortDirection(sortDirection).Search(search).EventType(eventType).ResourceType(resourceType).ResourceId(resourceId).AuthorEmail(authorEmail).Start(start).End(end).Execute()
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
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 
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

