# UpdateDashboardRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **NullableString** | Updated display name of the dashboard | [optional] 
**Description** | Pointer to **NullableString** | Updated description of the dashboard purpose and telemetry scope | [optional] 
**Config** | Pointer to [**NullableUpdateDashboardRequestConfig**](UpdateDashboardRequestConfig.md) |  | [optional] 

## Methods

### NewUpdateDashboardRequest

`func NewUpdateDashboardRequest() *UpdateDashboardRequest`

NewUpdateDashboardRequest instantiates a new UpdateDashboardRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateDashboardRequestWithDefaults

`func NewUpdateDashboardRequestWithDefaults() *UpdateDashboardRequest`

NewUpdateDashboardRequestWithDefaults instantiates a new UpdateDashboardRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *UpdateDashboardRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateDashboardRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateDashboardRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *UpdateDashboardRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *UpdateDashboardRequest) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *UpdateDashboardRequest) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetDescription

`func (o *UpdateDashboardRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *UpdateDashboardRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *UpdateDashboardRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *UpdateDashboardRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *UpdateDashboardRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *UpdateDashboardRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetConfig

`func (o *UpdateDashboardRequest) GetConfig() UpdateDashboardRequestConfig`

GetConfig returns the Config field if non-nil, zero value otherwise.

### GetConfigOk

`func (o *UpdateDashboardRequest) GetConfigOk() (*UpdateDashboardRequestConfig, bool)`

GetConfigOk returns a tuple with the Config field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfig

`func (o *UpdateDashboardRequest) SetConfig(v UpdateDashboardRequestConfig)`

SetConfig sets Config field to given value.

### HasConfig

`func (o *UpdateDashboardRequest) HasConfig() bool`

HasConfig returns a boolean if a field has been set.

### SetConfigNil

`func (o *UpdateDashboardRequest) SetConfigNil(b bool)`

 SetConfigNil sets the value for Config to be an explicit nil

### UnsetConfig
`func (o *UpdateDashboardRequest) UnsetConfig()`

UnsetConfig ensures that no value is present for Config, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


