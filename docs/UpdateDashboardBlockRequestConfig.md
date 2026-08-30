# UpdateDashboardBlockRequestConfig

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | Pointer to **NullableString** | UUID of the entity template | [optional] 
**MetricAttributeId** | Pointer to **NullableString** | UUID of the metric attribute | [optional] 
**TimeWindow** | Pointer to **NullableInt32** | Time range query window in seconds for historical telemetry (e.g. 3600, 10800, 21600, 43200, 86400, 604800, 2592000) | [optional] 
**BucketWidth** | Pointer to **NullableString** | Time bucket interval for chart aggregation (e.g. \&quot;1 min\&quot;, \&quot;5 min\&quot;, \&quot;1 hour\&quot;, \&quot;1 day\&quot;) | [optional] 
**Aggregate** | Pointer to **NullableString** | Aggregation function (\&quot;avg\&quot;, \&quot;sum\&quot;, \&quot;min\&quot;, \&quot;max\&quot;, \&quot;first\&quot;, \&quot;last\&quot;, \&quot;count\&quot;) | [optional] 
**EntityLimit** | Pointer to **NullableInt32** | Maximum entity series count (1-50) | [optional] 
**Min** | Pointer to **NullableFloat32** | Minimum scale value for gauge blocks | [optional] 
**Max** | Pointer to **NullableFloat32** | Maximum scale value for gauge blocks | [optional] 
**Unit** | Pointer to **NullableString** | Unit suffix for gauge blocks (e.g. \&quot;%\&quot;) | [optional] 
**StartColor** | Pointer to **NullableString** | Start gradient color | [optional] 
**MidColor** | Pointer to **NullableString** | Middle gradient color | [optional] 
**EndColor** | Pointer to **NullableString** | End gradient color | [optional] 
**Limit** | Pointer to **NullableInt32** | Entity limit for list blocks | [optional] 
**Sort** | Pointer to **map[string]interface{}** | Sort config object for list blocks | [optional] 
**VisibleAttributes** | Pointer to **[]string** | List block visible attribute IDs | [optional] 
**Filters** | Pointer to **[]map[string]interface{}** | Entity filter rules | [optional] 
**X** | Pointer to **NullableInt32** | Horizontal grid column (0..11 on 12-column grid) | [optional] 
**Y** | Pointer to **NullableInt32** | Vertical grid row (0..N) | [optional] 
**Cols** | Pointer to **NullableInt32** | Block width in columns (1..12) | [optional] 
**Rows** | Pointer to **NullableInt32** | Block height in rows (1..N) | [optional] 

## Methods

### NewUpdateDashboardBlockRequestConfig

`func NewUpdateDashboardBlockRequestConfig() *UpdateDashboardBlockRequestConfig`

NewUpdateDashboardBlockRequestConfig instantiates a new UpdateDashboardBlockRequestConfig object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateDashboardBlockRequestConfigWithDefaults

`func NewUpdateDashboardBlockRequestConfigWithDefaults() *UpdateDashboardBlockRequestConfig`

NewUpdateDashboardBlockRequestConfigWithDefaults instantiates a new UpdateDashboardBlockRequestConfig object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *UpdateDashboardBlockRequestConfig) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *UpdateDashboardBlockRequestConfig) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *UpdateDashboardBlockRequestConfig) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *UpdateDashboardBlockRequestConfig) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### SetTemplateIdNil

`func (o *UpdateDashboardBlockRequestConfig) SetTemplateIdNil(b bool)`

 SetTemplateIdNil sets the value for TemplateId to be an explicit nil

### UnsetTemplateId
`func (o *UpdateDashboardBlockRequestConfig) UnsetTemplateId()`

UnsetTemplateId ensures that no value is present for TemplateId, not even an explicit nil
### GetMetricAttributeId

`func (o *UpdateDashboardBlockRequestConfig) GetMetricAttributeId() string`

