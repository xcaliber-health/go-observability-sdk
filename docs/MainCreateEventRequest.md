# MainCreateEventRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**DataProductId** | Pointer to **int32** |  | [optional] 
**MicroBatchId** | Pointer to **string** |  | [optional] 
**NamespaceId** | Pointer to **int32** |  | [optional] 
**ParentPipelineID** | Pointer to **int32** |  | [optional] 
**ParentPipelineWorkflowID** | Pointer to **string** |  | [optional] 
**PipelineID** | Pointer to **int32** |  | [optional] 
**SourceId** | Pointer to **int32** |  | [optional] 
**State** | Pointer to **string** |  | [optional] 
**TenantId** | Pointer to **int32** |  | [optional] 
**Timestamp** | Pointer to **string** |  | [optional] 
**WorkflowID** | Pointer to **string** |  | [optional] 

## Methods

### NewMainCreateEventRequest

`func NewMainCreateEventRequest() *MainCreateEventRequest`

NewMainCreateEventRequest instantiates a new MainCreateEventRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMainCreateEventRequestWithDefaults

`func NewMainCreateEventRequestWithDefaults() *MainCreateEventRequest`

NewMainCreateEventRequestWithDefaults instantiates a new MainCreateEventRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetDataProductId

`func (o *MainCreateEventRequest) GetDataProductId() int32`

GetDataProductId returns the DataProductId field if non-nil, zero value otherwise.

### GetDataProductIdOk

`func (o *MainCreateEventRequest) GetDataProductIdOk() (*int32, bool)`

GetDataProductIdOk returns a tuple with the DataProductId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataProductId

`func (o *MainCreateEventRequest) SetDataProductId(v int32)`

SetDataProductId sets DataProductId field to given value.

### HasDataProductId

`func (o *MainCreateEventRequest) HasDataProductId() bool`

HasDataProductId returns a boolean if a field has been set.

### GetMicroBatchId

`func (o *MainCreateEventRequest) GetMicroBatchId() string`

GetMicroBatchId returns the MicroBatchId field if non-nil, zero value otherwise.

### GetMicroBatchIdOk

`func (o *MainCreateEventRequest) GetMicroBatchIdOk() (*string, bool)`

GetMicroBatchIdOk returns a tuple with the MicroBatchId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMicroBatchId

`func (o *MainCreateEventRequest) SetMicroBatchId(v string)`

SetMicroBatchId sets MicroBatchId field to given value.

### HasMicroBatchId

`func (o *MainCreateEventRequest) HasMicroBatchId() bool`

HasMicroBatchId returns a boolean if a field has been set.

### GetNamespaceId

`func (o *MainCreateEventRequest) GetNamespaceId() int32`

GetNamespaceId returns the NamespaceId field if non-nil, zero value otherwise.

### GetNamespaceIdOk

`func (o *MainCreateEventRequest) GetNamespaceIdOk() (*int32, bool)`

GetNamespaceIdOk returns a tuple with the NamespaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNamespaceId

`func (o *MainCreateEventRequest) SetNamespaceId(v int32)`

SetNamespaceId sets NamespaceId field to given value.

### HasNamespaceId

`func (o *MainCreateEventRequest) HasNamespaceId() bool`

HasNamespaceId returns a boolean if a field has been set.

### GetParentPipelineID

`func (o *MainCreateEventRequest) GetParentPipelineID() int32`

GetParentPipelineID returns the ParentPipelineID field if non-nil, zero value otherwise.

### GetParentPipelineIDOk

`func (o *MainCreateEventRequest) GetParentPipelineIDOk() (*int32, bool)`

GetParentPipelineIDOk returns a tuple with the ParentPipelineID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParentPipelineID

`func (o *MainCreateEventRequest) SetParentPipelineID(v int32)`

SetParentPipelineID sets ParentPipelineID field to given value.

### HasParentPipelineID

`func (o *MainCreateEventRequest) HasParentPipelineID() bool`

HasParentPipelineID returns a boolean if a field has been set.

### GetParentPipelineWorkflowID

`func (o *MainCreateEventRequest) GetParentPipelineWorkflowID() string`

