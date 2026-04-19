# \FeedbackAPI

All URIs are relative to *https://api.omnismith.io/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**SendFeedback**](FeedbackAPI.md#SendFeedback) | **Post** /feedback | Submit user feedback



## SendFeedback

> SendFeedback(ctx).SendFeedbackRequest(sendFeedbackRequest).Execute()

Submit user feedback



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
	sendFeedbackRequest := *openapiclient.NewSendFeedbackRequest("Dashboard chart is not rendering correctly", "Bug Report", "When I open the dashboard page, the chart widget shows a blank area instead of data.") // SendFeedbackRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.FeedbackAPI.SendFeedback(context.Background()).SendFeedbackRequest(sendFeedbackRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `FeedbackAPI.SendFeedback``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSendFeedbackRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sendFeedbackRequest** | [**SendFeedbackRequest**](SendFeedbackRequest.md) |  | 

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

