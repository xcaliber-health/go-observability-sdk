# \PipelinesAPI

All URIs are relative to *http://localhost:4444*

Method | HTTP request | Description
------------- | ------------- | -------------
[**PipelinesFailedGet**](PipelinesAPI.md#PipelinesFailedGet) | **Get** /pipelines/failed | Get the number of pipelines that have failed
[**PipelinesPipelineIdDurationGet**](PipelinesAPI.md#PipelinesPipelineIdDurationGet) | **Get** /pipelines/{pipeline_id}/duration | Get the total duration of a specific pipeline
[**PipelinesPipelineIdEventsGet**](PipelinesAPI.md#PipelinesPipelineIdEventsGet) | **Get** /pipelines/{pipeline_id}/events | Get all events of a specific pipeline within a duration
[**PipelinesPipelineIdStatusGet**](PipelinesAPI.md#PipelinesPipelineIdStatusGet) | **Get** /pipelines/{pipeline_id}/status | Get the current status of a specific pipeline
[**PipelinesPost**](PipelinesAPI.md#PipelinesPost) | **Post** /pipelines | Register a new pipeline
[**PipelinesSucceededGet**](PipelinesAPI.md#PipelinesSucceededGet) | **Get** /pipelines/succeeded | Get the number of pipelines that have succeeded
[**PipelinesTotalGet**](PipelinesAPI.md#PipelinesTotalGet) | **Get** /pipelines/total | Get the total number of pipelines
[**PipelinesTypeAverageDurationGet**](PipelinesAPI.md#PipelinesTypeAverageDurationGet) | **Get** /pipelines/{type}/average_duration | Get the average duration of a specific type of pipeline
[**PipelinesTypeMaxDurationGet**](PipelinesAPI.md#PipelinesTypeMaxDurationGet) | **Get** /pipelines/{type}/max_duration | Get the maximum duration of a specific type of pipeline



## PipelinesFailedGet

> map[string]int32 PipelinesFailedGet(ctx).StartTime(startTime).EndTime(endTime).Execute()

Get the number of pipelines that have failed



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
	startTime := "startTime_example" // string | Start Time (optional)
	endTime := "endTime_example" // string | End Time (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PipelinesAPI.PipelinesFailedGet(context.Background()).StartTime(startTime).EndTime(endTime).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PipelinesAPI.PipelinesFailedGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PipelinesFailedGet`: map[string]int32
	fmt.Fprintf(os.Stdout, "Response from `PipelinesAPI.PipelinesFailedGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPipelinesFailedGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **startTime** | **string** | Start Time | 
 **endTime** | **string** | End Time | 

### Return type

**map[string]int32**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: */*

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PipelinesPipelineIdDurationGet

> map[string]interface{} PipelinesPipelineIdDurationGet(ctx, pipelineId).Execute()

Get the total duration of a specific pipeline



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
	pipelineId := "pipelineId_example" // string | Pipeline ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PipelinesAPI.PipelinesPipelineIdDurationGet(context.Background(), pipelineId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PipelinesAPI.PipelinesPipelineIdDurationGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PipelinesPipelineIdDurationGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PipelinesAPI.PipelinesPipelineIdDurationGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**pipelineId** | **string** | Pipeline ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiPipelinesPipelineIdDurationGetRequest struct via the builder pattern


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


## PipelinesPipelineIdEventsGet

> map[string]interface{} PipelinesPipelineIdEventsGet(ctx, pipelineId).StartTime(startTime).EndTime(endTime).Execute()

Get all events of a specific pipeline within a duration



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
	pipelineId := "pipelineId_example" // string | Pipeline ID
	startTime := "startTime_example" // string | Start Time
	endTime := "endTime_example" // string | End Time

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PipelinesAPI.PipelinesPipelineIdEventsGet(context.Background(), pipelineId).StartTime(startTime).EndTime(endTime).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PipelinesAPI.PipelinesPipelineIdEventsGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PipelinesPipelineIdEventsGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PipelinesAPI.PipelinesPipelineIdEventsGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**pipelineId** | **string** | Pipeline ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiPipelinesPipelineIdEventsGetRequest struct via the builder pattern


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


## PipelinesPipelineIdStatusGet

> map[string]interface{} PipelinesPipelineIdStatusGet(ctx, pipelineId).Execute()

Get the current status of a specific pipeline



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
	pipelineId := "pipelineId_example" // string | Pipeline ID

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PipelinesAPI.PipelinesPipelineIdStatusGet(context.Background(), pipelineId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PipelinesAPI.PipelinesPipelineIdStatusGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PipelinesPipelineIdStatusGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PipelinesAPI.PipelinesPipelineIdStatusGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**pipelineId** | **string** | Pipeline ID | 

### Other Parameters

Other parameters are passed through a pointer to a apiPipelinesPipelineIdStatusGetRequest struct via the builder pattern


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


## PipelinesPost

> PipelinesPost(ctx).Pipeline(pipeline).Execute()

Register a new pipeline



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
	pipeline := *openapiclient.NewMainRegisterPipelineRequest(int32(123), int32(123), "PipelineName_example", []string{"States_example"}, "micro_batch") // MainRegisterPipelineRequest | Pipeline data

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	r, err := apiClient.PipelinesAPI.PipelinesPost(context.Background()).Pipeline(pipeline).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PipelinesAPI.PipelinesPost``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPipelinesPostRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pipeline** | [**MainRegisterPipelineRequest**](MainRegisterPipelineRequest.md) | Pipeline data | 

### Return type

 (empty response body)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PipelinesSucceededGet

> map[string]int32 PipelinesSucceededGet(ctx).StartTime(startTime).EndTime(endTime).Execute()

Get the number of pipelines that have succeeded



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
	startTime := "startTime_example" // string | Start Time (optional)
	endTime := "endTime_example" // string | End Time (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PipelinesAPI.PipelinesSucceededGet(context.Background()).StartTime(startTime).EndTime(endTime).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PipelinesAPI.PipelinesSucceededGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PipelinesSucceededGet`: map[string]int32
	fmt.Fprintf(os.Stdout, "Response from `PipelinesAPI.PipelinesSucceededGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPipelinesSucceededGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **startTime** | **string** | Start Time | 
 **endTime** | **string** | End Time | 

### Return type

**map[string]int32**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: */*

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PipelinesTotalGet

> map[string]int32 PipelinesTotalGet(ctx).StartTime(startTime).EndTime(endTime).Execute()

Get the total number of pipelines



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
	startTime := "startTime_example" // string | Start Time (optional)
	endTime := "endTime_example" // string | End Time (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PipelinesAPI.PipelinesTotalGet(context.Background()).StartTime(startTime).EndTime(endTime).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PipelinesAPI.PipelinesTotalGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PipelinesTotalGet`: map[string]int32
	fmt.Fprintf(os.Stdout, "Response from `PipelinesAPI.PipelinesTotalGet`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiPipelinesTotalGetRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **startTime** | **string** | Start Time | 
 **endTime** | **string** | End Time | 

### Return type

**map[string]int32**

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: */*

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## PipelinesTypeAverageDurationGet

> map[string]interface{} PipelinesTypeAverageDurationGet(ctx, type_).StartTime(startTime).EndTime(endTime).Execute()

Get the average duration of a specific type of pipeline



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
	type_ := "type__example" // string | Pipeline Type
	startTime := "startTime_example" // string | Start Time (optional)
	endTime := "endTime_example" // string | End Time (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PipelinesAPI.PipelinesTypeAverageDurationGet(context.Background(), type_).StartTime(startTime).EndTime(endTime).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PipelinesAPI.PipelinesTypeAverageDurationGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PipelinesTypeAverageDurationGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PipelinesAPI.PipelinesTypeAverageDurationGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** | Pipeline Type | 

### Other Parameters

Other parameters are passed through a pointer to a apiPipelinesTypeAverageDurationGetRequest struct via the builder pattern


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


## PipelinesTypeMaxDurationGet

> map[string]interface{} PipelinesTypeMaxDurationGet(ctx, type_).StartTime(startTime).EndTime(endTime).Execute()

Get the maximum duration of a specific type of pipeline



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
	type_ := "type__example" // string | Pipeline Type
	startTime := "startTime_example" // string | Start Time (optional)
	endTime := "endTime_example" // string | End Time (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PipelinesAPI.PipelinesTypeMaxDurationGet(context.Background(), type_).StartTime(startTime).EndTime(endTime).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PipelinesAPI.PipelinesTypeMaxDurationGet``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `PipelinesTypeMaxDurationGet`: map[string]interface{}
	fmt.Fprintf(os.Stdout, "Response from `PipelinesAPI.PipelinesTypeMaxDurationGet`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**type_** | **string** | Pipeline Type | 

### Other Parameters

Other parameters are passed through a pointer to a apiPipelinesTypeMaxDurationGetRequest struct via the builder pattern


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

