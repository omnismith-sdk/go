# IngestMetricsRequestMetricValuesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | Pointer to **NullableString** | Target metric attribute UUID (provide either attribute_id or attribute_slug) | [optional] 
**AttributeSlug** | Pointer to **NullableString** | Target metric attribute slug (provide either attribute_id or attribute_slug) | [optional] 
**Value** | Pointer to **string** | Numeric observation value formatted as a string | [optional] 
**UpdatedAt** | Pointer to **NullableTime** | Observation timestamp in ISO 8601 or YYYY-MM-DD HH:MM:SS format. Defaults to current UTC time when omitted. | [optional] 

## Methods

### NewIngestMetricsRequestMetricValuesInner

`func NewIngestMetricsRequestMetricValuesInner() *IngestMetricsRequestMetricValuesInner`

NewIngestMetricsRequestMetricValuesInner instantiates a new IngestMetricsRequestMetricValuesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewIngestMetricsRequestMetricValuesInnerWithDefaults

`func NewIngestMetricsRequestMetricValuesInnerWithDefaults() *IngestMetricsRequestMetricValuesInner`

NewIngestMetricsRequestMetricValuesInnerWithDefaults instantiates a new IngestMetricsRequestMetricValuesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeId

`func (o *IngestMetricsRequestMetricValuesInner) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *IngestMetricsRequestMetricValuesInner) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *IngestMetricsRequestMetricValuesInner) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.

### HasAttributeId

`func (o *IngestMetricsRequestMetricValuesInner) HasAttributeId() bool`

HasAttributeId returns a boolean if a field has been set.

### SetAttributeIdNil

`func (o *IngestMetricsRequestMetricValuesInner) SetAttributeIdNil(b bool)`

 SetAttributeIdNil sets the value for AttributeId to be an explicit nil

### UnsetAttributeId
`func (o *IngestMetricsRequestMetricValuesInner) UnsetAttributeId()`

UnsetAttributeId ensures that no value is present for AttributeId, not even an explicit nil
### GetAttributeSlug

`func (o *IngestMetricsRequestMetricValuesInner) GetAttributeSlug() string`

GetAttributeSlug returns the AttributeSlug field if non-nil, zero value otherwise.

### GetAttributeSlugOk

`func (o *IngestMetricsRequestMetricValuesInner) GetAttributeSlugOk() (*string, bool)`

GetAttributeSlugOk returns a tuple with the AttributeSlug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeSlug

`func (o *IngestMetricsRequestMetricValuesInner) SetAttributeSlug(v string)`

SetAttributeSlug sets AttributeSlug field to given value.

### HasAttributeSlug

`func (o *IngestMetricsRequestMetricValuesInner) HasAttributeSlug() bool`

HasAttributeSlug returns a boolean if a field has been set.

### SetAttributeSlugNil

`func (o *IngestMetricsRequestMetricValuesInner) SetAttributeSlugNil(b bool)`

 SetAttributeSlugNil sets the value for AttributeSlug to be an explicit nil

### UnsetAttributeSlug
`func (o *IngestMetricsRequestMetricValuesInner) UnsetAttributeSlug()`

UnsetAttributeSlug ensures that no value is present for AttributeSlug, not even an explicit nil
### GetValue

`func (o *IngestMetricsRequestMetricValuesInner) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *IngestMetricsRequestMetricValuesInner) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *IngestMetricsRequestMetricValuesInner) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *IngestMetricsRequestMetricValuesInner) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *IngestMetricsRequestMetricValuesInner) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *IngestMetricsRequestMetricValuesInner) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *IngestMetricsRequestMetricValuesInner) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *IngestMetricsRequestMetricValuesInner) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.

### SetUpdatedAtNil

`func (o *IngestMetricsRequestMetricValuesInner) SetUpdatedAtNil(b bool)`

 SetUpdatedAtNil sets the value for UpdatedAt to be an explicit nil

### UnsetUpdatedAt
`func (o *IngestMetricsRequestMetricValuesInner) UnsetUpdatedAt()`

UnsetUpdatedAt ensures that no value is present for UpdatedAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


