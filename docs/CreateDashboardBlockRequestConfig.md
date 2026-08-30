# CreateDashboardBlockRequestConfig

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | Pointer to **string** | UUID of the entity template serving as the data source (required for all block types). | [optional] 
**MetricAttributeId** | Pointer to **NullableString** | UUID of the metric attribute to aggregate/plot (required for chart and metric gauge blocks). | [optional] 
**TimeWindow** | Pointer to **NullableInt32** | Time range query window in seconds for historical telemetry. CRITICAL for chart and time-series gauge blocks to query Entity Log data points. Presets: 3600 (1 hour), 10800 (3 hours), 21600 (6 hours), 43200 (12 hours), 86400 (24 hours / 1 day, recommended default), 604800 (7 days / 1 week), 2592000 (30 days / 1 month). | [optional] [default to 86400]
**BucketWidth** | Pointer to **string** | Time bucket interval for chart data aggregation. Standard values: \&quot;1 min\&quot;, \&quot;5 min\&quot;, \&quot;10 min\&quot;, \&quot;15 min\&quot;, \&quot;1 hour\&quot; (default), \&quot;6 hours\&quot;, \&quot;12 hours\&quot;, \&quot;1 day\&quot;, \&quot;1 week\&quot;, \&quot;1 month\&quot;. | [optional] [default to "1 hour"]
**Aggregate** | Pointer to **string** | Aggregation function for telemetry metric points: \&quot;avg\&quot; (default for gauge/chart), \&quot;sum\&quot;, \&quot;min\&quot;, \&quot;max\&quot;, \&quot;first\&quot;, \&quot;last\&quot;, \&quot;count\&quot;. | [optional] [default to "avg"]
**EntityLimit** | Pointer to **int32** | Maximum number of entity series lines to plot concurrently in chart blocks (1-50, default: 10). | [optional] [default to 10]
**Min** | Pointer to **float32** | Minimum scale value for gauge blocks (default: 0). | [optional] [default to 0]
**Max** | Pointer to **float32** | Maximum scale value for gauge blocks (default: 100). | [optional] [default to 100]
**Unit** | Pointer to **NullableString** | Optional unit suffix for gauge blocks (e.g. \&quot;%\&quot;, \&quot;°C\&quot;, \&quot;MB/s\&quot;, \&quot;req/s\&quot;). | [optional] 
**StartColor** | Pointer to **NullableString** | Start gradient hex color for gauge blocks (e.g. \&quot;#3b82f6\&quot;). | [optional] 
**MidColor** | Pointer to **NullableString** | Middle gradient hex color for gauge blocks (optional). | [optional] 
**EndColor** | Pointer to **NullableString** | End gradient hex color for gauge blocks (e.g. \&quot;#06b6d4\&quot;). | [optional] 
**Limit** | Pointer to **int32** | Maximum number of rows to return for list table blocks (default: 10). | [optional] [default to 10]
**Sort** | Pointer to **map[string]interface{}** | Sort configuration object for list table blocks (e.g. {\&quot;created_at\&quot;: \&quot;desc\&quot;}). | [optional] 
**VisibleAttributes** | Pointer to **[]string** | Ordered list of attribute UUIDs (or \&quot;created_at\&quot;, \&quot;updated_at\&quot;) to display as columns in list table blocks. | [optional] 
**Filters** | Pointer to [**[]CreateDashboardBlockRequestConfigFiltersInner**](CreateDashboardBlockRequestConfigFiltersInner.md) | Optional entity filtering conditions applied to block data. | [optional] 
**X** | Pointer to **int32** | Horizontal grid column position (0 to 11 on the 12-column grid canvas). | [optional] [default to 0]
**Y** | Pointer to **int32** | Vertical grid row position (0 to N, 0-indexed). | [optional] [default to 0]
**Cols** | Pointer to **int32** | Block width in columns on the 12-column grid canvas (1 to 12). Guidelines: 12 &#x3D; full-width (chart/list), 6 &#x3D; half-width (chart/gauge, 2 per row), 4 &#x3D; one-third width (stat/gauge, 3 per row), 3 &#x3D; one-fourth width (stat, 4 per row). Sum of cols in a row should equal 12 for edge-to-edge alignment. | [optional] 
**Rows** | Pointer to **int32** | Block height in grid rows (1 to N). Guidelines: 2 &#x3D; KPI stat / radial gauge, 3-4 &#x3D; time-series chart, 4-5 &#x3D; list table. | [optional] 

## Methods

### NewCreateDashboardBlockRequestConfig

`func NewCreateDashboardBlockRequestConfig() *CreateDashboardBlockRequestConfig`

NewCreateDashboardBlockRequestConfig instantiates a new CreateDashboardBlockRequestConfig object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateDashboardBlockRequestConfigWithDefaults

`func NewCreateDashboardBlockRequestConfigWithDefaults() *CreateDashboardBlockRequestConfig`

NewCreateDashboardBlockRequestConfigWithDefaults instantiates a new CreateDashboardBlockRequestConfig object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *CreateDashboardBlockRequestConfig) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *CreateDashboardBlockRequestConfig) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *CreateDashboardBlockRequestConfig) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *CreateDashboardBlockRequestConfig) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetMetricAttributeId

