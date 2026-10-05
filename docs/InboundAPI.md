# \InboundAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddInboundEndpointSecret**](InboundAPI.md#AddInboundEndpointSecret) | **Post** /templates/{templateId}/inbound-endpoints/{id}/secrets | Add a secret to an inbound endpoint (start a rotation)
[**CreateTemplateInboundEndpoint**](InboundAPI.md#CreateTemplateInboundEndpoint) | **Post** /templates/{templateId}/inbound-endpoints | Create an inbound endpoint on a template
[**DeleteInboundEndpointSecret**](InboundAPI.md#DeleteInboundEndpointSecret) | **Delete** /templates/{templateId}/inbound-endpoints/{id}/secrets/{secretId} | Remove a secret from an inbound endpoint (finish a rotation)
[**DeleteTemplateInboundEndpoint**](InboundAPI.md#DeleteTemplateInboundEndpoint) | **Delete** /templates/{templateId}/inbound-endpoints/{id} | Delete an inbound endpoint
[**GetInboundDelivery**](InboundAPI.md#GetInboundDelivery) | **Get** /templates/{templateId}/inbound-endpoints/{id}/deliveries/{deliveryId} | Get one delivery an inbound endpoint received
[**GetTemplateInboundEndpoint**](InboundAPI.md#GetTemplateInboundEndpoint) | **Get** /templates/{templateId}/inbound-endpoints/{id} | Get an inbound endpoint
[**ListInboundDeliveries**](InboundAPI.md#ListInboundDeliveries) | **Get** /templates/{templateId}/inbound-endpoints/{id}/deliveries | List the deliveries an inbound endpoint received
[**ListTemplateInboundEndpoints**](InboundAPI.md#ListTemplateInboundEndpoints) | **Get** /templates/{templateId}/inbound-endpoints | List the inbound endpoints of a template
[**PreviewInboundMapping**](InboundAPI.md#PreviewInboundMapping) | **Post** /templates/{templateId}/inbound-endpoints/{id}/preview | Preview what an inbound mapping does with a sample payload
[**ReceiveInboundDelivery**](InboundAPI.md#ReceiveInboundDelivery) | **Post** /inbound/{projectId}/{endpointId} | Receive a delivery from an outside system
[**ReplayInboundDelivery**](InboundAPI.md#ReplayInboundDelivery) | **Post** /templates/{templateId}/inbound-endpoints/{id}/deliveries/{deliveryId}/replay | Replay a stored inbound delivery through the current mapping
[**UpdateTemplateInboundEndpoint**](InboundAPI.md#UpdateTemplateInboundEndpoint) | **Patch** /templates/{templateId}/inbound-endpoints/{id} | Update an inbound endpoint



## AddInboundEndpointSecret

> InboundSecretRevealed AddInboundEndpointSecret(ctx, templateId, id).XOmnismithProjectId(xOmnismithProjectId).AddInboundEndpointSecretRequest(addInboundEndpointSecretRequest).Execute()

Add a secret to an inbound endpoint (start a rotation)



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
	templateId := "customer" // string | UUID or slug of the template
	id := "01a0f0e2-7c1a-7000-8000-000000000001" // string | Inbound endpoint UUID
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)
	addInboundEndpointSecretRequest := *openapiclient.NewAddInboundEndpointSecretRequest() // AddInboundEndpointSecretRequest |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InboundAPI.AddInboundEndpointSecret(context.Background(), templateId, id).XOmnismithProjectId(xOmnismithProjectId).AddInboundEndpointSecretRequest(addInboundEndpointSecretRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboundAPI.AddInboundEndpointSecret``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AddInboundEndpointSecret`: InboundSecretRevealed
	fmt.Fprintf(os.Stdout, "Response from `InboundAPI.AddInboundEndpointSecret`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 
**id** | **string** | Inbound endpoint UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiAddInboundEndpointSecretRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 
 **addInboundEndpointSecretRequest** | [**AddInboundEndpointSecretRequest**](AddInboundEndpointSecretRequest.md) |  | 

### Return type

[**InboundSecretRevealed**](InboundSecretRevealed.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateTemplateInboundEndpoint

> InboundEndpointCreatedResponse CreateTemplateInboundEndpoint(ctx, templateId).CreateInboundEndpointRequest(createInboundEndpointRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Create an inbound endpoint on a template



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
	templateId := "customer" // string | UUID or slug of the template
	createInboundEndpointRequest := *openapiclient.NewCreateInboundEndpointRequest("Stripe customers", map[string]interface{}{"key": interface{}(123)}, map[string]interface{}{"key": interface{}(123)}) // CreateInboundEndpointRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InboundAPI.CreateTemplateInboundEndpoint(context.Background(), templateId).CreateInboundEndpointRequest(createInboundEndpointRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboundAPI.CreateTemplateInboundEndpoint``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTemplateInboundEndpoint`: InboundEndpointCreatedResponse
	fmt.Fprintf(os.Stdout, "Response from `InboundAPI.CreateTemplateInboundEndpoint`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateTemplateInboundEndpointRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createInboundEndpointRequest** | [**CreateInboundEndpointRequest**](CreateInboundEndpointRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**InboundEndpointCreatedResponse**](InboundEndpointCreatedResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteInboundEndpointSecret

> DeleteInboundEndpointSecret(ctx, templateId, id, secretId).XOmnismithProjectId(xOmnismithProjectId).Execute()

Remove a secret from an inbound endpoint (finish a rotation)



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
	templateId := "customer" // string | UUID or slug of the template
	id := "01a0f0e2-7c1a-7000-8000-000000000001" // string | Inbound endpoint UUID
	secretId := "01a0f0e2-7c1a-7000-8000-0000000000c1" // string | Secret UUID, from the endpoint's `secrets`
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.InboundAPI.DeleteInboundEndpointSecret(context.Background(), templateId, id, secretId).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboundAPI.DeleteInboundEndpointSecret``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 
**id** | **string** | Inbound endpoint UUID | 
**secretId** | **string** | Secret UUID, from the endpoint&#39;s &#x60;secrets&#x60; | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteInboundEndpointSecretRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

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


## DeleteTemplateInboundEndpoint

> DeleteTemplateInboundEndpoint(ctx, templateId, id).XOmnismithProjectId(xOmnismithProjectId).Execute()

Delete an inbound endpoint



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
	templateId := "customer" // string | UUID or slug of the template
	id := "01a0f0e2-7c1a-7000-8000-000000000001" // string | Inbound endpoint UUID
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.InboundAPI.DeleteTemplateInboundEndpoint(context.Background(), templateId, id).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboundAPI.DeleteTemplateInboundEndpoint``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 
**id** | **string** | Inbound endpoint UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteTemplateInboundEndpointRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

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


## GetInboundDelivery

> InboundDeliveryDetail GetInboundDelivery(ctx, templateId, id, deliveryId).XOmnismithProjectId(xOmnismithProjectId).Execute()

Get one delivery an inbound endpoint received



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
	templateId := "customer" // string | UUID or slug of the template
	id := "01a0f0e2-7c1a-7000-8000-000000000001" // string | Inbound endpoint UUID
	deliveryId := "01a0f0e2-7c1a-7000-8000-0000000000d1" // string | Delivery log row UUID
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InboundAPI.GetInboundDelivery(context.Background(), templateId, id, deliveryId).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboundAPI.GetInboundDelivery``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetInboundDelivery`: InboundDeliveryDetail
	fmt.Fprintf(os.Stdout, "Response from `InboundAPI.GetInboundDelivery`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 
**id** | **string** | Inbound endpoint UUID | 
**deliveryId** | **string** | Delivery log row UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetInboundDeliveryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**InboundDeliveryDetail**](InboundDeliveryDetail.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetTemplateInboundEndpoint

> InboundEndpointResponse GetTemplateInboundEndpoint(ctx, templateId, id).XOmnismithProjectId(xOmnismithProjectId).Execute()

Get an inbound endpoint



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
	templateId := "customer" // string | UUID or slug of the template
	id := "01a0f0e2-7c1a-7000-8000-000000000001" // string | Inbound endpoint UUID
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InboundAPI.GetTemplateInboundEndpoint(context.Background(), templateId, id).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboundAPI.GetTemplateInboundEndpoint``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTemplateInboundEndpoint`: InboundEndpointResponse
	fmt.Fprintf(os.Stdout, "Response from `InboundAPI.GetTemplateInboundEndpoint`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 
**id** | **string** | Inbound endpoint UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTemplateInboundEndpointRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**InboundEndpointResponse**](InboundEndpointResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListInboundDeliveries

> ListInboundDeliveries200Response ListInboundDeliveries(ctx, templateId, id).XOmnismithProjectId(xOmnismithProjectId).Outcome(outcome).From(from).To(to).Limit(limit).Offset(offset).Execute()

List the deliveries an inbound endpoint received



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
	templateId := "customer" // string | UUID or slug of the template
	id := "01a0f0e2-7c1a-7000-8000-000000000001" // string | Inbound endpoint UUID
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)
	outcome := []string{"Outcome_example"} // []string | Only deliveries with one of these outcomes; comma-separated (optional)
	from := time.Now() // time.Time | Only deliveries received at or after this RFC 3339 time (optional)
	to := time.Now() // time.Time | Only deliveries received at or before this RFC 3339 time (optional)
	limit := int32(56) // int32 | Page size (optional) (default to 20)
	offset := int32(56) // int32 | Number of deliveries to skip (optional) (default to 0)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InboundAPI.ListInboundDeliveries(context.Background(), templateId, id).XOmnismithProjectId(xOmnismithProjectId).Outcome(outcome).From(from).To(to).Limit(limit).Offset(offset).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboundAPI.ListInboundDeliveries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListInboundDeliveries`: ListInboundDeliveries200Response
	fmt.Fprintf(os.Stdout, "Response from `InboundAPI.ListInboundDeliveries`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 
**id** | **string** | Inbound endpoint UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiListInboundDeliveriesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 
 **outcome** | **[]string** | Only deliveries with one of these outcomes; comma-separated | 
 **from** | **time.Time** | Only deliveries received at or after this RFC 3339 time | 
 **to** | **time.Time** | Only deliveries received at or before this RFC 3339 time | 
 **limit** | **int32** | Page size | [default to 20]
 **offset** | **int32** | Number of deliveries to skip | [default to 0]

### Return type

[**ListInboundDeliveries200Response**](ListInboundDeliveries200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTemplateInboundEndpoints

> ListTemplateInboundEndpoints200Response ListTemplateInboundEndpoints(ctx, templateId).XOmnismithProjectId(xOmnismithProjectId).Execute()

List the inbound endpoints of a template



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
	templateId := "customer" // string | UUID or slug of the template
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InboundAPI.ListTemplateInboundEndpoints(context.Background(), templateId).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboundAPI.ListTemplateInboundEndpoints``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTemplateInboundEndpoints`: ListTemplateInboundEndpoints200Response
	fmt.Fprintf(os.Stdout, "Response from `InboundAPI.ListTemplateInboundEndpoints`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 

### Other Parameters

Other parameters are passed through a pointer to a apiListTemplateInboundEndpointsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**ListTemplateInboundEndpoints200Response**](ListTemplateInboundEndpoints200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PreviewInboundMapping

> PreviewInboundMapping200Response PreviewInboundMapping(ctx, templateId, id).PreviewInboundMappingRequest(previewInboundMappingRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Preview what an inbound mapping does with a sample payload



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
	templateId := "customer" // string | UUID or slug of the template
	id := "01a0f0e2-7c1a-7000-8000-000000000001" // string | Inbound endpoint UUID
	previewInboundMappingRequest := *openapiclient.NewPreviewInboundMappingRequest() // PreviewInboundMappingRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InboundAPI.PreviewInboundMapping(context.Background(), templateId, id).PreviewInboundMappingRequest(previewInboundMappingRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboundAPI.PreviewInboundMapping``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PreviewInboundMapping`: PreviewInboundMapping200Response
	fmt.Fprintf(os.Stdout, "Response from `InboundAPI.PreviewInboundMapping`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 
**id** | **string** | Inbound endpoint UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiPreviewInboundMappingRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **previewInboundMappingRequest** | [**PreviewInboundMappingRequest**](PreviewInboundMappingRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**PreviewInboundMapping200Response**](PreviewInboundMapping200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ReceiveInboundDelivery

> ReceiveInboundDelivery200Response ReceiveInboundDelivery(ctx, projectId, endpointId).RequestBody(requestBody).Execute()

Receive a delivery from an outside system



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
	projectId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Project UUID
	endpointId := "38400000-8cf0-11bd-b23e-10b96e4ef00d" // string | Inbound endpoint UUID
	requestBody := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} | The sender's JSON payload, unchanged. At most 1 MB.

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InboundAPI.ReceiveInboundDelivery(context.Background(), projectId, endpointId).RequestBody(requestBody).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboundAPI.ReceiveInboundDelivery``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ReceiveInboundDelivery`: ReceiveInboundDelivery200Response
	fmt.Fprintf(os.Stdout, "Response from `InboundAPI.ReceiveInboundDelivery`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**projectId** | **string** | Project UUID | 
**endpointId** | **string** | Inbound endpoint UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiReceiveInboundDeliveryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **requestBody** | **map[string]interface{}** | The sender&#39;s JSON payload, unchanged. At most 1 MB. | 

### Return type

[**ReceiveInboundDelivery200Response**](ReceiveInboundDelivery200Response.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ReplayInboundDelivery

> InboundDeliverySummary ReplayInboundDelivery(ctx, templateId, id, deliveryId).XOmnismithProjectId(xOmnismithProjectId).Execute()

Replay a stored inbound delivery through the current mapping



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
	templateId := "customer" // string | UUID or slug of the template
	id := "01a0f0e2-7c1a-7000-8000-000000000001" // string | Inbound endpoint UUID
	deliveryId := "01a0f0e2-7c1a-7000-8000-0000000000d1" // string | The delivery log row to replay
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InboundAPI.ReplayInboundDelivery(context.Background(), templateId, id, deliveryId).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboundAPI.ReplayInboundDelivery``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ReplayInboundDelivery`: InboundDeliverySummary
	fmt.Fprintf(os.Stdout, "Response from `InboundAPI.ReplayInboundDelivery`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 
**id** | **string** | Inbound endpoint UUID | 
**deliveryId** | **string** | The delivery log row to replay | 

### Other Parameters

Other parameters are passed through a pointer to a apiReplayInboundDeliveryRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**InboundDeliverySummary**](InboundDeliverySummary.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateTemplateInboundEndpoint

> InboundEndpointResponse UpdateTemplateInboundEndpoint(ctx, templateId, id).UpdateInboundEndpointRequest(updateInboundEndpointRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Update an inbound endpoint



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
	templateId := "customer" // string | UUID or slug of the template
	id := "01a0f0e2-7c1a-7000-8000-000000000001" // string | Inbound endpoint UUID
	updateInboundEndpointRequest := *openapiclient.NewUpdateInboundEndpointRequest() // UpdateInboundEndpointRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.InboundAPI.UpdateTemplateInboundEndpoint(context.Background(), templateId, id).UpdateInboundEndpointRequest(updateInboundEndpointRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `InboundAPI.UpdateTemplateInboundEndpoint``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateTemplateInboundEndpoint`: InboundEndpointResponse
	fmt.Fprintf(os.Stdout, "Response from `InboundAPI.UpdateTemplateInboundEndpoint`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 
**id** | **string** | Inbound endpoint UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateTemplateInboundEndpointRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateInboundEndpointRequest** | [**UpdateInboundEndpointRequest**](UpdateInboundEndpointRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**InboundEndpointResponse**](InboundEndpointResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

