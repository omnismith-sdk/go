# \AutomationPushDevicesAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListPushDevices**](AutomationPushDevicesAPI.md#ListPushDevices) | **Get** /automation/push-devices | List registered push devices
[**RegisterPushDevice**](AutomationPushDevicesAPI.md#RegisterPushDevice) | **Post** /automation/push-devices | Register a mobile push notification device
[**UnregisterPushDevice**](AutomationPushDevicesAPI.md#UnregisterPushDevice) | **Delete** /automation/push-devices | Unregister a mobile push notification device



## ListPushDevices

> ListPushDevices200Response ListPushDevices(ctx).XOmnismithProjectId(xOmnismithProjectId).Execute()

List registered push devices



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
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutomationPushDevicesAPI.ListPushDevices(context.Background()).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutomationPushDevicesAPI.ListPushDevices``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPushDevices`: ListPushDevices200Response
	fmt.Fprintf(os.Stdout, "Response from `AutomationPushDevicesAPI.ListPushDevices`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiListPushDevicesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**ListPushDevices200Response**](ListPushDevices200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## RegisterPushDevice

> RegisterPushDevice201Response RegisterPushDevice(ctx).RegisterPushDeviceRequest(registerPushDeviceRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Register a mobile push notification device



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
	registerPushDeviceRequest := *openapiclient.NewRegisterPushDeviceRequest("dK1_f92La...xR8_token") // RegisterPushDeviceRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutomationPushDevicesAPI.RegisterPushDevice(context.Background()).RegisterPushDeviceRequest(registerPushDeviceRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutomationPushDevicesAPI.RegisterPushDevice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RegisterPushDevice`: RegisterPushDevice201Response
	fmt.Fprintf(os.Stdout, "Response from `AutomationPushDevicesAPI.RegisterPushDevice`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRegisterPushDeviceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registerPushDeviceRequest** | [**RegisterPushDeviceRequest**](RegisterPushDeviceRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**RegisterPushDevice201Response**](RegisterPushDevice201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UnregisterPushDevice

> UnregisterPushDevice(ctx).UnregisterPushDeviceRequest(unregisterPushDeviceRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Unregister a mobile push notification device



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
	unregisterPushDeviceRequest := *openapiclient.NewUnregisterPushDeviceRequest("dK1_f92La...xR8_token") // UnregisterPushDeviceRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AutomationPushDevicesAPI.UnregisterPushDevice(context.Background()).UnregisterPushDeviceRequest(unregisterPushDeviceRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutomationPushDevicesAPI.UnregisterPushDevice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiUnregisterPushDeviceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **unregisterPushDeviceRequest** | [**UnregisterPushDeviceRequest**](UnregisterPushDeviceRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

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

