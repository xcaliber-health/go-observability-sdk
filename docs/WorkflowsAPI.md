# \WorkflowsAPI

All URIs are relative to *http://localhost:4444*

Method | HTTP request | Description
------------- | ------------- | -------------
[**WorkflowsEventsGet**](WorkflowsAPI.md#WorkflowsEventsGet) | **Get** /workflows/events | Get all workflow events within a duration



## WorkflowsEventsGet

> map[string]interface{} WorkflowsEventsGet(ctx).StartTime(startTime).EndTime(endTime).Execute()

Get all workflow events within a duration



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
	startTime := "startTime_example" // string | Start Time
	endTime := "endTime_example" // string | End Time

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.WorkflowsAPI.WorkflowsEventsGet(context.Background()).StartTime(startTime).EndTime(endTime).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `WorkflowsAPI.WorkflowsEventsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `WorkflowsEventsGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `WorkflowsAPI.WorkflowsEventsGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiWorkflowsEventsGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **startTime** | **string** | Start Time | 
 **endTime** | **string** | End Time | 

### Return type

**map[string]interface{}**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: */*

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

