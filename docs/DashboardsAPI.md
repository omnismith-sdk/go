# \DashboardsAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateDashboard**](DashboardsAPI.md#CreateDashboard) | **Post** /dashboards | Create a new dashboard
[**DeleteDashboard**](DashboardsAPI.md#DeleteDashboard) | **Delete** /dashboards/{id} | Delete a dashboard
[**GetDashboard**](DashboardsAPI.md#GetDashboard) | **Get** /dashboards/{id} | Get a dashboard by ID
[**ListDashboards**](DashboardsAPI.md#ListDashboards) | **Get** /dashboards | List all dashboards
[**UpdateDashboard**](DashboardsAPI.md#UpdateDashboard) | **Put** /dashboards/{id} | Update a dashboard



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
	resp, r, err := apiClient.DashboardsAPI.CreateDashboard(context.Background()).CreateDashboardRequest(createDashboardRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DashboardsAPI.CreateDashboard``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateDashboard`: CreateDashboard201Response
	fmt.Fprintf(os.Stdout, "Response from `DashboardsAPI.CreateDashboard`: %v\n", resp)
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
	r, err := apiClient.DashboardsAPI.DeleteDashboard(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DashboardsAPI.DeleteDashboard``: %v\n", err)
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
	resp, r, err := apiClient.DashboardsAPI.GetDashboard(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DashboardsAPI.GetDashboard``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetDashboard`: DashboardResponse
	fmt.Fprintf(os.Stdout, "Response from `DashboardsAPI.GetDashboard`: %v\n", resp)
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
	resp, r, err := apiClient.DashboardsAPI.ListDashboards(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DashboardsAPI.ListDashboards``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListDashboards`: ListDashboards200Response
	fmt.Fprintf(os.Stdout, "Response from `DashboardsAPI.ListDashboards`: %v\n", resp)
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
	r, err := apiClient.DashboardsAPI.UpdateDashboard(context.Background(), id).UpdateDashboardRequest(updateDashboardRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `DashboardsAPI.UpdateDashboard``: %v\n", err)
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

