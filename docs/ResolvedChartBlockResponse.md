# ResolvedChartBlockResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BlockId** | Pointer to **string** | Dashboard block unique identifier | [optional] 
**Title** | Pointer to **string** | Block header title | [optional] 
**Type** | Pointer to **string** | Block type discriminator | [optional] 
**BucketWidth** | Pointer to **string** | Time-bucket aggregation interval applied to telemetry metrics | [optional] 
**Series** | Pointer to [**[]ResolvedChartBlockResponseSeriesInner**](ResolvedChartBlockResponseSeriesInner.md) | Time-series data grouped per entity | [optional] 

## Methods

### NewResolvedChartBlockResponse

`func NewResolvedChartBlockResponse() *ResolvedChartBlockResponse`

NewResolvedChartBlockResponse instantiates a new ResolvedChartBlockResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResolvedChartBlockResponseWithDefaults

`func NewResolvedChartBlockResponseWithDefaults() *ResolvedChartBlockResponse`

NewResolvedChartBlockResponseWithDefaults instantiates a new ResolvedChartBlockResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBlockId

`func (o *ResolvedChartBlockResponse) GetBlockId() string`

GetBlockId returns the BlockId field if non-nil, zero value otherwise.

### GetBlockIdOk

`func (o *ResolvedChartBlockResponse) GetBlockIdOk() (*string, bool)`

GetBlockIdOk returns a tuple with the BlockId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlockId

`func (o *ResolvedChartBlockResponse) SetBlockId(v string)`

SetBlockId sets BlockId field to given value.

### HasBlockId

`func (o *ResolvedChartBlockResponse) HasBlockId() bool`

HasBlockId returns a boolean if a field has been set.

### GetTitle

`func (o *ResolvedChartBlockResponse) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ResolvedChartBlockResponse) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ResolvedChartBlockResponse) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ResolvedChartBlockResponse) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetType

`func (o *ResolvedChartBlockResponse) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ResolvedChartBlockResponse) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ResolvedChartBlockResponse) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ResolvedChartBlockResponse) HasType() bool`

HasType returns a boolean if a field has been set.

### GetBucketWidth

`func (o *ResolvedChartBlockResponse) GetBucketWidth() string`

GetBucketWidth returns the BucketWidth field if non-nil, zero value otherwise.

### GetBucketWidthOk

`func (o *ResolvedChartBlockResponse) GetBucketWidthOk() (*string, bool)`

GetBucketWidthOk returns a tuple with the BucketWidth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBucketWidth

`func (o *ResolvedChartBlockResponse) SetBucketWidth(v string)`

SetBucketWidth sets BucketWidth field to given value.

### HasBucketWidth

`func (o *ResolvedChartBlockResponse) HasBucketWidth() bool`

HasBucketWidth returns a boolean if a field has been set.

### GetSeries

`func (o *ResolvedChartBlockResponse) GetSeries() []ResolvedChartBlockResponseSeriesInner`

GetSeries returns the Series field if non-nil, zero value otherwise.

### GetSeriesOk

`func (o *ResolvedChartBlockResponse) GetSeriesOk() (*[]ResolvedChartBlockResponseSeriesInner, bool)`

GetSeriesOk returns a tuple with the Series field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeries

`func (o *ResolvedChartBlockResponse) SetSeries(v []ResolvedChartBlockResponseSeriesInner)`

SetSeries sets Series field to given value.

### HasSeries

`func (o *ResolvedChartBlockResponse) HasSeries() bool`

HasSeries returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