GetMetricAttributeId returns the MetricAttributeId field if non-nil, zero value otherwise.

### GetMetricAttributeIdOk

`func (o *UpdateDashboardBlockRequestConfig) GetMetricAttributeIdOk() (*string, bool)`

GetMetricAttributeIdOk returns a tuple with the MetricAttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetricAttributeId

`func (o *UpdateDashboardBlockRequestConfig) SetMetricAttributeId(v string)`

SetMetricAttributeId sets MetricAttributeId field to given value.

### HasMetricAttributeId

`func (o *UpdateDashboardBlockRequestConfig) HasMetricAttributeId() bool`

HasMetricAttributeId returns a boolean if a field has been set.

### SetMetricAttributeIdNil

`func (o *UpdateDashboardBlockRequestConfig) SetMetricAttributeIdNil(b bool)`

 SetMetricAttributeIdNil sets the value for MetricAttributeId to be an explicit nil

### UnsetMetricAttributeId
`func (o *UpdateDashboardBlockRequestConfig) UnsetMetricAttributeId()`

UnsetMetricAttributeId ensures that no value is present for MetricAttributeId, not even an explicit nil
### GetTimeWindow

`func (o *UpdateDashboardBlockRequestConfig) GetTimeWindow() int32`

GetTimeWindow returns the TimeWindow field if non-nil, zero value otherwise.

### GetTimeWindowOk

`func (o *UpdateDashboardBlockRequestConfig) GetTimeWindowOk() (*int32, bool)`

GetTimeWindowOk returns a tuple with the TimeWindow field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimeWindow

`func (o *UpdateDashboardBlockRequestConfig) SetTimeWindow(v int32)`

SetTimeWindow sets TimeWindow field to given value.

### HasTimeWindow

`func (o *UpdateDashboardBlockRequestConfig) HasTimeWindow() bool`

HasTimeWindow returns a boolean if a field has been set.

### SetTimeWindowNil

`func (o *UpdateDashboardBlockRequestConfig) SetTimeWindowNil(b bool)`

 SetTimeWindowNil sets the value for TimeWindow to be an explicit nil

### UnsetTimeWindow
`func (o *UpdateDashboardBlockRequestConfig) UnsetTimeWindow()`

UnsetTimeWindow ensures that no value is present for TimeWindow, not even an explicit nil
### GetBucketWidth

`func (o *UpdateDashboardBlockRequestConfig) GetBucketWidth() string`

GetBucketWidth returns the BucketWidth field if non-nil, zero value otherwise.

### GetBucketWidthOk

`func (o *UpdateDashboardBlockRequestConfig) GetBucketWidthOk() (*string, bool)`

GetBucketWidthOk returns a tuple with the BucketWidth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBucketWidth

`func (o *UpdateDashboardBlockRequestConfig) SetBucketWidth(v string)`

SetBucketWidth sets BucketWidth field to given value.

### HasBucketWidth

`func (o *UpdateDashboardBlockRequestConfig) HasBucketWidth() bool`

HasBucketWidth returns a boolean if a field has been set.

### SetBucketWidthNil

`func (o *UpdateDashboardBlockRequestConfig) SetBucketWidthNil(b bool)`

 SetBucketWidthNil sets the value for BucketWidth to be an explicit nil

### UnsetBucketWidth
`func (o *UpdateDashboardBlockRequestConfig) UnsetBucketWidth()`

UnsetBucketWidth ensures that no value is present for BucketWidth, not even an explicit nil
### GetAggregate

`func (o *UpdateDashboardBlockRequestConfig) GetAggregate() string`

GetAggregate returns the Aggregate field if non-nil, zero value otherwise.

### GetAggregateOk

`func (o *UpdateDashboardBlockRequestConfig) GetAggregateOk() (*string, bool)`

GetAggregateOk returns a tuple with the Aggregate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAggregate

`func (o *UpdateDashboardBlockRequestConfig) SetAggregate(v string)`