`func (o *CreateDashboardBlockRequestConfig) GetMetricAttributeId() string`

GetMetricAttributeId returns the MetricAttributeId field if non-nil, zero value otherwise.

### GetMetricAttributeIdOk

`func (o *CreateDashboardBlockRequestConfig) GetMetricAttributeIdOk() (*string, bool)`

GetMetricAttributeIdOk returns a tuple with the MetricAttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetricAttributeId

`func (o *CreateDashboardBlockRequestConfig) SetMetricAttributeId(v string)`

SetMetricAttributeId sets MetricAttributeId field to given value.

### HasMetricAttributeId

`func (o *CreateDashboardBlockRequestConfig) HasMetricAttributeId() bool`

HasMetricAttributeId returns a boolean if a field has been set.

### SetMetricAttributeIdNil

`func (o *CreateDashboardBlockRequestConfig) SetMetricAttributeIdNil(b bool)`

 SetMetricAttributeIdNil sets the value for MetricAttributeId to be an explicit nil

### UnsetMetricAttributeId
`func (o *CreateDashboardBlockRequestConfig) UnsetMetricAttributeId()`

UnsetMetricAttributeId ensures that no value is present for MetricAttributeId, not even an explicit nil
### GetTimeWindow

`func (o *CreateDashboardBlockRequestConfig) GetTimeWindow() int32`

GetTimeWindow returns the TimeWindow field if non-nil, zero value otherwise.

### GetTimeWindowOk

`func (o *CreateDashboardBlockRequestConfig) GetTimeWindowOk() (*int32, bool)`

GetTimeWindowOk returns a tuple with the TimeWindow field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimeWindow

`func (o *CreateDashboardBlockRequestConfig) SetTimeWindow(v int32)`

SetTimeWindow sets TimeWindow field to given value.

### HasTimeWindow

`func (o *CreateDashboardBlockRequestConfig) HasTimeWindow() bool`

HasTimeWindow returns a boolean if a field has been set.

### SetTimeWindowNil

`func (o *CreateDashboardBlockRequestConfig) SetTimeWindowNil(b bool)`

 SetTimeWindowNil sets the value for TimeWindow to be an explicit nil

### UnsetTimeWindow
`func (o *CreateDashboardBlockRequestConfig) UnsetTimeWindow()`

UnsetTimeWindow ensures that no value is present for TimeWindow, not even an explicit nil
### GetBucketWidth

`func (o *CreateDashboardBlockRequestConfig) GetBucketWidth() string`

GetBucketWidth returns the BucketWidth field if non-nil, zero value otherwise.

### GetBucketWidthOk

`func (o *CreateDashboardBlockRequestConfig) GetBucketWidthOk() (*string, bool)`

