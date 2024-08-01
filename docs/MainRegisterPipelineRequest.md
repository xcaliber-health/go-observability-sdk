# MainRegisterPipelineRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**NamespaceId** | **int32** |  | 
**ParentPipelineId** | Pointer to **int32** |  | [optional] 
**ParentPipelineName** | Pointer to **string** |  | [optional] 
**PipelineId** | **int32** |  | 
**PipelineName** | **string** |  | 
**States** | **[]string** |  | 
**Type** | **string** |  | 

## Methods

### NewMainRegisterPipelineRequest

`func NewMainRegisterPipelineRequest(namespaceId int32, pipelineId int32, pipelineName string, states []string, type_ string, ) *MainRegisterPipelineRequest`

NewMainRegisterPipelineRequest instantiates a new MainRegisterPipelineRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMainRegisterPipelineRequestWithDefaults

`func NewMainRegisterPipelineRequestWithDefaults() *MainRegisterPipelineRequest`

NewMainRegisterPipelineRequestWithDefaults instantiates a new MainRegisterPipelineRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetNamespaceId

`func (o *MainRegisterPipelineRequest) GetNamespaceId() int32`

GetNamespaceId returns the NamespaceId field if non-nil, zero value otherwise.

### GetNamespaceIdOk

`func (o *MainRegisterPipelineRequest) GetNamespaceIdOk() (*int32, bool)`

GetNamespaceIdOk returns a tuple with the NamespaceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNamespaceId

`func (o *MainRegisterPipelineRequest) SetNamespaceId(v int32)`

SetNamespaceId sets NamespaceId field to given value.


### GetParentPipelineId

`func (o *MainRegisterPipelineRequest) GetParentPipelineId() int32`

GetParentPipelineId returns the ParentPipelineId field if non-nil, zero value otherwise.

### GetParentPipelineIdOk

`func (o *MainRegisterPipelineRequest) GetParentPipelineIdOk() (*int32, bool)`

GetParentPipelineIdOk returns a tuple with the ParentPipelineId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParentPipelineId

`func (o *MainRegisterPipelineRequest) SetParentPipelineId(v int32)`

SetParentPipelineId sets ParentPipelineId field to given value.

### HasParentPipelineId

`func (o *MainRegisterPipelineRequest) HasParentPipelineId() bool`

HasParentPipelineId returns a boolean if a field has been set.

### GetParentPipelineName

`func (o *MainRegisterPipelineRequest) GetParentPipelineName() string`

GetParentPipelineName returns the ParentPipelineName field if non-nil, zero value otherwise.

### GetParentPipelineNameOk

`func (o *MainRegisterPipelineRequest) GetParentPipelineNameOk() (*string, bool)`

GetParentPipelineNameOk returns a tuple with the ParentPipelineName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetParentPipelineName

`func (o *MainRegisterPipelineRequest) SetParentPipelineName(v string)`

SetParentPipelineName sets ParentPipelineName field to given value.

### HasParentPipelineName

`func (o *MainRegisterPipelineRequest) HasParentPipelineName() bool`

HasParentPipelineName returns a boolean if a field has been set.

### GetPipelineId

`func (o *MainRegisterPipelineRequest) GetPipelineId() int32`

GetPipelineId returns the PipelineId field if non-nil, zero value otherwise.

### GetPipelineIdOk

`func (o *MainRegisterPipelineRequest) GetPipelineIdOk() (*int32, bool)`

GetPipelineIdOk returns a tuple with the PipelineId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPipelineId

`func (o *MainRegisterPipelineRequest) SetPipelineId(v int32)`

SetPipelineId sets PipelineId field to given value.


### GetPipelineName

`func (o *MainRegisterPipelineRequest) GetPipelineName() string`

GetPipelineName returns the PipelineName field if non-nil, zero value otherwise.

### GetPipelineNameOk

`func (o *MainRegisterPipelineRequest) GetPipelineNameOk() (*string, bool)`

GetPipelineNameOk returns a tuple with the PipelineName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPipelineName

`func (o *MainRegisterPipelineRequest) SetPipelineName(v string)`

SetPipelineName sets PipelineName field to given value.


### GetStates

`func (o *MainRegisterPipelineRequest) GetStates() []string`

GetStates returns the States field if non-nil, zero value otherwise.

### GetStatesOk

`func (o *MainRegisterPipelineRequest) GetStatesOk() (*[]string, bool)`

GetStatesOk returns a tuple with the States field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStates

`func (o *MainRegisterPipelineRequest) SetStates(v []string)`

SetStates sets States field to given value.


### GetType

`func (o *MainRegisterPipelineRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *MainRegisterPipelineRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *MainRegisterPipelineRequest) SetType(v string)`

SetType sets Type field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