SetAggregate sets Aggregate field to given value.

### HasAggregate

`func (o *UpdateDashboardBlockRequestConfig) HasAggregate() bool`

HasAggregate returns a boolean if a field has been set.

### SetAggregateNil

`func (o *UpdateDashboardBlockRequestConfig) SetAggregateNil(b bool)`

 SetAggregateNil sets the value for Aggregate to be an explicit nil

### UnsetAggregate
`func (o *UpdateDashboardBlockRequestConfig) UnsetAggregate()`

UnsetAggregate ensures that no value is present for Aggregate, not even an explicit nil
### GetEntityLimit

`func (o *UpdateDashboardBlockRequestConfig) GetEntityLimit() int32`

GetEntityLimit returns the EntityLimit field if non-nil, zero value otherwise.

### GetEntityLimitOk

`func (o *UpdateDashboardBlockRequestConfig) GetEntityLimitOk() (*int32, bool)`

GetEntityLimitOk returns a tuple with the EntityLimit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityLimit

`func (o *UpdateDashboardBlockRequestConfig) SetEntityLimit(v int32)`

SetEntityLimit sets EntityLimit field to given value.

### HasEntityLimit

`func (o *UpdateDashboardBlockRequestConfig) HasEntityLimit() bool`

HasEntityLimit returns a boolean if a field has been set.

### SetEntityLimitNil

`func (o *UpdateDashboardBlockRequestConfig) SetEntityLimitNil(b bool)`

 SetEntityLimitNil sets the value for EntityLimit to be an explicit nil

### UnsetEntityLimit
`func (o *UpdateDashboardBlockRequestConfig) UnsetEntityLimit()`

UnsetEntityLimit ensures that no value is present for EntityLimit, not even an explicit nil
### GetMin

`func (o *UpdateDashboardBlockRequestConfig) GetMin() float32`

GetMin returns the Min field if non-nil, zero value otherwise.

### GetMinOk

`func (o *UpdateDashboardBlockRequestConfig) GetMinOk() (*float32, bool)`

GetMinOk returns a tuple with the Min field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMin

`func (o *UpdateDashboardBlockRequestConfig) SetMin(v float32)`

SetMin sets Min field to given value.

### HasMin

`func (o *UpdateDashboardBlockRequestConfig) HasMin() bool`

HasMin returns a boolean if a field has been set.

### SetMinNil

`func (o *UpdateDashboardBlockRequestConfig) SetMinNil(b bool)`

 SetMinNil sets the value for Min to be an explicit nil

### UnsetMin
`func (o *UpdateDashboardBlockRequestConfig) UnsetMin()`

UnsetMin ensures that no value is present for Min, not even an explicit nil
### GetMax

`func (o *UpdateDashboardBlockRequestConfig) GetMax() float32`

GetMax returns the Max field if non-nil, zero value otherwise.

### GetMaxOk

`func (o *UpdateDashboardBlockRequestConfig) GetMaxOk() (*float32, bool)`

GetMaxOk returns a tuple with the Max field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMax

`func (o *UpdateDashboardBlockRequestConfig) SetMax(v float32)`

SetMax sets Max field to given value.

### HasMax

`func (o *UpdateDashboardBlockRequestConfig) HasMax() bool`

HasMax returns a boolean if a field has been set.

### SetMaxNil

`func (o *UpdateDashboardBlockRequestConfig) SetMaxNil(b bool)`

 SetMaxNil sets the value for Max to be an explicit nil

### UnsetMax
`func (o *UpdateDashboardBlockRequestConfig) UnsetMax()`

UnsetMax ensures that no value is present for Max, not even an explicit nil
### GetUnit

`func (o *UpdateDashboardBlockRequestConfig) GetUnit() string`

GetUnit returns the Unit field if non-nil, zero value otherwise.

### GetUnitOk