GetBucketWidthOk returns a tuple with the BucketWidth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBucketWidth

`func (o *CreateDashboardBlockRequestConfig) SetBucketWidth(v string)`

SetBucketWidth sets BucketWidth field to given value.

### HasBucketWidth

`func (o *CreateDashboardBlockRequestConfig) HasBucketWidth() bool`

HasBucketWidth returns a boolean if a field has been set.

### GetAggregate

`func (o *CreateDashboardBlockRequestConfig) GetAggregate() string`

GetAggregate returns the Aggregate field if non-nil, zero value otherwise.

### GetAggregateOk

`func (o *CreateDashboardBlockRequestConfig) GetAggregateOk() (*string, bool)`

GetAggregateOk returns a tuple with the Aggregate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAggregate

`func (o *CreateDashboardBlockRequestConfig) SetAggregate(v string)`

SetAggregate sets Aggregate field to given value.

### HasAggregate

`func (o *CreateDashboardBlockRequestConfig) HasAggregate() bool`

HasAggregate returns a boolean if a field has been set.

### GetEntityLimit

`func (o *CreateDashboardBlockRequestConfig) GetEntityLimit() int32`

GetEntityLimit returns the EntityLimit field if non-nil, zero value otherwise.

### GetEntityLimitOk

`func (o *CreateDashboardBlockRequestConfig) GetEntityLimitOk() (*int32, bool)`

GetEntityLimitOk returns a tuple with the EntityLimit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityLimit

`func (o *CreateDashboardBlockRequestConfig) SetEntityLimit(v int32)`

SetEntityLimit sets EntityLimit field to given value.

### HasEntityLimit

`func (o *CreateDashboardBlockRequestConfig) HasEntityLimit() bool`

HasEntityLimit returns a boolean if a field has been set.

### GetMin

`func (o *CreateDashboardBlockRequestConfig) GetMin() float32`

GetMin returns the Min field if non-nil, zero value otherwise.

### GetMinOk

`func (o *CreateDashboardBlockRequestConfig) GetMinOk() (*float32, bool)`

GetMinOk returns a tuple with the Min field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMin

`func (o *CreateDashboardBlockRequestConfig) SetMin(v float32)`

SetMin sets Min field to given value.

### HasMin

`func (o *CreateDashboardBlockRequestConfig) HasMin() bool`

HasMin returns a boolean if a field has been set.

### GetMax

`func (o *CreateDashboardBlockRequestConfig) GetMax() float32`

GetMax returns the Max field if non-nil, zero value otherwise.

### GetMaxOk

`func (o *CreateDashboardBlockRequestConfig) GetMaxOk() (*float32, bool)`

GetMaxOk returns a tuple with the Max field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMax

`func (o *CreateDashboardBlockRequestConfig) SetMax(v float32)`

SetMax sets Max field to given value.

### HasMax

`func (o *CreateDashboardBlockRequestConfig) HasMax() bool`

HasMax returns a boolean if a field has been set.

### GetUnit

`func (o *CreateDashboardBlockRequestConfig) GetUnit() string`

GetUnit returns the Unit field if non-nil, zero value otherwise.

### GetUnitOk

`func (o *CreateDashboardBlockRequestConfig) GetUnitOk() (*string, bool)`

GetUnitOk returns a tuple with the Unit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnit

`func (o *CreateDashboardBlockRequestConfig) SetUnit(v string)`

SetUnit sets Unit field to given value.

### HasUnit

`func (o *CreateDashboardBlockRequestConfig) HasUnit() bool`

HasUnit returns a boolean if a field has been set.

### SetUnitNil

`func (o *CreateDashboardBlockRequestConfig) SetUnitNil(b bool)`

 SetUnitNil sets the value for Unit to be an explicit nil

### UnsetUnit
`func (o *CreateDashboardBlockRequestConfig) UnsetUnit()`

UnsetUnit ensures that no value is present for Unit, not even an explicit nil
### GetStartColor

