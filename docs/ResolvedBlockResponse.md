# ResolvedBlockResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BlockId** | Pointer to **string** |  | [optional] 
**Title** | Pointer to **string** |  | [optional] 
**Type** | Pointer to **string** |  | [optional] 
**Count** | Pointer to **int32** |  | [optional] 
**Value** | Pointer to **float32** |  | [optional] 
**Min** | Pointer to **float32** |  | [optional] 
**Max** | Pointer to **float32** |  | [optional] 
**Percentage** | Pointer to **float32** |  | [optional] 
**BucketWidth** | Pointer to **string** |  | [optional] 
**Series** | Pointer to [**[]ResolvedChartBlockResponseSeriesInner**](ResolvedChartBlockResponseSeriesInner.md) |  | [optional] 
**Items** | Pointer to [**[]ResolvedListBlockResponseItemsInner**](ResolvedListBlockResponseItemsInner.md) |  | [optional] 
**TotalCount** | Pointer to **int32** |  | [optional] 

## Methods

### NewResolvedBlockResponse

`func NewResolvedBlockResponse() *ResolvedBlockResponse`

NewResolvedBlockResponse instantiates a new ResolvedBlockResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResolvedBlockResponseWithDefaults

`func NewResolvedBlockResponseWithDefaults() *ResolvedBlockResponse`

NewResolvedBlockResponseWithDefaults instantiates a new ResolvedBlockResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBlockId

`func (o *ResolvedBlockResponse) GetBlockId() string`

GetBlockId returns the BlockId field if non-nil, zero value otherwise.

### GetBlockIdOk

`func (o *ResolvedBlockResponse) GetBlockIdOk() (*string, bool)`

GetBlockIdOk returns a tuple with the BlockId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlockId

`func (o *ResolvedBlockResponse) SetBlockId(v string)`

SetBlockId sets BlockId field to given value.

### HasBlockId

`func (o *ResolvedBlockResponse) HasBlockId() bool`

HasBlockId returns a boolean if a field has been set.

### GetTitle

`func (o *ResolvedBlockResponse) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ResolvedBlockResponse) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ResolvedBlockResponse) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ResolvedBlockResponse) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetType

`func (o *ResolvedBlockResponse) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ResolvedBlockResponse) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ResolvedBlockResponse) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ResolvedBlockResponse) HasType() bool`

HasType returns a boolean if a field has been set.

### GetCount

`func (o *ResolvedBlockResponse) GetCount() int32`

GetCount returns the Count field if non-nil, zero value otherwise.

### GetCountOk

`func (o *ResolvedBlockResponse) GetCountOk() (*int32, bool)`

GetCountOk returns a tuple with the Count field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCount

`func (o *ResolvedBlockResponse) SetCount(v int32)`

SetCount sets Count field to given value.

### HasCount

`func (o *ResolvedBlockResponse) HasCount() bool`

HasCount returns a boolean if a field has been set.

### GetValue

`func (o *ResolvedBlockResponse) GetValue() float32`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *ResolvedBlockResponse) GetValueOk() (*float32, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *ResolvedBlockResponse) SetValue(v float32)`

SetValue sets Value field to given value.

### HasValue

`func (o *ResolvedBlockResponse) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetMin

`func (o *ResolvedBlockResponse) GetMin() float32`

GetMin returns the Min field if non-nil, zero value otherwise.

### GetMinOk

`func (o *ResolvedBlockResponse) GetMinOk() (*float32, bool)`

GetMinOk returns a tuple with the Min field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMin

`func (o *ResolvedBlockResponse) SetMin(v float32)`

SetMin sets Min field to given value.

### HasMin

`func (o *ResolvedBlockResponse) HasMin() bool`

HasMin returns a boolean if a field has been set.

### GetMax

`func (o *ResolvedBlockResponse) GetMax() float32`

GetMax returns the Max field if non-nil, zero value otherwise.

### GetMaxOk

`func (o *ResolvedBlockResponse) GetMaxOk() (*float32, bool)`

GetMaxOk returns a tuple with the Max field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMax

`func (o *ResolvedBlockResponse) SetMax(v float32)`

SetMax sets Max field to given value.

### HasMax

`func (o *ResolvedBlockResponse) HasMax() bool`

HasMax returns a boolean if a field has been set.

### GetPercentage

`func (o *ResolvedBlockResponse) GetPercentage() float32`

GetPercentage returns the Percentage field if non-nil, zero value otherwise.

### GetPercentageOk

`func (o *ResolvedBlockResponse) GetPercentageOk() (*float32, bool)`

GetPercentageOk returns a tuple with the Percentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPercentage

`func (o *ResolvedBlockResponse) SetPercentage(v float32)`

SetPercentage sets Percentage field to given value.

### HasPercentage

`func (o *ResolvedBlockResponse) HasPercentage() bool`

HasPercentage returns a boolean if a field has been set.

### GetBucketWidth

`func (o *ResolvedBlockResponse) GetBucketWidth() string`

GetBucketWidth returns the BucketWidth field if non-nil, zero value otherwise.

### GetBucketWidthOk

`func (o *ResolvedBlockResponse) GetBucketWidthOk() (*string, bool)`

GetBucketWidthOk returns a tuple with the BucketWidth field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBucketWidth

`func (o *ResolvedBlockResponse) SetBucketWidth(v string)`

SetBucketWidth sets BucketWidth field to given value.

### HasBucketWidth

`func (o *ResolvedBlockResponse) HasBucketWidth() bool`

HasBucketWidth returns a boolean if a field has been set.

### GetSeries

`func (o *ResolvedBlockResponse) GetSeries() []ResolvedChartBlockResponseSeriesInner`

GetSeries returns the Series field if non-nil, zero value otherwise.

### GetSeriesOk

`func (o *ResolvedBlockResponse) GetSeriesOk() (*[]ResolvedChartBlockResponseSeriesInner, bool)`

GetSeriesOk returns a tuple with the Series field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeries

`func (o *ResolvedBlockResponse) SetSeries(v []ResolvedChartBlockResponseSeriesInner)`

SetSeries sets Series field to given value.

### HasSeries

`func (o *ResolvedBlockResponse) HasSeries() bool`

HasSeries returns a boolean if a field has been set.

### GetItems

`func (o *ResolvedBlockResponse) GetItems() []ResolvedListBlockResponseItemsInner`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *ResolvedBlockResponse) GetItemsOk() (*[]ResolvedListBlockResponseItemsInner, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *ResolvedBlockResponse) SetItems(v []ResolvedListBlockResponseItemsInner)`

SetItems sets Items field to given value.

### HasItems

`func (o *ResolvedBlockResponse) HasItems() bool`

HasItems returns a boolean if a field has been set.

### GetTotalCount

`func (o *ResolvedBlockResponse) GetTotalCount() int32`

GetTotalCount returns the TotalCount field if non-nil, zero value otherwise.

### GetTotalCountOk

`func (o *ResolvedBlockResponse) GetTotalCountOk() (*int32, bool)`

GetTotalCountOk returns a tuple with the TotalCount field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotalCount

`func (o *ResolvedBlockResponse) SetTotalCount(v int32)`

SetTotalCount sets TotalCount field to given value.

### HasTotalCount

`func (o *ResolvedBlockResponse) HasTotalCount() bool`

HasTotalCount returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


