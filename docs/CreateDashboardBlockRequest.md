# CreateDashboardBlockRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** | Block visualization type: stat (single KPI counter of matching entities), chart (time-series telemetry multi-line graph aggregating metric values over time), gauge (radial threshold meter displaying metric aggregate within bounds), list (filtered and sorted entity data table). | 
**Title** | **string** | Header title displayed on the dashboard widget card (e.g., \&quot;CPU Utilization — Time Series\&quot;, \&quot;Total Servers\&quot;, \&quot;Peak CPU Utilization\&quot;). | 
**Config** | Pointer to [**CreateDashboardBlockRequestConfig**](CreateDashboardBlockRequestConfig.md) |  | [optional] 

## Methods

### NewCreateDashboardBlockRequest

`func NewCreateDashboardBlockRequest(type_ string, title string, ) *CreateDashboardBlockRequest`

NewCreateDashboardBlockRequest instantiates a new CreateDashboardBlockRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateDashboardBlockRequestWithDefaults

`func NewCreateDashboardBlockRequestWithDefaults() *CreateDashboardBlockRequest`

NewCreateDashboardBlockRequestWithDefaults instantiates a new CreateDashboardBlockRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *CreateDashboardBlockRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CreateDashboardBlockRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CreateDashboardBlockRequest) SetType(v string)`

SetType sets Type field to given value.


### GetTitle

`func (o *CreateDashboardBlockRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *CreateDashboardBlockRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *CreateDashboardBlockRequest) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetConfig

`func (o *CreateDashboardBlockRequest) GetConfig() CreateDashboardBlockRequestConfig`

GetConfig returns the Config field if non-nil, zero value otherwise.

### GetConfigOk

`func (o *CreateDashboardBlockRequest) GetConfigOk() (*CreateDashboardBlockRequestConfig, bool)`

GetConfigOk returns a tuple with the Config field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfig

`func (o *CreateDashboardBlockRequest) SetConfig(v CreateDashboardBlockRequestConfig)`

SetConfig sets Config field to given value.

### HasConfig

`func (o *CreateDashboardBlockRequest) HasConfig() bool`

HasConfig returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