GetParentPipelineWorkflowID returns the ParentPipelineWorkflowID field if non-nil, zero value otherwise.

### GetParentPipelineWorkflowIDOk

`func (o *MainCreateEventRequest) GetParentPipelineWorkflowIDOk() (*string, bool)`

GetParentPipelineWorkflowIDOk returns a tuple with the ParentPipelineWorkflowID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParentPipelineWorkflowID

`func (o *MainCreateEventRequest) SetParentPipelineWorkflowID(v string)`

SetParentPipelineWorkflowID sets ParentPipelineWorkflowID field to given value.

### HasParentPipelineWorkflowID

`func (o *MainCreateEventRequest) HasParentPipelineWorkflowID() bool`

HasParentPipelineWorkflowID returns a boolean if a field has been set.

### GetPipelineID

`func (o *MainCreateEventRequest) GetPipelineID() int32`

GetPipelineID returns the PipelineID field if non-nil, zero value otherwise.

### GetPipelineIDOk

`func (o *MainCreateEventRequest) GetPipelineIDOk() (*int32, bool)`

GetPipelineIDOk returns a tuple with the PipelineID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPipelineID

`func (o *MainCreateEventRequest) SetPipelineID(v int32)`

SetPipelineID sets PipelineID field to given value.

### HasPipelineID

`func (o *MainCreateEventRequest) HasPipelineID() bool`

HasPipelineID returns a boolean if a field has been set.

### GetSourceId

`func (o *MainCreateEventRequest) GetSourceId() int32`

GetSourceId returns the SourceId field if non-nil, zero value otherwise.

### GetSourceIdOk

`func (o *MainCreateEventRequest) GetSourceIdOk() (*int32, bool)`

GetSourceIdOk returns a tuple with the SourceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSourceId

`func (o *MainCreateEventRequest) SetSourceId(v int32)`

SetSourceId sets SourceId field to given value.

### HasSourceId

`func (o *MainCreateEventRequest) HasSourceId() bool`

HasSourceId returns a boolean if a field has been set.

### GetState

`func (o *MainCreateEventRequest) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *MainCreateEventRequest) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *MainCreateEventRequest) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *MainCreateEventRequest) HasState() bool`

HasState returns a boolean if a field has been set.

### GetTenantId

`func (o *MainCreateEventRequest) GetTenantId() int32`

GetTenantId returns the TenantId field if non-nil, zero value otherwise.

### GetTenantIdOk

`func (o *MainCreateEventRequest) GetTenantIdOk() (*int32, bool)`

GetTenantIdOk returns a tuple with the TenantId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTenantId

`func (o *MainCreateEventRequest) SetTenantId(v int32)`

SetTenantId sets TenantId field to given value.

### HasTenantId

`func (o *MainCreateEventRequest) HasTenantId() bool`

HasTenantId returns a boolean if a field has been set.

### GetTimestamp

`func (o *MainCreateEventRequest) GetTimestamp() string`

GetTimestamp returns the Timestamp field if non-nil, zero value otherwise.

### GetTimestampOk

`func (o *MainCreateEventRequest) GetTimestampOk() (*string, bool)`

GetTimestampOk returns a tuple with the Timestamp field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimestamp

`func (o *MainCreateEventRequest) SetTimestamp(v string)`

SetTimestamp sets Timestamp field to given value.

### HasTimestamp

`func (o *MainCreateEventRequest) HasTimestamp() bool`

HasTimestamp returns a boolean if a field has been set.

### GetWorkflowID

`func (o *MainCreateEventRequest) GetWorkflowID() string`

GetWorkflowID returns the WorkflowID field if non-nil, zero value otherwise.

### GetWorkflowIDOk

`func (o *MainCreateEventRequest) GetWorkflowIDOk() (*string, bool)`

GetWorkflowIDOk returns a tuple with the WorkflowID field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetWorkflowID

`func (o *MainCreateEventRequest) SetWorkflowID(v string)`

SetWorkflowID sets WorkflowID field to given value.

### HasWorkflowID

`func (o *MainCreateEventRequest) HasWorkflowID() bool`

HasWorkflowID returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


