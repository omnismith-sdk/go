# \SchemaAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**GetProjectSchema**](SchemaAPI.md#GetProjectSchema) | **Get** /discovery/project-schema | Get complete project schema graph



## GetProjectSchema

> ProjectSchemaResponse GetProjectSchema(ctx).Execute()

Get complete project schema graph



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
	resp, r, err := apiClient.SchemaAPI.GetProjectSchema(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `SchemaAPI.GetProjectSchema``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetProjectSchema`: ProjectSchemaResponse
	fmt.Fprintf(os.Stdout, "Response from `SchemaAPI.GetProjectSchema`: %v\n", resp)
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

