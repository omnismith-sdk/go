# UpdateDashboardBlockRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | Pointer to **string** |  | [optional] 
**Config** | Pointer to **map[string]interface{}** | Block-specific configuration | [optional] 

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

### GetConfig

`func (o *UpdateDashboardBlockRequest) GetConfig() map[string]interface{}`

GetConfig returns the Config field if non-nil, zero value otherwise.

### GetConfigOk

`func (o *UpdateDashboardBlockRequest) GetConfigOk() (*map[string]interface{}, bool)`

GetConfigOk returns a tuple with the Config field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfig

`func (o *UpdateDashboardBlockRequest) SetConfig(v map[string]interface{})`

SetConfig sets Config field to given value.

### HasConfig

`func (o *UpdateDashboardBlockRequest) HasConfig() bool`

HasConfig returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