`func (o *CreateDashboardBlockRequestConfig) GetStartColor() string`

GetStartColor returns the StartColor field if non-nil, zero value otherwise.

### GetStartColorOk

`func (o *CreateDashboardBlockRequestConfig) GetStartColorOk() (*string, bool)`

GetStartColorOk returns a tuple with the StartColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartColor

`func (o *CreateDashboardBlockRequestConfig) SetStartColor(v string)`

SetStartColor sets StartColor field to given value.

### HasStartColor

`func (o *CreateDashboardBlockRequestConfig) HasStartColor() bool`

HasStartColor returns a boolean if a field has been set.

### SetStartColorNil

`func (o *CreateDashboardBlockRequestConfig) SetStartColorNil(b bool)`

 SetStartColorNil sets the value for StartColor to be an explicit nil

### UnsetStartColor
`func (o *CreateDashboardBlockRequestConfig) UnsetStartColor()`

UnsetStartColor ensures that no value is present for StartColor, not even an explicit nil
### GetMidColor

`func (o *CreateDashboardBlockRequestConfig) GetMidColor() string`

GetMidColor returns the MidColor field if non-nil, zero value otherwise.

### GetMidColorOk

`func (o *CreateDashboardBlockRequestConfig) GetMidColorOk() (*string, bool)`

GetMidColorOk returns a tuple with the MidColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMidColor

`func (o *CreateDashboardBlockRequestConfig) SetMidColor(v string)`

SetMidColor sets MidColor field to given value.

### HasMidColor

`func (o *CreateDashboardBlockRequestConfig) HasMidColor() bool`

HasMidColor returns a boolean if a field has been set.

### SetMidColorNil

`func (o *CreateDashboardBlockRequestConfig) SetMidColorNil(b bool)`

 SetMidColorNil sets the value for MidColor to be an explicit nil

### UnsetMidColor
`func (o *CreateDashboardBlockRequestConfig) UnsetMidColor()`

UnsetMidColor ensures that no value is present for MidColor, not even an explicit nil
### GetEndColor

`func (o *CreateDashboardBlockRequestConfig) GetEndColor() string`

GetEndColor returns the EndColor field if non-nil, zero value otherwise.

### GetEndColorOk

`func (o *CreateDashboardBlockRequestConfig) GetEndColorOk() (*string, bool)`

GetEndColorOk returns a tuple with the EndColor field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndColor

`func (o *CreateDashboardBlockRequestConfig) SetEndColor(v string)`

SetEndColor sets EndColor field to given value.

### HasEndColor

`func (o *CreateDashboardBlockRequestConfig) HasEndColor() bool`

HasEndColor returns a boolean if a field has been set.

### SetEndColorNil

`func (o *CreateDashboardBlockRequestConfig) SetEndColorNil(b bool)`

 SetEndColorNil sets the value for EndColor to be an explicit nil

### UnsetEndColor
`func (o *CreateDashboardBlockRequestConfig) UnsetEndColor()`

UnsetEndColor ensures that no value is present for EndColor, not even an explicit nil
### GetLimit

`func (o *CreateDashboardBlockRequestConfig) GetLimit() int32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *CreateDashboardBlockRequestConfig) GetLimitOk() (*int32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *CreateDashboardBlockRequestConfig) SetLimit(v int32)`

SetLimit sets Limit field to given value.

### HasLimit

`func (o *CreateDashboardBlockRequestConfig) HasLimit() bool`

HasLimit returns a boolean if a field has been set.

### GetSort

`func (o *CreateDashboardBlockRequestConfig) GetSort() map[string]interface{}`

GetSort returns the Sort field if non-nil, zero value otherwise.

### GetSortOk

`func (o *CreateDashboardBlockRequestConfig) GetSortOk() (*map[string]interface{}, bool)`

GetSortOk returns a tuple with the Sort field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSort

`func (o *CreateDashboardBlockRequestConfig) SetSort(v map[string]interface{})`

SetSort sets Sort field to given value.

### HasSort

