# GetEntityChart200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Series** | Pointer to [**[]GetEntityChart200ResponseSeriesInner**](GetEntityChart200ResponseSeriesInner.md) | List of aggregated metric series | [optional] 

## Methods

### NewGetEntityChart200Response

`func NewGetEntityChart200Response() *GetEntityChart200Response`

NewGetEntityChart200Response instantiates a new GetEntityChart200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetEntityChart200ResponseWithDefaults

`func NewGetEntityChart200ResponseWithDefaults() *GetEntityChart200Response`

NewGetEntityChart200ResponseWithDefaults instantiates a new GetEntityChart200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSeries

`func (o *GetEntityChart200Response) GetSeries() []GetEntityChart200ResponseSeriesInner`

GetSeries returns the Series field if non-nil, zero value otherwise.

### GetSeriesOk

`func (o *GetEntityChart200Response) GetSeriesOk() (*[]GetEntityChart200ResponseSeriesInner, bool)`

GetSeriesOk returns a tuple with the Series field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSeries

`func (o *GetEntityChart200Response) SetSeries(v []GetEntityChart200ResponseSeriesInner)`

SetSeries sets Series field to given value.

### HasSeries

`func (o *GetEntityChart200Response) HasSeries() bool`

HasSeries returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


