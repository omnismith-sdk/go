# \TemplatesAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateTemplate**](TemplatesAPI.md#CreateTemplate) | **Post** /templates | Create a new template
[**DeleteTemplate**](TemplatesAPI.md#DeleteTemplate) | **Delete** /templates/{id} | Delete a template
[**GetTemplate**](TemplatesAPI.md#GetTemplate) | **Get** /templates/{id} | Get a template by ID or slug
[**ListTemplateEntityCounts**](TemplatesAPI.md#ListTemplateEntityCounts) | **Get** /templates/entity-counts | List entity counts per template
[**ListTemplates**](TemplatesAPI.md#ListTemplates) | **Get** /templates | List all templates
[**PatchTemplate**](TemplatesAPI.md#PatchTemplate) | **Patch** /templates/{id} | Patch a template (granular partial update)
[**UpdateTemplate**](TemplatesAPI.md#UpdateTemplate) | **Put** /templates/{id} | Update a template (full replacement)



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
	resp, r, err := apiClient.TemplatesAPI.CreateTemplate(context.Background()).CreateTemplateRequest(createTemplateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.CreateTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTemplate`: CreateTemplate201Response
	fmt.Fprintf(os.Stdout, "Response from `TemplatesAPI.CreateTemplate`: %v\n", resp)
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
	r, err := apiClient.TemplatesAPI.DeleteTemplate(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.DeleteTemplate``: %v\n", err)
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
	resp, r, err := apiClient.TemplatesAPI.GetTemplate(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.GetTemplate``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTemplate`: TemplateResponse
	fmt.Fprintf(os.Stdout, "Response from `TemplatesAPI.GetTemplate`: %v\n", resp)
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
	resp, r, err := apiClient.TemplatesAPI.ListTemplateEntityCounts(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.ListTemplateEntityCounts``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTemplateEntityCounts`: ListTemplateEntityCounts200Response
	fmt.Fprintf(os.Stdout, "Response from `TemplatesAPI.ListTemplateEntityCounts`: %v\n", resp)
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
	resp, r, err := apiClient.TemplatesAPI.ListTemplates(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.ListTemplates``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTemplates`: ListTemplates200Response
	fmt.Fprintf(os.Stdout, "Response from `TemplatesAPI.ListTemplates`: %v\n", resp)
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
	r, err := apiClient.TemplatesAPI.PatchTemplate(context.Background(), id).PatchTemplateRequest(patchTemplateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.PatchTemplate``: %v\n", err)
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
	r, err := apiClient.TemplatesAPI.UpdateTemplate(context.Background(), id).UpdateTemplateRequest(updateTemplateRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `TemplatesAPI.UpdateTemplate``: %v\n", err)
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

