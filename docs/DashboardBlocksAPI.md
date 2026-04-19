# \DashboardBlocksAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateDashboardBlock**](DashboardBlocksAPI.md#CreateDashboardBlock) | **Post** /dashboards/{dashboardId}/blocks | Create a new block in a dashboard
[**DeleteDashboardBlock**](DashboardBlocksAPI.md#DeleteDashboardBlock) | **Delete** /dashboards/{dashboardId}/blocks/{blockId} | Delete a dashboard block
[**GetDashboardBlock**](DashboardBlocksAPI.md#GetDashboardBlock) | **Get** /dashboards/{dashboardId}/blocks/{blockId} | Get a dashboard block by ID
[**ListDashboardBlocks**](DashboardBlocksAPI.md#ListDashboardBlocks) | **Get** /dashboards/{dashboardId}/blocks | List all blocks in a dashboard
[**ResolveDashboardBlock**](DashboardBlocksAPI.md#ResolveDashboardBlock) | **Get** /dashboards/{dashboardId}/blocks/{blockId}/resolve | Resolve a dashboard block to its computed data
[**UpdateDashboardBlock**](DashboardBlocksAPI.md#UpdateDashboardBlock) | **Put** /dashboards/{dashboardId}/blocks/{blockId} | Update a dashboard block



## CreateDashboardBlock

> CreateAttributeItem201Response CreateDashboardBlock(ctx, dashboardId).CreateDashboardBlockRequest(createDashboardBlockRequest).Execute()

Create a new block in a dashboard

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
	dashboardId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Dashboard ID
	createDashboardBlockRequest := *openapiclient.NewCreateDashboardBlockRequest("Type_example", "My Block") // CreateDashboardBlockRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DashboardBlocksAPI.CreateDashboardBlock(context.Background(), dashboardId).CreateDashboardBlockRequest(createDashboardBlockRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DashboardBlocksAPI.CreateDashboardBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateDashboardBlock`: CreateAttributeItem201Response
	fmt.Fprintf(os.Stdout, "Response from `DashboardBlocksAPI.CreateDashboardBlock`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dashboardId** | **string** | Dashboard ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateDashboardBlockRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createDashboardBlockRequest** | [**CreateDashboardBlockRequest**](CreateDashboardBlockRequest.md) |  | 

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
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	dashboardId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Dashboard ID
	blockId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Block ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.DashboardBlocksAPI.DeleteDashboardBlock(context.Background(), dashboardId, blockId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DashboardBlocksAPI.DeleteDashboardBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dashboardId** | **string** | Dashboard ID | 
**blockId** | **string** | Block ID | 

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
- **Accept**: Not defined

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
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	dashboardId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Dashboard ID
	blockId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Block ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DashboardBlocksAPI.GetDashboardBlock(context.Background(), dashboardId, blockId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DashboardBlocksAPI.GetDashboardBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDashboardBlock`: DashboardBlockResponse
	fmt.Fprintf(os.Stdout, "Response from `DashboardBlocksAPI.GetDashboardBlock`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dashboardId** | **string** | Dashboard ID | 
**blockId** | **string** | Block ID | 

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
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	dashboardId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Dashboard ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DashboardBlocksAPI.ListDashboardBlocks(context.Background(), dashboardId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DashboardBlocksAPI.ListDashboardBlocks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDashboardBlocks`: ListDashboardBlocks200Response
	fmt.Fprintf(os.Stdout, "Response from `DashboardBlocksAPI.ListDashboardBlocks`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dashboardId** | **string** | Dashboard ID | 

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
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	dashboardId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Dashboard ID
	blockId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Block ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.DashboardBlocksAPI.ResolveDashboardBlock(context.Background(), dashboardId, blockId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DashboardBlocksAPI.ResolveDashboardBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ResolveDashboardBlock`: ResolvedBlockResponse
	fmt.Fprintf(os.Stdout, "Response from `DashboardBlocksAPI.ResolveDashboardBlock`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dashboardId** | **string** | Dashboard ID | 
**blockId** | **string** | Block ID | 

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
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	dashboardId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Dashboard ID
	blockId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Block ID
	updateDashboardBlockRequest := *openapiclient.NewUpdateDashboardBlockRequest() // UpdateDashboardBlockRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.DashboardBlocksAPI.UpdateDashboardBlock(context.Background(), dashboardId, blockId).UpdateDashboardBlockRequest(updateDashboardBlockRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DashboardBlocksAPI.UpdateDashboardBlock``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**dashboardId** | **string** | Dashboard ID | 
**blockId** | **string** | Block ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateDashboardBlockRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateDashboardBlockRequest** | [**UpdateDashboardBlockRequest**](UpdateDashboardBlockRequest.md) |  | 

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