`func (o *UpdateDashboardBlockRequestConfig) GetUnitOk() (*string, bool)`

GetUnitOk returns a tuple with the Unit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnit

`func (o *UpdateDashboardBlockRequestConfig) SetUnit(v string)`

SetUnit sets Unit field to given value.

### HasUnit

`func (o *UpdateDashboardBlockRequestConfig) HasUnit() bool`

HasUnit returns a boolean if a field has been set.

### SetUnitNil

`func (o *UpdateDashboardBlockRequestConfig) SetUnitNil(b bool)`

 SetUnitNil sets the value for Unit to be an explicit nil

### UnsetUnit
`func (o *UpdateDashboardBlockRequestConfig) UnsetUnit()`

UnsetUnit ensures that no value is present for Unit, not even an explicit nil
### GetStartColor

`func (o *UpdateDashboardBlockRequestConfig) GetStartColor() string`

GetStartColor returns the StartColor field if non-nil, zero value otherwise.

### GetStartColorOk

`func (o *UpdateDashboardBlockRequestConfig) GetStartColorOk() (*string, bool)`

GetStartColorOk returns a tuple with the StartColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartColor

`func (o *UpdateDashboardBlockRequestConfig) SetStartColor(v string)`

SetStartColor sets StartColor field to given value.

### HasStartColor

`func (o *UpdateDashboardBlockRequestConfig) HasStartColor() bool`

HasStartColor returns a boolean if a field has been set.

### SetStartColorNil

`func (o *UpdateDashboardBlockRequestConfig) SetStartColorNil(b bool)`

 SetStartColorNil sets the value for StartColor to be an explicit nil

### UnsetStartColor
`func (o *UpdateDashboardBlockRequestConfig) UnsetStartColor()`

UnsetStartColor ensures that no value is present for StartColor, not even an explicit nil
### GetMidColor

`func (o *UpdateDashboardBlockRequestConfig) GetMidColor() string`

GetMidColor returns the MidColor field if non-nil, zero value otherwise.

### GetMidColorOk

`func (o *UpdateDashboardBlockRequestConfig) GetMidColorOk() (*string, bool)`

GetMidColorOk returns a tuple with the MidColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMidColor

`func (o *UpdateDashboardBlockRequestConfig) SetMidColor(v string)`

SetMidColor sets MidColor field to given value.

### HasMidColor

`func (o *UpdateDashboardBlockRequestConfig) HasMidColor() bool`

HasMidColor returns a boolean if a field has been set.

### SetMidColorNil

`func (o *UpdateDashboardBlockRequestConfig) SetMidColorNil(b bool)`

 SetMidColorNil sets the value for MidColor to be an explicit nil

### UnsetMidColor
`func (o *UpdateDashboardBlockRequestConfig) UnsetMidColor()`

UnsetMidColor ensures that no value is present for MidColor, not even an explicit nil
### GetEndColor

`func (o *UpdateDashboardBlockRequestConfig) GetEndColor() string`

GetEndColor returns the EndColor field if non-nil, zero value otherwise.

### GetEndColorOk

`func (o *UpdateDashboardBlockRequestConfig) GetEndColorOk() (*string, bool)`

GetEndColorOk returns a tuple with the EndColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndColor

`func (o *UpdateDashboardBlockRequestConfig) SetEndColor(v string)`

SetEndColor sets EndColor field to given value.

### HasEndColor

`func (o *UpdateDashboardBlockRequestConfig) HasEndColor() bool`

HasEndColor returns a boolean if a field has been set.

### SetEndColorNil

`func (o *UpdateDashboardBlockRequestConfig) SetEndColorNil(b bool)`

 SetEndColorNil sets the value for EndColor to be an explicit nil

### UnsetEndColor
`func (o *UpdateDashboardBlockRequestConfig) UnsetEndColor()`

UnsetEndColor ensures that no value is present for EndColor, not even an explicit nil
### GetLimit