`func (o *CreateDashboardBlockRequestConfig) HasSort() bool`

HasSort returns a boolean if a field has been set.

### GetVisibleAttributes

`func (o *CreateDashboardBlockRequestConfig) GetVisibleAttributes() []string`

GetVisibleAttributes returns the VisibleAttributes field if non-nil, zero value otherwise.

### GetVisibleAttributesOk

`func (o *CreateDashboardBlockRequestConfig) GetVisibleAttributesOk() (*[]string, bool)`

GetVisibleAttributesOk returns a tuple with the VisibleAttributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVisibleAttributes

`func (o *CreateDashboardBlockRequestConfig) SetVisibleAttributes(v []string)`

SetVisibleAttributes sets VisibleAttributes field to given value.

### HasVisibleAttributes

`func (o *CreateDashboardBlockRequestConfig) HasVisibleAttributes() bool`

HasVisibleAttributes returns a boolean if a field has been set.

### GetFilters

`func (o *CreateDashboardBlockRequestConfig) GetFilters() []CreateDashboardBlockRequestConfigFiltersInner`

GetFilters returns the Filters field if non-nil, zero value otherwise.

### GetFiltersOk

`func (o *CreateDashboardBlockRequestConfig) GetFiltersOk() (*[]CreateDashboardBlockRequestConfigFiltersInner, bool)`

GetFiltersOk returns a tuple with the Filters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilters

`func (o *CreateDashboardBlockRequestConfig) SetFilters(v []CreateDashboardBlockRequestConfigFiltersInner)`

SetFilters sets Filters field to given value.

### HasFilters

`func (o *CreateDashboardBlockRequestConfig) HasFilters() bool`

HasFilters returns a boolean if a field has been set.

### GetX

`func (o *CreateDashboardBlockRequestConfig) GetX() int32`

GetX returns the X field if non-nil, zero value otherwise.

### GetXOk

`func (o *CreateDashboardBlockRequestConfig) GetXOk() (*int32, bool)`

GetXOk returns a tuple with the X field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetX

`func (o *CreateDashboardBlockRequestConfig) SetX(v int32)`

SetX sets X field to given value.

### HasX

`func (o *CreateDashboardBlockRequestConfig) HasX() bool`

HasX returns a boolean if a field has been set.

### GetY

`func (o *CreateDashboardBlockRequestConfig) GetY() int32`

GetY returns the Y field if non-nil, zero value otherwise.

### GetYOk

`func (o *CreateDashboardBlockRequestConfig) GetYOk() (*int32, bool)`

GetYOk returns a tuple with the Y field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetY

`func (o *CreateDashboardBlockRequestConfig) SetY(v int32)`

SetY sets Y field to given value.

### HasY

`func (o *CreateDashboardBlockRequestConfig) HasY() bool`

HasY returns a boolean if a field has been set.

### GetCols

`func (o *CreateDashboardBlockRequestConfig) GetCols() int32`

GetCols returns the Cols field if non-nil, zero value otherwise.

### GetColsOk

`func (o *CreateDashboardBlockRequestConfig) GetColsOk() (*int32, bool)`

GetColsOk returns a tuple with the Cols field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCols

`func (o *CreateDashboardBlockRequestConfig) SetCols(v int32)`

SetCols sets Cols field to given value.

### HasCols

`func (o *CreateDashboardBlockRequestConfig) HasCols() bool`

HasCols returns a boolean if a field has been set.

### GetRows

`func (o *CreateDashboardBlockRequestConfig) GetRows() int32`

GetRows returns the Rows field if non-nil, zero value otherwise.

### GetRowsOk

`func (o *CreateDashboardBlockRequestConfig) GetRowsOk() (*int32, bool)`

GetRowsOk returns a tuple with the Rows field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRows

`func (o *CreateDashboardBlockRequestConfig) SetRows(v int32)`

SetRows sets Rows field to given value.

### HasRows

`func (o *CreateDashboardBlockRequestConfig) HasRows() bool`

HasRows returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


