# \AutomationPushDevicesAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListPushDevices**](AutomationPushDevicesAPI.md#ListPushDevices) | **Get** /automation/push-devices | List the current user&#39;s registered push devices
[**RegisterPushDevice**](AutomationPushDevicesAPI.md#RegisterPushDevice) | **Post** /automation/push-devices | Register a push notification device token
[**UnregisterPushDevice**](AutomationPushDevicesAPI.md#UnregisterPushDevice) | **Delete** /automation/push-devices | Unregister a push notification device token



## ListPushDevices

> ListPushDevices200Response ListPushDevices(ctx).Execute()

List the current user's registered push devices

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
	resp, r, err := apiClient.AutomationPushDevicesAPI.ListPushDevices(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutomationPushDevicesAPI.ListPushDevices``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListPushDevices`: ListPushDevices200Response
	fmt.Fprintf(os.Stdout, "Response from `AutomationPushDevicesAPI.ListPushDevices`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListPushDevicesRequest struct via the builder pattern


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

> CreateAttributeItem201Response RegisterPushDevice(ctx).RegisterPushDeviceRequest(registerPushDeviceRequest).Execute()

Register a push notification device token

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
	registerPushDeviceRequest := *openapiclient.NewRegisterPushDeviceRequest("Token_example") // RegisterPushDeviceRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutomationPushDevicesAPI.RegisterPushDevice(context.Background()).RegisterPushDeviceRequest(registerPushDeviceRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AutomationPushDevicesAPI.RegisterPushDevice``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `RegisterPushDevice`: CreateAttributeItem201Response
	fmt.Fprintf(os.Stdout, "Response from `AutomationPushDevicesAPI.RegisterPushDevice`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiRegisterPushDeviceRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registerPushDeviceRequest** | [**RegisterPushDeviceRequest**](RegisterPushDeviceRequest.md) |  | 

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


## UnregisterPushDevice

> UnregisterPushDevice(ctx).UnregisterPushDeviceRequest(unregisterPushDeviceRequest).Execute()

Unregister a push notification device token

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
	unregisterPushDeviceRequest := *openapiclient.NewUnregisterPushDeviceRequest("Token_example") // UnregisterPushDeviceRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.AutomationPushDevicesAPI.UnregisterPushDevice(context.Background()).UnregisterPushDeviceRequest(unregisterPushDeviceRequest).Execute()
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