`func (o *UpdateDashboardBlockRequestConfig) GetLimit() int32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *UpdateDashboardBlockRequestConfig) GetLimitOk() (*int32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *UpdateDashboardBlockRequestConfig) SetLimit(v int32)`

SetLimit sets Limit field to given value.

### HasLimit

`func (o *UpdateDashboardBlockRequestConfig) HasLimit() bool`

HasLimit returns a boolean if a field has been set.

### SetLimitNil

`func (o *UpdateDashboardBlockRequestConfig) SetLimitNil(b bool)`

 SetLimitNil sets the value for Limit to be an explicit nil

### UnsetLimit
`func (o *UpdateDashboardBlockRequestConfig) UnsetLimit()`

UnsetLimit ensures that no value is present for Limit, not even an explicit nil
### GetSort

`func (o *UpdateDashboardBlockRequestConfig) GetSort() map[string]interface{}`

GetSort returns the Sort field if non-nil, zero value otherwise.

### GetSortOk

`func (o *UpdateDashboardBlockRequestConfig) GetSortOk() (*map[string]interface{}, bool)`

GetSortOk returns a tuple with the Sort field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSort

`func (o *UpdateDashboardBlockRequestConfig) SetSort(v map[string]interface{})`

SetSort sets Sort field to given value.

### HasSort

`func (o *UpdateDashboardBlockRequestConfig) HasSort() bool`

HasSort returns a boolean if a field has been set.

### SetSortNil

`func (o *UpdateDashboardBlockRequestConfig) SetSortNil(b bool)`

 SetSortNil sets the value for Sort to be an explicit nil

### UnsetSort
`func (o *UpdateDashboardBlockRequestConfig) UnsetSort()`

UnsetSort ensures that no value is present for Sort, not even an explicit nil
### GetVisibleAttributes

`func (o *UpdateDashboardBlockRequestConfig) GetVisibleAttributes() []string`

GetVisibleAttributes returns the VisibleAttributes field if non-nil, zero value otherwise.

### GetVisibleAttributesOk

`func (o *UpdateDashboardBlockRequestConfig) GetVisibleAttributesOk() (*[]string, bool)`

GetVisibleAttributesOk returns a tuple with the VisibleAttributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVisibleAttributes

`func (o *UpdateDashboardBlockRequestConfig) SetVisibleAttributes(v []string)`

SetVisibleAttributes sets VisibleAttributes field to given value.

### HasVisibleAttributes

`func (o *UpdateDashboardBlockRequestConfig) HasVisibleAttributes() bool`

HasVisibleAttributes returns a boolean if a field has been set.

### SetVisibleAttributesNil

`func (o *UpdateDashboardBlockRequestConfig) SetVisibleAttributesNil(b bool)`

 SetVisibleAttributesNil sets the value for VisibleAttributes to be an explicit nil

### UnsetVisibleAttributes
`func (o *UpdateDashboardBlockRequestConfig) UnsetVisibleAttributes()`

UnsetVisibleAttributes ensures that no value is present for VisibleAttributes, not even an explicit nil
### GetFilters

`func (o *UpdateDashboardBlockRequestConfig) GetFilters() []map[string]interface{}`

GetFilters returns the Filters field if non-nil, zero value otherwise.

### GetFiltersOk

`func (o *UpdateDashboardBlockRequestConfig) GetFiltersOk() (*[]map[string]interface{}, bool)`

GetFiltersOk returns a tuple with the Filters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilters

`func (o *UpdateDashboardBlockRequestConfig) SetFilters(v []map[string]interface{})`

SetFilters sets Filters field to given value.

### HasFilters

`func (o *UpdateDashboardBlockRequestConfig) HasFilters() bool`

HasFilters returns a boolean if a field has been set.

### SetFiltersNil

`func (o *UpdateDashboardBlockRequestConfig) SetFiltersNil(b bool)`

 SetFiltersNil sets the value for Filters to be an explicit nil

