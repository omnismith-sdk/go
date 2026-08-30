# CreateDashboardRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Display name of the dashboard | 
**Description** | Pointer to **string** | Detailed description of the dashboard purpose and telemetry scope | [optional] 
**Config** | Pointer to [**CreateDashboardRequestConfig**](CreateDashboardRequestConfig.md) |  | [optional] 

## Methods

### NewCreateDashboardRequest

`func NewCreateDashboardRequest(name string, ) *CreateDashboardRequest`

NewCreateDashboardRequest instantiates a new CreateDashboardRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateDashboardRequestWithDefaults

`func NewCreateDashboardRequestWithDefaults() *CreateDashboardRequest`

NewCreateDashboardRequestWithDefaults instantiates a new CreateDashboardRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreateDashboardRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateDashboardRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateDashboardRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *CreateDashboardRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateDashboardRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateDashboardRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CreateDashboardRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetConfig

`func (o *CreateDashboardRequest) GetConfig() CreateDashboardRequestConfig`

GetConfig returns the Config field if non-nil, zero value otherwise.

### GetConfigOk

`func (o *CreateDashboardRequest) GetConfigOk() (*CreateDashboardRequestConfig, bool)`

GetConfigOk returns a tuple with the Config field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfig

`func (o *CreateDashboardRequest) SetConfig(v CreateDashboardRequestConfig)`

SetConfig sets Config field to given value.

### HasConfig

`func (o *CreateDashboardRequest) HasConfig() bool`

HasConfig returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


