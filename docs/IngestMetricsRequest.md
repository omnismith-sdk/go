# IngestMetricsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**MetricValues** | Pointer to [**[]IngestMetricsRequestMetricValuesInner**](IngestMetricsRequestMetricValuesInner.md) | List of metric attribute observations to ingest | [optional] 

## Methods

### NewIngestMetricsRequest

`func NewIngestMetricsRequest() *IngestMetricsRequest`

NewIngestMetricsRequest instantiates a new IngestMetricsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewIngestMetricsRequestWithDefaults

`func NewIngestMetricsRequestWithDefaults() *IngestMetricsRequest`

NewIngestMetricsRequestWithDefaults instantiates a new IngestMetricsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMetricValues

`func (o *IngestMetricsRequest) GetMetricValues() []IngestMetricsRequestMetricValuesInner`

GetMetricValues returns the MetricValues field if non-nil, zero value otherwise.

### GetMetricValuesOk

`func (o *IngestMetricsRequest) GetMetricValuesOk() (*[]IngestMetricsRequestMetricValuesInner, bool)`

GetMetricValuesOk returns a tuple with the MetricValues field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetricValues

`func (o *IngestMetricsRequest) SetMetricValues(v []IngestMetricsRequestMetricValuesInner)`

SetMetricValues sets MetricValues field to given value.

### HasMetricValues

`func (o *IngestMetricsRequest) HasMetricValues() bool`

HasMetricValues returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