### UnsetFilters
`func (o *UpdateDashboardBlockRequestConfig) UnsetFilters()`

UnsetFilters ensures that no value is present for Filters, not even an explicit nil
### GetX

`func (o *UpdateDashboardBlockRequestConfig) GetX() int32`

GetX returns the X field if non-nil, zero value otherwise.

### GetXOk

`func (o *UpdateDashboardBlockRequestConfig) GetXOk() (*int32, bool)`

GetXOk returns a tuple with the X field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetX

`func (o *UpdateDashboardBlockRequestConfig) SetX(v int32)`

SetX sets X field to given value.

### HasX

`func (o *UpdateDashboardBlockRequestConfig) HasX() bool`

HasX returns a boolean if a field has been set.

### SetXNil

`func (o *UpdateDashboardBlockRequestConfig) SetXNil(b bool)`

 SetXNil sets the value for X to be an explicit nil

### UnsetX
`func (o *UpdateDashboardBlockRequestConfig) UnsetX()`

UnsetX ensures that no value is present for X, not even an explicit nil
### GetY

`func (o *UpdateDashboardBlockRequestConfig) GetY() int32`

GetY returns the Y field if non-nil, zero value otherwise.

### GetYOk

`func (o *UpdateDashboardBlockRequestConfig) GetYOk() (*int32, bool)`

GetYOk returns a tuple with the Y field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetY

`func (o *UpdateDashboardBlockRequestConfig) SetY(v int32)`

SetY sets Y field to given value.

### HasY

`func (o *UpdateDashboardBlockRequestConfig) HasY() bool`

HasY returns a boolean if a field has been set.

### SetYNil

`func (o *UpdateDashboardBlockRequestConfig) SetYNil(b bool)`

 SetYNil sets the value for Y to be an explicit nil

### UnsetY
`func (o *UpdateDashboardBlockRequestConfig) UnsetY()`

UnsetY ensures that no value is present for Y, not even an explicit nil
### GetCols

`func (o *UpdateDashboardBlockRequestConfig) GetCols() int32`

GetCols returns the Cols field if non-nil, zero value otherwise.

### GetColsOk

`func (o *UpdateDashboardBlockRequestConfig) GetColsOk() (*int32, bool)`

GetColsOk returns a tuple with the Cols field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCols

`func (o *UpdateDashboardBlockRequestConfig) SetCols(v int32)`

SetCols sets Cols field to given value.

### HasCols

`func (o *UpdateDashboardBlockRequestConfig) HasCols() bool`

HasCols returns a boolean if a field has been set.

### SetColsNil

`func (o *UpdateDashboardBlockRequestConfig) SetColsNil(b bool)`

 SetColsNil sets the value for Cols to be an explicit nil

### UnsetCols
`func (o *UpdateDashboardBlockRequestConfig) UnsetCols()`

UnsetCols ensures that no value is present for Cols, not even an explicit nil
### GetRows

`func (o *UpdateDashboardBlockRequestConfig) GetRows() int32`

GetRows returns the Rows field if non-nil, zero value otherwise.

### GetRowsOk

`func (o *UpdateDashboardBlockRequestConfig) GetRowsOk() (*int32, bool)`

GetRowsOk returns a tuple with the Rows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRows

`func (o *UpdateDashboardBlockRequestConfig) SetRows(v int32)`

SetRows sets Rows field to given value.

### HasRows

`func (o *UpdateDashboardBlockRequestConfig) HasRows() bool`

HasRows returns a boolean if a field has been set.

### SetRowsNil

`func (o *UpdateDashboardBlockRequestConfig) SetRowsNil(b bool)`

 SetRowsNil sets the value for Rows to be an explicit nil

### UnsetRows
`func (o *UpdateDashboardBlockRequestConfig) UnsetRows()`

UnsetRows ensures that no value is present for Rows, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


