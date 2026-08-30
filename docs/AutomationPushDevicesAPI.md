# \AutomationPushDevicesAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListPushDevices**](AutomationPushDevicesAPI.md#ListPushDevices) | **Get** /automation/push-devices | List registered push devices
[**RegisterPushDevice**](AutomationPushDevicesAPI.md#RegisterPushDevice) | **Post** /automation/push-devices | Register a mobile push notification device
[**UnregisterPushDevice**](AutomationPushDevicesAPI.md#UnregisterPushDevice) | **Delete** /automation/push-devices | Unregister a mobile push notification device



## ListPushDevices

> ListPushDevices200Response ListPushDevices(ctx).Execute()

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

> RegisterPushDevice201Response RegisterPushDevice(ctx).RegisterPushDeviceRequest(registerPushDeviceRequest).Execute()

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AutomationPushDevicesAPI.RegisterPushDevice(context.Background()).RegisterPushDeviceRequest(registerPushDeviceRequest).Execute()
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

> UnregisterPushDevice(ctx).UnregisterPushDeviceRequest(unregisterPushDeviceRequest).Execute()

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

