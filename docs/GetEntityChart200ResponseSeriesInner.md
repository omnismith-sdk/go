# GetEntityChart200ResponseSeriesInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | Pointer to **string** | Metric attribute UUID | [optional] 
**Data** | Pointer to [**[]GetEntityChart200ResponseSeriesInnerDataInner**](GetEntityChart200ResponseSeriesInnerDataInner.md) | Chronological time-series data points | [optional] 

## Methods

### NewGetEntityChart200ResponseSeriesInner

`func NewGetEntityChart200ResponseSeriesInner() *GetEntityChart200ResponseSeriesInner`

NewGetEntityChart200ResponseSeriesInner instantiates a new GetEntityChart200ResponseSeriesInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetEntityChart200ResponseSeriesInnerWithDefaults

`func NewGetEntityChart200ResponseSeriesInnerWithDefaults() *GetEntityChart200ResponseSeriesInner`

NewGetEntityChart200ResponseSeriesInnerWithDefaults instantiates a new GetEntityChart200ResponseSeriesInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeId

`func (o *GetEntityChart200ResponseSeriesInner) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *GetEntityChart200ResponseSeriesInner) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *GetEntityChart200ResponseSeriesInner) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.

### HasAttributeId

`func (o *GetEntityChart200ResponseSeriesInner) HasAttributeId() bool`

HasAttributeId returns a boolean if a field has been set.

### GetData

`func (o *GetEntityChart200ResponseSeriesInner) GetData() []GetEntityChart200ResponseSeriesInnerDataInner`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *GetEntityChart200ResponseSeriesInner) GetDataOk() (*[]GetEntityChart200ResponseSeriesInnerDataInner, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *GetEntityChart200ResponseSeriesInner) SetData(v []GetEntityChart200ResponseSeriesInnerDataInner)`

SetData sets Data field to given value.

### HasData

`func (o *GetEntityChart200ResponseSeriesInner) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


