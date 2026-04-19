# \AttributesAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateAttribute**](AttributesAPI.md#CreateAttribute) | **Post** /attributes | Create a new attribute
[**CreateAttributeItem**](AttributesAPI.md#CreateAttributeItem) | **Post** /attributes/{id}/items | Add a list item to an attribute
[**DeleteAttribute**](AttributesAPI.md#DeleteAttribute) | **Delete** /attributes/{id} | Delete an attribute
[**DeleteAttributeItem**](AttributesAPI.md#DeleteAttributeItem) | **Delete** /attributes/{id}/items/{itemId} | Remove a list item from an attribute
[**DeleteAttributeReferenceConfig**](AttributesAPI.md#DeleteAttributeReferenceConfig) | **Delete** /attributes/{id}/reference | Delete reference configuration for an attribute
[**GetAttribute**](AttributesAPI.md#GetAttribute) | **Get** /attributes/{id} | Get an attribute
[**GetAttributeReferenceConfig**](AttributesAPI.md#GetAttributeReferenceConfig) | **Get** /attributes/{id}/reference | Get reference configuration for an attribute
[**GetProjectSchema**](AttributesAPI.md#GetProjectSchema) | **Get** /discovery/project-schema | Get complete project schema
[**ListAttributeItems**](AttributesAPI.md#ListAttributeItems) | **Get** /attributes/{id}/items | List items of an attribute
[**ListAttributes**](AttributesAPI.md#ListAttributes) | **Get** /attributes | List attributes
[**SetAttributeItems**](AttributesAPI.md#SetAttributeItems) | **Put** /attributes/{id}/items | Set list items for an attribute (replaces all existing items)
[**SetAttributeReferenceConfig**](AttributesAPI.md#SetAttributeReferenceConfig) | **Put** /attributes/{id}/reference | Set or update reference configuration for an attribute
[**UpdateAttribute**](AttributesAPI.md#UpdateAttribute) | **Put** /attributes/{id} | Update an attribute
[**UpdateAttributeItem**](AttributesAPI.md#UpdateAttributeItem) | **Put** /attributes/{id}/items/{itemId} | Update a list item of an attribute



## CreateAttribute

> CreateAttributeItem201Response CreateAttribute(ctx).CreateAttributeRequest(createAttributeRequest).Execute()

Create a new attribute

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
	createAttributeRequest := *openapiclient.NewCreateAttributeRequest("Color", int32(0), int32(0)) // CreateAttributeRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AttributesAPI.CreateAttribute(context.Background()).CreateAttributeRequest(createAttributeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AttributesAPI.CreateAttribute``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateAttribute`: CreateAttributeItem201Response
	fmt.Fprintf(os.Stdout, "Response from `AttributesAPI.CreateAttribute`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateAttributeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createAttributeRequest** | [**CreateAttributeRequest**](CreateAttributeRequest.md) |  | 

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


## CreateAttributeItem

> CreateAttributeItem201Response CreateAttributeItem(ctx, id).AddListItemRequest(addListItemRequest).Execute()

Add a list item to an attribute

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Attribute ID
	addListItemRequest := *openapiclient.NewAddListItemRequest("red") // AddListItemRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AttributesAPI.CreateAttributeItem(context.Background(), id).AddListItemRequest(addListItemRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AttributesAPI.CreateAttributeItem``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateAttributeItem`: CreateAttributeItem201Response
	fmt.Fprintf(os.Stdout, "Response from `AttributesAPI.CreateAttributeItem`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Attribute ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateAttributeItemRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **addListItemRequest** | [**AddListItemRequest**](AddListItemRequest.md) |  | 

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


## DeleteAttribute

> DeleteAttribute(ctx, id).Execute()

Delete an attribute

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AttributesAPI.DeleteAttribute(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AttributesAPI.DeleteAttribute``: %v\n", err)
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

Other parameters are passed through a pointer to a apiDeleteAttributeRequest struct via the builder pattern


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


## DeleteAttributeItem

> DeleteAttributeItem(ctx, id, itemId).Execute()

Remove a list item from an attribute

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Attribute ID
	itemId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | List Item ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AttributesAPI.DeleteAttributeItem(context.Background(), id, itemId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AttributesAPI.DeleteAttributeItem``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Attribute ID | 
**itemId** | **string** | List Item ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAttributeItemRequest struct via the builder pattern


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


## DeleteAttributeReferenceConfig

> DeleteAttributeReferenceConfig(ctx, id).Execute()

Delete reference configuration for an attribute

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Attribute ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AttributesAPI.DeleteAttributeReferenceConfig(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AttributesAPI.DeleteAttributeReferenceConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Attribute ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteAttributeReferenceConfigRequest struct via the builder pattern


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


## GetAttribute

> AttributeResponse GetAttribute(ctx, id).Execute()

Get an attribute

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AttributesAPI.GetAttribute(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AttributesAPI.GetAttribute``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAttribute`: AttributeResponse
	fmt.Fprintf(os.Stdout, "Response from `AttributesAPI.GetAttribute`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** |  | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAttributeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**AttributeResponse**](AttributeResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetAttributeReferenceConfig

> ReferenceConfigResponse GetAttributeReferenceConfig(ctx, id).Execute()

Get reference configuration for an attribute

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Attribute ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AttributesAPI.GetAttributeReferenceConfig(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AttributesAPI.GetAttributeReferenceConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetAttributeReferenceConfig`: ReferenceConfigResponse
	fmt.Fprintf(os.Stdout, "Response from `AttributesAPI.GetAttributeReferenceConfig`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Attribute ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetAttributeReferenceConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ReferenceConfigResponse**](ReferenceConfigResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetProjectSchema

> ProjectSchemaResponse GetProjectSchema(ctx).Execute()

Get complete project schema



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AttributesAPI.GetProjectSchema(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AttributesAPI.GetProjectSchema``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetProjectSchema`: ProjectSchemaResponse
	fmt.Fprintf(os.Stdout, "Response from `AttributesAPI.GetProjectSchema`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetProjectSchemaRequest struct via the builder pattern


### Return type

[**ProjectSchemaResponse**](ProjectSchemaResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListAttributeItems

> ListAttributeItems200Response ListAttributeItems(ctx, id).Execute()

List items of an attribute

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Attribute ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AttributesAPI.ListAttributeItems(context.Background(), id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AttributesAPI.ListAttributeItems``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAttributeItems`: ListAttributeItems200Response
	fmt.Fprintf(os.Stdout, "Response from `AttributesAPI.ListAttributeItems`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Attribute ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiListAttributeItemsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ListAttributeItems200Response**](ListAttributeItems200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListAttributes

> ListAttributes200Response ListAttributes(ctx).Execute()

List attributes

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AttributesAPI.ListAttributes(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AttributesAPI.ListAttributes``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListAttributes`: ListAttributes200Response
	fmt.Fprintf(os.Stdout, "Response from `AttributesAPI.ListAttributes`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListAttributesRequest struct via the builder pattern


### Return type

[**ListAttributes200Response**](ListAttributes200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SetAttributeItems

> SetAttributeItems(ctx, id).SetListItemsRequest(setListItemsRequest).Execute()

Set list items for an attribute (replaces all existing items)

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Attribute ID
	setListItemsRequest := *openapiclient.NewSetListItemsRequest([]openapiclient.ListItemInput{*openapiclient.NewListItemInput("red")}) // SetListItemsRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AttributesAPI.SetAttributeItems(context.Background(), id).SetListItemsRequest(setListItemsRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AttributesAPI.SetAttributeItems``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Attribute ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetAttributeItemsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **setListItemsRequest** | [**SetListItemsRequest**](SetListItemsRequest.md) |  | 

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


## SetAttributeReferenceConfig

> SetAttributeReferenceConfig(ctx, id).SetReferenceConfigRequest(setReferenceConfigRequest).Execute()

Set or update reference configuration for an attribute

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Attribute ID
	setReferenceConfigRequest := *openapiclient.NewSetReferenceConfigRequest("TargetTemplateId_example", "TargetAttributeId_example") // SetReferenceConfigRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AttributesAPI.SetAttributeReferenceConfig(context.Background(), id).SetReferenceConfigRequest(setReferenceConfigRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AttributesAPI.SetAttributeReferenceConfig``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Attribute ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiSetAttributeReferenceConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **setReferenceConfigRequest** | [**SetReferenceConfigRequest**](SetReferenceConfigRequest.md) |  | 

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


## UpdateAttribute

> UpdateAttribute(ctx, id).UpdateAttributeRequest(updateAttributeRequest).Execute()

Update an attribute

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | 
	updateAttributeRequest := *openapiclient.NewUpdateAttributeRequest("Color") // UpdateAttributeRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AttributesAPI.UpdateAttribute(context.Background(), id).UpdateAttributeRequest(updateAttributeRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AttributesAPI.UpdateAttribute``: %v\n", err)
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

Other parameters are passed through a pointer to a apiUpdateAttributeRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **updateAttributeRequest** | [**UpdateAttributeRequest**](UpdateAttributeRequest.md) |  | 

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


## UpdateAttributeItem

> UpdateAttributeItem(ctx, id, itemId).UpdateListItemRequest(updateListItemRequest).Execute()

Update a list item of an attribute

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
	id := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Attribute ID
	itemId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | List Item ID
	updateListItemRequest := *openapiclient.NewUpdateListItemRequest("blue") // UpdateListItemRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AttributesAPI.UpdateAttributeItem(context.Background(), id, itemId).UpdateListItemRequest(updateListItemRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AttributesAPI.UpdateAttributeItem``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**id** | **string** | Attribute ID | 
**itemId** | **string** | List Item ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateAttributeItemRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateListItemRequest** | [**UpdateListItemRequest**](UpdateListItemRequest.md) |  | 

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

