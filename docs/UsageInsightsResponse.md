# UsageInsightsResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TierId** | Pointer to **string** | The ID of the current tier | [optional] 
**Usage** | Pointer to [**UsageInsightsResponseUsage**](UsageInsightsResponseUsage.md) |  | [optional] 
**Limits** | Pointer to [**UsageInsightsResponseUsage**](UsageInsightsResponseUsage.md) |  | [optional] 
**Percentages** | Pointer to [**UsageInsightsResponsePercentages**](UsageInsightsResponsePercentages.md) |  | [optional] 

## Methods

### NewUsageInsightsResponse

`func NewUsageInsightsResponse() *UsageInsightsResponse`

NewUsageInsightsResponse instantiates a new UsageInsightsResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUsageInsightsResponseWithDefaults

`func NewUsageInsightsResponseWithDefaults() *UsageInsightsResponse`

NewUsageInsightsResponseWithDefaults instantiates a new UsageInsightsResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTierId

`func (o *UsageInsightsResponse) GetTierId() string`

GetTierId returns the TierId field if non-nil, zero value otherwise.

### GetTierIdOk

`func (o *UsageInsightsResponse) GetTierIdOk() (*string, bool)`

GetTierIdOk returns a tuple with the TierId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTierId

`func (o *UsageInsightsResponse) SetTierId(v string)`

SetTierId sets TierId field to given value.

### HasTierId

`func (o *UsageInsightsResponse) HasTierId() bool`

HasTierId returns a boolean if a field has been set.

### GetUsage

`func (o *UsageInsightsResponse) GetUsage() UsageInsightsResponseUsage`

GetUsage returns the Usage field if non-nil, zero value otherwise.

### GetUsageOk

`func (o *UsageInsightsResponse) GetUsageOk() (*UsageInsightsResponseUsage, bool)`

GetUsageOk returns a tuple with the Usage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsage

`func (o *UsageInsightsResponse) SetUsage(v UsageInsightsResponseUsage)`

SetUsage sets Usage field to given value.

### HasUsage

`func (o *UsageInsightsResponse) HasUsage() bool`

HasUsage returns a boolean if a field has been set.

### GetLimits

`func (o *UsageInsightsResponse) GetLimits() UsageInsightsResponseUsage`

GetLimits returns the Limits field if non-nil, zero value otherwise.

### GetLimitsOk

`func (o *UsageInsightsResponse) GetLimitsOk() (*UsageInsightsResponseUsage, bool)`

GetLimitsOk returns a tuple with the Limits field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimits

`func (o *UsageInsightsResponse) SetLimits(v UsageInsightsResponseUsage)`

SetLimits sets Limits field to given value.

### HasLimits

`func (o *UsageInsightsResponse) HasLimits() bool`

HasLimits returns a boolean if a field has been set.

### GetPercentages

`func (o *UsageInsightsResponse) GetPercentages() UsageInsightsResponsePercentages`

GetPercentages returns the Percentages field if non-nil, zero value otherwise.

### GetPercentagesOk

`func (o *UsageInsightsResponse) GetPercentagesOk() (*UsageInsightsResponsePercentages, bool)`

GetPercentagesOk returns a tuple with the Percentages field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPercentages

`func (o *UsageInsightsResponse) SetPercentages(v UsageInsightsResponsePercentages)`

SetPercentages sets Percentages field to given value.

### HasPercentages

`func (o *UsageInsightsResponse) HasPercentages() bool`

HasPercentages returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


