# UpdateDashboardBlockRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | Pointer to **NullableString** | Updated display title for the widget card header | [optional] 
**Config** | Pointer to [**NullableUpdateDashboardBlockRequestConfig**](UpdateDashboardBlockRequestConfig.md) |  | [optional] 

## Methods

### NewUpdateDashboardBlockRequest

`func NewUpdateDashboardBlockRequest() *UpdateDashboardBlockRequest`

NewUpdateDashboardBlockRequest instantiates a new UpdateDashboardBlockRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateDashboardBlockRequestWithDefaults

`func NewUpdateDashboardBlockRequestWithDefaults() *UpdateDashboardBlockRequest`

NewUpdateDashboardBlockRequestWithDefaults instantiates a new UpdateDashboardBlockRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTitle

`func (o *UpdateDashboardBlockRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *UpdateDashboardBlockRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *UpdateDashboardBlockRequest) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *UpdateDashboardBlockRequest) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### SetTitleNil

`func (o *UpdateDashboardBlockRequest) SetTitleNil(b bool)`

 SetTitleNil sets the value for Title to be an explicit nil

### UnsetTitle
`func (o *UpdateDashboardBlockRequest) UnsetTitle()`

UnsetTitle ensures that no value is present for Title, not even an explicit nil
### GetConfig

`func (o *UpdateDashboardBlockRequest) GetConfig() UpdateDashboardBlockRequestConfig`

GetConfig returns the Config field if non-nil, zero value otherwise.

### GetConfigOk

`func (o *UpdateDashboardBlockRequest) GetConfigOk() (*UpdateDashboardBlockRequestConfig, bool)`

GetConfigOk returns a tuple with the Config field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfig

`func (o *UpdateDashboardBlockRequest) SetConfig(v UpdateDashboardBlockRequestConfig)`

SetConfig sets Config field to given value.

### HasConfig

`func (o *UpdateDashboardBlockRequest) HasConfig() bool`

HasConfig returns a boolean if a field has been set.

### SetConfigNil

`func (o *UpdateDashboardBlockRequest) SetConfigNil(b bool)`

 SetConfigNil sets the value for Config to be an explicit nil

### UnsetConfig
`func (o *UpdateDashboardBlockRequest) UnsetConfig()`

UnsetConfig ensures that no value is present for Config, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


