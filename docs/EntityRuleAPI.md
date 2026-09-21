# \EntityRuleAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateTemplateRule**](EntityRuleAPI.md#CreateTemplateRule) | **Post** /templates/{templateId}/rules | Create a business rule on a template
[**DeleteTemplateRule**](EntityRuleAPI.md#DeleteTemplateRule) | **Delete** /templates/{templateId}/rules/{id} | Delete a business rule
[**GetTemplateRule**](EntityRuleAPI.md#GetTemplateRule) | **Get** /templates/{templateId}/rules/{id} | Get a business rule
[**ListTemplateRules**](EntityRuleAPI.md#ListTemplateRules) | **Get** /templates/{templateId}/rules | List the business rules of a template
[**ToggleTemplateRule**](EntityRuleAPI.md#ToggleTemplateRule) | **Post** /templates/{templateId}/rules/{id}/toggle | Enable or disable a business rule
[**UpdateTemplateRule**](EntityRuleAPI.md#UpdateTemplateRule) | **Put** /templates/{templateId}/rules/{id} | Replace a business rule



## CreateTemplateRule

> CreateTemplateRule201Response CreateTemplateRule(ctx, templateId).CreateEntityRuleRequest(createEntityRuleRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Create a business rule on a template



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
	templateId := "018b2f1b-8c1a-75b3-8000-7f0000010010" // string | UUID or slug of the template
	createEntityRuleRequest := *openapiclient.NewCreateEntityRuleRequest("Dietary options when dietary", "Dietary options are required when dietary is yes", []openapiclient.EntityRulePredicate{*openapiclient.NewEntityRulePredicate("018b2f1b-8c1a-75b3-8000-7f0000010000", "eq")}) // CreateEntityRuleRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityRuleAPI.CreateTemplateRule(context.Background(), templateId).CreateEntityRuleRequest(createEntityRuleRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityRuleAPI.CreateTemplateRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateTemplateRule`: CreateTemplateRule201Response
	fmt.Fprintf(os.Stdout, "Response from `EntityRuleAPI.CreateTemplateRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateTemplateRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createEntityRuleRequest** | [**CreateEntityRuleRequest**](CreateEntityRuleRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**CreateTemplateRule201Response**](CreateTemplateRule201Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## DeleteTemplateRule

> DeleteTemplateRule(ctx, templateId, id).XOmnismithProjectId(xOmnismithProjectId).Execute()

Delete a business rule



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
	templateId := "018b2f1b-8c1a-75b3-8000-7f0000010010" // string | UUID or slug of the template
	id := "01a09800-0000-7000-8000-000000000001" // string | Rule UUID
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.EntityRuleAPI.DeleteTemplateRule(context.Background(), templateId, id).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityRuleAPI.DeleteTemplateRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 
**id** | **string** | Rule UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteTemplateRuleRequest struct via the builder pattern


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


## GetTemplateRule

> EntityRuleResponse GetTemplateRule(ctx, templateId, id).XOmnismithProjectId(xOmnismithProjectId).Execute()

Get a business rule



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
	templateId := "018b2f1b-8c1a-75b3-8000-7f0000010010" // string | UUID or slug of the template
	id := "01a09800-0000-7000-8000-000000000001" // string | Rule UUID
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityRuleAPI.GetTemplateRule(context.Background(), templateId, id).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityRuleAPI.GetTemplateRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetTemplateRule`: EntityRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `EntityRuleAPI.GetTemplateRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 
**id** | **string** | Rule UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiGetTemplateRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**EntityRuleResponse**](EntityRuleResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListTemplateRules

> ListTemplateRules200Response ListTemplateRules(ctx, templateId).XOmnismithProjectId(xOmnismithProjectId).IsEnabled(isEnabled).Execute()

List the business rules of a template



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
	templateId := "018b2f1b-8c1a-75b3-8000-7f0000010010" // string | UUID or slug of the template
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)
	isEnabled := true // bool | Only enabled (`true`) or only disabled (`false`) rules (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityRuleAPI.ListTemplateRules(context.Background(), templateId).XOmnismithProjectId(xOmnismithProjectId).IsEnabled(isEnabled).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityRuleAPI.ListTemplateRules``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListTemplateRules`: ListTemplateRules200Response
	fmt.Fprintf(os.Stdout, "Response from `EntityRuleAPI.ListTemplateRules`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 

### Other Parameters

Other parameters are passed through a pointer to a apiListTemplateRulesRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 
 **isEnabled** | **bool** | Only enabled (&#x60;true&#x60;) or only disabled (&#x60;false&#x60;) rules | 

### Return type

[**ListTemplateRules200Response**](ListTemplateRules200Response.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ToggleTemplateRule

> EntityRuleResponse ToggleTemplateRule(ctx, templateId, id).ToggleEntityRuleRequest(toggleEntityRuleRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Enable or disable a business rule



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
	templateId := "018b2f1b-8c1a-75b3-8000-7f0000010010" // string | UUID or slug of the template
	id := "01a09800-0000-7000-8000-000000000001" // string | Rule UUID
	toggleEntityRuleRequest := *openapiclient.NewToggleEntityRuleRequest(false) // ToggleEntityRuleRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityRuleAPI.ToggleTemplateRule(context.Background(), templateId, id).ToggleEntityRuleRequest(toggleEntityRuleRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityRuleAPI.ToggleTemplateRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ToggleTemplateRule`: EntityRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `EntityRuleAPI.ToggleTemplateRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 
**id** | **string** | Rule UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiToggleTemplateRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **toggleEntityRuleRequest** | [**ToggleEntityRuleRequest**](ToggleEntityRuleRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**EntityRuleResponse**](EntityRuleResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateTemplateRule

> EntityRuleResponse UpdateTemplateRule(ctx, templateId, id).UpdateEntityRuleRequest(updateEntityRuleRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()

Replace a business rule



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
	templateId := "018b2f1b-8c1a-75b3-8000-7f0000010010" // string | UUID or slug of the template
	id := "01a09800-0000-7000-8000-000000000001" // string | Rule UUID
	updateEntityRuleRequest := *openapiclient.NewUpdateEntityRuleRequest("Dietary options when dietary", "Dietary options are required when dietary is yes", []openapiclient.EntityRulePredicate{*openapiclient.NewEntityRulePredicate("018b2f1b-8c1a-75b3-8000-7f0000010000", "eq")}) // UpdateEntityRuleRequest | 
	xOmnismithProjectId := "018b2f1b-7c3a-7d2e-8f1a-2b3c4d5e6f7d" // string | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential's `projects` claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code `stale_project_grant`; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 `no_project_selected`. Two clients holding the same credential may send different values at the same time. (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EntityRuleAPI.UpdateTemplateRule(context.Background(), templateId, id).UpdateEntityRuleRequest(updateEntityRuleRequest).XOmnismithProjectId(xOmnismithProjectId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EntityRuleAPI.UpdateTemplateRule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateTemplateRule`: EntityRuleResponse
	fmt.Fprintf(os.Stdout, "Response from `EntityRuleAPI.UpdateTemplateRule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**templateId** | **string** | UUID or slug of the template | 
**id** | **string** | Rule UUID | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateTemplateRuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **updateEntityRuleRequest** | [**UpdateEntityRuleRequest**](UpdateEntityRuleRequest.md) |  | 
 **xOmnismithProjectId** | **string** | The project this call acts on. A credential proves identity and grants a set of projects; it never selects one, so every tenant-scoped call names its target here. The value must be one of the projects in the credential&#39;s &#x60;projects&#x60; claim and must still be reachable — a project the caller is not a member of, or one that has been deleted, is rejected with 403 rather than silently ignored. A project the caller *is* a member of but which the credential predates is also rejected with 403, carrying the code &#x60;stale_project_grant&#x60;; that one is answered by refreshing the credential once and retrying, and is the only 403 here worth retrying. Omitting the header is not an error: the caller is simply acting with no project selected, and a tenant-scoped operation then answers 409 &#x60;no_project_selected&#x60;. Two clients holding the same credential may send different values at the same time. | 

### Return type

[**EntityRuleResponse**](EntityRuleResponse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

