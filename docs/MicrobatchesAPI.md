# \MicrobatchesAPI

All URIs are relative to *http://localhost:4444*

Method | HTTP request | Description
------------- | ------------- | -------------
[**MicrobatchesEventsGet**](MicrobatchesAPI.md#MicrobatchesEventsGet) | **Get** /microbatches/events | Get all microbatch events within a duration
[**MicrobatchesMicrobatchIdDurationGet**](MicrobatchesAPI.md#MicrobatchesMicrobatchIdDurationGet) | **Get** /microbatches/{microbatch_id}/duration | Get the total duration of a specific microbatch
[**MicrobatchesMicrobatchIdStatusGet**](MicrobatchesAPI.md#MicrobatchesMicrobatchIdStatusGet) | **Get** /microbatches/{microbatch_id}/status | Get the current status of a specific microbatch



## MicrobatchesEventsGet

> map[string]interface{} MicrobatchesEventsGet(ctx).StartTime(startTime).EndTime(endTime).Execute()

Get all microbatch events within a duration



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
	resp, r, err := apiClient.MicrobatchesAPI.MicrobatchesEventsGet(context.Background()).StartTime(startTime).EndTime(endTime).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MicrobatchesAPI.MicrobatchesEventsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MicrobatchesEventsGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MicrobatchesAPI.MicrobatchesEventsGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiMicrobatchesEventsGetRequest struct via the builder pattern


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


## MicrobatchesMicrobatchIdDurationGet

> map[string]interface{} MicrobatchesMicrobatchIdDurationGet(ctx, microbatchId).Execute()

Get the total duration of a specific microbatch



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
	microbatchId := "microbatchId_example" // string | Microbatch ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MicrobatchesAPI.MicrobatchesMicrobatchIdDurationGet(context.Background(), microbatchId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MicrobatchesAPI.MicrobatchesMicrobatchIdDurationGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MicrobatchesMicrobatchIdDurationGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MicrobatchesAPI.MicrobatchesMicrobatchIdDurationGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**microbatchId** | **string** | Microbatch ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiMicrobatchesMicrobatchIdDurationGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


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


## MicrobatchesMicrobatchIdStatusGet

> map[string]interface{} MicrobatchesMicrobatchIdStatusGet(ctx, microbatchId).Execute()

Get the current status of a specific microbatch



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
	microbatchId := "microbatchId_example" // string | Microbatch ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.MicrobatchesAPI.MicrobatchesMicrobatchIdStatusGet(context.Background(), microbatchId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `MicrobatchesAPI.MicrobatchesMicrobatchIdStatusGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `MicrobatchesMicrobatchIdStatusGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `MicrobatchesAPI.MicrobatchesMicrobatchIdStatusGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**microbatchId** | **string** | Microbatch ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiMicrobatchesMicrobatchIdStatusGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


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

