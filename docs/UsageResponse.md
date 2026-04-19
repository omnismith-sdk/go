# UsageResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeCount** | Pointer to **int32** |  | [optional] 
**TemplateCount** | Pointer to **int32** |  | [optional] 
**EntityCount** | Pointer to **int32** |  | [optional] 
**ProjectCount** | Pointer to **int32** |  | [optional] 
**DashboardCount** | Pointer to **int32** |  | [optional] 
**DiskUsageBytes** | Pointer to **int32** |  | [optional] 
**MonthlyMetricIngestions** | Pointer to **int32** |  | [optional] 
**MonthlyDimensionUpdates** | Pointer to **int32** |  | [optional] 
**AiCreditsUsed** | Pointer to **int32** |  | [optional] 
**UpdatedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewUsageResponse

`func NewUsageResponse() *UsageResponse`

NewUsageResponse instantiates a new UsageResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUsageResponseWithDefaults

`func NewUsageResponseWithDefaults() *UsageResponse`

NewUsageResponseWithDefaults instantiates a new UsageResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeCount

`func (o *UsageResponse) GetAttributeCount() int32`

GetAttributeCount returns the AttributeCount field if non-nil, zero value otherwise.

### GetAttributeCountOk

`func (o *UsageResponse) GetAttributeCountOk() (*int32, bool)`

GetAttributeCountOk returns a tuple with the AttributeCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeCount

`func (o *UsageResponse) SetAttributeCount(v int32)`

SetAttributeCount sets AttributeCount field to given value.

### HasAttributeCount

`func (o *UsageResponse) HasAttributeCount() bool`

HasAttributeCount returns a boolean if a field has been set.

### GetTemplateCount

`func (o *UsageResponse) GetTemplateCount() int32`

GetTemplateCount returns the TemplateCount field if non-nil, zero value otherwise.

### GetTemplateCountOk

`func (o *UsageResponse) GetTemplateCountOk() (*int32, bool)`

GetTemplateCountOk returns a tuple with the TemplateCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateCount

`func (o *UsageResponse) SetTemplateCount(v int32)`

SetTemplateCount sets TemplateCount field to given value.

### HasTemplateCount

`func (o *UsageResponse) HasTemplateCount() bool`

HasTemplateCount returns a boolean if a field has been set.

### GetEntityCount

`func (o *UsageResponse) GetEntityCount() int32`

GetEntityCount returns the EntityCount field if non-nil, zero value otherwise.

### GetEntityCountOk

`func (o *UsageResponse) GetEntityCountOk() (*int32, bool)`

GetEntityCountOk returns a tuple with the EntityCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityCount

`func (o *UsageResponse) SetEntityCount(v int32)`

SetEntityCount sets EntityCount field to given value.

### HasEntityCount

`func (o *UsageResponse) HasEntityCount() bool`

HasEntityCount returns a boolean if a field has been set.

### GetProjectCount

`func (o *UsageResponse) GetProjectCount() int32`

GetProjectCount returns the ProjectCount field if non-nil, zero value otherwise.

### GetProjectCountOk

`func (o *UsageResponse) GetProjectCountOk() (*int32, bool)`

GetProjectCountOk returns a tuple with the ProjectCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProjectCount

`func (o *UsageResponse) SetProjectCount(v int32)`

SetProjectCount sets ProjectCount field to given value.

### HasProjectCount

`func (o *UsageResponse) HasProjectCount() bool`

HasProjectCount returns a boolean if a field has been set.

### GetDashboardCount

`func (o *UsageResponse) GetDashboardCount() int32`

GetDashboardCount returns the DashboardCount field if non-nil, zero value otherwise.

### GetDashboardCountOk

`func (o *UsageResponse) GetDashboardCountOk() (*int32, bool)`

GetDashboardCountOk returns a tuple with the DashboardCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDashboardCount

`func (o *UsageResponse) SetDashboardCount(v int32)`

SetDashboardCount sets DashboardCount field to given value.

### HasDashboardCount

`func (o *UsageResponse) HasDashboardCount() bool`

HasDashboardCount returns a boolean if a field has been set.

### GetDiskUsageBytes

`func (o *UsageResponse) GetDiskUsageBytes() int32`

GetDiskUsageBytes returns the DiskUsageBytes field if non-nil, zero value otherwise.

### GetDiskUsageBytesOk

`func (o *UsageResponse) GetDiskUsageBytesOk() (*int32, bool)`

GetDiskUsageBytesOk returns a tuple with the DiskUsageBytes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDiskUsageBytes

`func (o *UsageResponse) SetDiskUsageBytes(v int32)`

SetDiskUsageBytes sets DiskUsageBytes field to given value.

### HasDiskUsageBytes

`func (o *UsageResponse) HasDiskUsageBytes() bool`

HasDiskUsageBytes returns a boolean if a field has been set.

### GetMonthlyMetricIngestions

`func (o *UsageResponse) GetMonthlyMetricIngestions() int32`

GetMonthlyMetricIngestions returns the MonthlyMetricIngestions field if non-nil, zero value otherwise.

### GetMonthlyMetricIngestionsOk

`func (o *UsageResponse) GetMonthlyMetricIngestionsOk() (*int32, bool)`

GetMonthlyMetricIngestionsOk returns a tuple with the MonthlyMetricIngestions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonthlyMetricIngestions

`func (o *UsageResponse) SetMonthlyMetricIngestions(v int32)`

SetMonthlyMetricIngestions sets MonthlyMetricIngestions field to given value.

### HasMonthlyMetricIngestions

`func (o *UsageResponse) HasMonthlyMetricIngestions() bool`

HasMonthlyMetricIngestions returns a boolean if a field has been set.

### GetMonthlyDimensionUpdates

`func (o *UsageResponse) GetMonthlyDimensionUpdates() int32`

GetMonthlyDimensionUpdates returns the MonthlyDimensionUpdates field if non-nil, zero value otherwise.

### GetMonthlyDimensionUpdatesOk

`func (o *UsageResponse) GetMonthlyDimensionUpdatesOk() (*int32, bool)`

GetMonthlyDimensionUpdatesOk returns a tuple with the MonthlyDimensionUpdates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMonthlyDimensionUpdates

`func (o *UsageResponse) SetMonthlyDimensionUpdates(v int32)`

SetMonthlyDimensionUpdates sets MonthlyDimensionUpdates field to given value.

### HasMonthlyDimensionUpdates

`func (o *UsageResponse) HasMonthlyDimensionUpdates() bool`

HasMonthlyDimensionUpdates returns a boolean if a field has been set.

### GetAiCreditsUsed

`func (o *UsageResponse) GetAiCreditsUsed() int32`

GetAiCreditsUsed returns the AiCreditsUsed field if non-nil, zero value otherwise.

### GetAiCreditsUsedOk

`func (o *UsageResponse) GetAiCreditsUsedOk() (*int32, bool)`

GetAiCreditsUsedOk returns a tuple with the AiCreditsUsed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAiCreditsUsed

`func (o *UsageResponse) SetAiCreditsUsed(v int32)`

SetAiCreditsUsed sets AiCreditsUsed field to given value.

### HasAiCreditsUsed

`func (o *UsageResponse) HasAiCreditsUsed() bool`

HasAiCreditsUsed returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *UsageResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *UsageResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *UsageResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *UsageResponse) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


