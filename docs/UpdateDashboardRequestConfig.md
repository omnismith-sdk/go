# UpdateDashboardRequestConfig

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**MinCols** | Pointer to **int32** | Minimum number of grid columns (standard: 12) | [optional] [default to 12]
**MaxCols** | Pointer to **int32** | Maximum number of grid columns (standard: 12) | [optional] [default to 12]
**MinRows** | Pointer to **int32** | Minimum number of grid rows (standard: 1) | [optional] [default to 1]
**MaxRows** | Pointer to **int32** | Maximum number of grid rows (standard: 100) | [optional] [default to 100]
**AutoRefresh** | Pointer to **int32** | Auto-refresh interval in seconds (0 &#x3D; off, 30, 60, 300) | [optional] [default to 0]
**Thumbnail** | Pointer to **NullableString** | Base64 data URL preview thumbnail of the dashboard canvas | [optional] 

## Methods

### NewUpdateDashboardRequestConfig

`func NewUpdateDashboardRequestConfig() *UpdateDashboardRequestConfig`

NewUpdateDashboardRequestConfig instantiates a new UpdateDashboardRequestConfig object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateDashboardRequestConfigWithDefaults

`func NewUpdateDashboardRequestConfigWithDefaults() *UpdateDashboardRequestConfig`

NewUpdateDashboardRequestConfigWithDefaults instantiates a new UpdateDashboardRequestConfig object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMinCols

`func (o *UpdateDashboardRequestConfig) GetMinCols() int32`

GetMinCols returns the MinCols field if non-nil, zero value otherwise.

### GetMinColsOk

`func (o *UpdateDashboardRequestConfig) GetMinColsOk() (*int32, bool)`

GetMinColsOk returns a tuple with the MinCols field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinCols

`func (o *UpdateDashboardRequestConfig) SetMinCols(v int32)`

SetMinCols sets MinCols field to given value.

### HasMinCols

`func (o *UpdateDashboardRequestConfig) HasMinCols() bool`

HasMinCols returns a boolean if a field has been set.

### GetMaxCols

`func (o *UpdateDashboardRequestConfig) GetMaxCols() int32`

GetMaxCols returns the MaxCols field if non-nil, zero value otherwise.

### GetMaxColsOk

`func (o *UpdateDashboardRequestConfig) GetMaxColsOk() (*int32, bool)`

GetMaxColsOk returns a tuple with the MaxCols field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxCols

`func (o *UpdateDashboardRequestConfig) SetMaxCols(v int32)`

SetMaxCols sets MaxCols field to given value.

### HasMaxCols

`func (o *UpdateDashboardRequestConfig) HasMaxCols() bool`

HasMaxCols returns a boolean if a field has been set.

### GetMinRows

`func (o *UpdateDashboardRequestConfig) GetMinRows() int32`

GetMinRows returns the MinRows field if non-nil, zero value otherwise.

### GetMinRowsOk

`func (o *UpdateDashboardRequestConfig) GetMinRowsOk() (*int32, bool)`

GetMinRowsOk returns a tuple with the MinRows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMinRows

`func (o *UpdateDashboardRequestConfig) SetMinRows(v int32)`

SetMinRows sets MinRows field to given value.

### HasMinRows

`func (o *UpdateDashboardRequestConfig) HasMinRows() bool`

HasMinRows returns a boolean if a field has been set.

### GetMaxRows

`func (o *UpdateDashboardRequestConfig) GetMaxRows() int32`

GetMaxRows returns the MaxRows field if non-nil, zero value otherwise.

### GetMaxRowsOk

`func (o *UpdateDashboardRequestConfig) GetMaxRowsOk() (*int32, bool)`

GetMaxRowsOk returns a tuple with the MaxRows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMaxRows

`func (o *UpdateDashboardRequestConfig) SetMaxRows(v int32)`

SetMaxRows sets MaxRows field to given value.

### HasMaxRows

`func (o *UpdateDashboardRequestConfig) HasMaxRows() bool`

HasMaxRows returns a boolean if a field has been set.

### GetAutoRefresh

`func (o *UpdateDashboardRequestConfig) GetAutoRefresh() int32`

GetAutoRefresh returns the AutoRefresh field if non-nil, zero value otherwise.

### GetAutoRefreshOk

`func (o *UpdateDashboardRequestConfig) GetAutoRefreshOk() (*int32, bool)`

GetAutoRefreshOk returns a tuple with the AutoRefresh field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAutoRefresh

`func (o *UpdateDashboardRequestConfig) SetAutoRefresh(v int32)`

SetAutoRefresh sets AutoRefresh field to given value.

### HasAutoRefresh

`func (o *UpdateDashboardRequestConfig) HasAutoRefresh() bool`

HasAutoRefresh returns a boolean if a field has been set.

### GetThumbnail

`func (o *UpdateDashboardRequestConfig) GetThumbnail() string`

GetThumbnail returns the Thumbnail field if non-nil, zero value otherwise.

### GetThumbnailOk

`func (o *UpdateDashboardRequestConfig) GetThumbnailOk() (*string, bool)`

GetThumbnailOk returns a tuple with the Thumbnail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetThumbnail

`func (o *UpdateDashboardRequestConfig) SetThumbnail(v string)`

SetThumbnail sets Thumbnail field to given value.

### HasThumbnail

`func (o *UpdateDashboardRequestConfig) HasThumbnail() bool`

HasThumbnail returns a boolean if a field has been set.

### SetThumbnailNil

`func (o *UpdateDashboardRequestConfig) SetThumbnailNil(b bool)`

 SetThumbnailNil sets the value for Thumbnail to be an explicit nil

### UnsetThumbnail
`func (o *UpdateDashboardRequestConfig) UnsetThumbnail()`

UnsetThumbnail ensures that no value is present for Thumbnail, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


