# \EventsAPI

All URIs are relative to *http://localhost:4444*

Method | HTTP request | Description
------------- | ------------- | -------------
[**EventsPost**](EventsAPI.md#EventsPost) | **Post** /events | Create a new event



## EventsPost

> map[string]string EventsPost(ctx).Event(event).Execute()

Create a new event



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/xcaliber-health/go-observability-sdk"
)

func main() {
	event := *openapiclient.NewMainCreateEventRequest() // MainCreateEventRequest | Event to be created

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EventsAPI.EventsPost(context.Background()).Event(event).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EventsAPI.EventsPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EventsPost`: map[string]string
	fmt.Fprintf(os.Stdout, "Response from `EventsAPI.EventsPost`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiEventsPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **event** | [**MainCreateEventRequest**](MainCreateEventRequest.md) | Event to be created | 

### Return type

**map[string]string**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

