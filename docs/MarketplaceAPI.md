# \MarketplaceAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteMarketplaceBlueprint**](MarketplaceAPI.md#DeleteMarketplaceBlueprint) | **Delete** /marketplace/blueprints/{id} | Delete a marketplace blueprint
[**GetMarketplaceBlueprint**](MarketplaceAPI.md#GetMarketplaceBlueprint) | **Get** /marketplace/blueprints/{id} | Get marketplace blueprint details
[**InstallMarketplaceBlueprint**](MarketplaceAPI.md#InstallMarketplaceBlueprint) | **Post** /marketplace/blueprints/{id}/install | Install a marketplace blueprint into a project
[**ListMarketplaceKeywords**](MarketplaceAPI.md#ListMarketplaceKeywords) | **Get** /marketplace/keywords | List marketplace keywords
[**PublishMarketplaceBlueprint**](MarketplaceAPI.md#PublishMarketplaceBlueprint) | **Post** /marketplace/blueprints | Publish or update a marketplace blueprint
[**SearchMarketplaceBlueprints**](MarketplaceAPI.md#SearchMarketplaceBlueprints) | **Get** /marketplace/blueprints | Search marketplace blueprints



## DeleteMarketplaceBlueprint

> DeleteMarketplaceBlueprint(ctx, id).Execute()

Delete a marketplace blueprint



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
	id := "01912ecb-4654-7890-a1b2-c3d4e5f60003" // string | Unique blueprint UUID to delete

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.MarketplaceAPI.DeleteMarketplaceBlueprint(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MarketplaceAPI.DeleteMarketplaceBlueprint``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Unique blueprint UUID to delete | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteMarketplaceBlueprintRequest struct via the builder pattern


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
	resp, r, err := apiClient.MarketplaceAPI.GetMarketplaceBlueprint(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MarketplaceAPI.GetMarketplaceBlueprint``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetMarketplaceBlueprint`: GetMarketplaceBlueprint200Response
	fmt.Fprintf(os.Stdout, "Response from `MarketplaceAPI.GetMarketplaceBlueprint`: %v\n", resp)
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
	r, err := apiClient.MarketplaceAPI.InstallMarketplaceBlueprint(context.Background(), id).InstallMarketplaceBlueprintRequest(installMarketplaceBlueprintRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MarketplaceAPI.InstallMarketplaceBlueprint``: %v\n", err)
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


## ListMarketplaceKeywords

> ListMarketplaceKeywords200Response ListMarketplaceKeywords(ctx).Execute()

List marketplace keywords



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
	resp, r, err := apiClient.MarketplaceAPI.ListMarketplaceKeywords(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MarketplaceAPI.ListMarketplaceKeywords``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListMarketplaceKeywords`: ListMarketplaceKeywords200Response
	fmt.Fprintf(os.Stdout, "Response from `MarketplaceAPI.ListMarketplaceKeywords`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListMarketplaceKeywordsRequest struct via the builder pattern


### Return type

[**ListMarketplaceKeywords200Response**](ListMarketplaceKeywords200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PublishMarketplaceBlueprint

> GetMarketplaceBlueprint200Response PublishMarketplaceBlueprint(ctx).PublishMarketplaceBlueprintRequest(publishMarketplaceBlueprintRequest).Execute()

Publish or update a marketplace blueprint



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
	publishMarketplaceBlueprintRequest := *openapiclient.NewPublishMarketplaceBlueprintRequest("CRM Pipeline & Lead Tracker", []string{"TemplateIds_example"}) // PublishMarketplaceBlueprintRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MarketplaceAPI.PublishMarketplaceBlueprint(context.Background()).PublishMarketplaceBlueprintRequest(publishMarketplaceBlueprintRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MarketplaceAPI.PublishMarketplaceBlueprint``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PublishMarketplaceBlueprint`: GetMarketplaceBlueprint200Response
	fmt.Fprintf(os.Stdout, "Response from `MarketplaceAPI.PublishMarketplaceBlueprint`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPublishMarketplaceBlueprintRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **publishMarketplaceBlueprintRequest** | [**PublishMarketplaceBlueprintRequest**](PublishMarketplaceBlueprintRequest.md) |  | 

### Return type

[**GetMarketplaceBlueprint200Response**](GetMarketplaceBlueprint200Response.md)

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
	resp, r, err := apiClient.MarketplaceAPI.SearchMarketplaceBlueprints(context.Background()).Search(search).Keywords(keywords).Limit(limit).Offset(offset).SortBy(sortBy).SortDirection(sortDirection).Featured(featured).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MarketplaceAPI.SearchMarketplaceBlueprints``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SearchMarketplaceBlueprints`: SearchMarketplaceBlueprints200Response
	fmt.Fprintf(os.Stdout, "Response from `MarketplaceAPI.SearchMarketplaceBlueprints`: %v\n", resp)
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

