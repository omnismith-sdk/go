# BiTimeSeriesResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | Pointer to [**[]BiTimeSeriesRow**](BiTimeSeriesRow.md) | List of flat time-bucketed metric observations | [optional] 

## Methods

### NewBiTimeSeriesResponse

`func NewBiTimeSeriesResponse() *BiTimeSeriesResponse`

NewBiTimeSeriesResponse instantiates a new BiTimeSeriesResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBiTimeSeriesResponseWithDefaults

`func NewBiTimeSeriesResponseWithDefaults() *BiTimeSeriesResponse`

NewBiTimeSeriesResponseWithDefaults instantiates a new BiTimeSeriesResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *BiTimeSeriesResponse) GetData() []BiTimeSeriesRow`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *BiTimeSeriesResponse) GetDataOk() (*[]BiTimeSeriesRow, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *BiTimeSeriesResponse) SetData(v []BiTimeSeriesRow)`

SetData sets Data field to given value.

### HasData

`func (o *BiTimeSeriesResponse) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


