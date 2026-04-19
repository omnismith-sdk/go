# SearchEntities200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | Pointer to [**[]EntityResponse**](EntityResponse.md) |  | [optional] 
**Total** | Pointer to **int32** |  | [optional] 
**Limit** | Pointer to **int32** |  | [optional] 
**Offset** | Pointer to **int32** |  | [optional] 

## Methods

### NewSearchEntities200Response

`func NewSearchEntities200Response() *SearchEntities200Response`

NewSearchEntities200Response instantiates a new SearchEntities200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSearchEntities200ResponseWithDefaults

`func NewSearchEntities200ResponseWithDefaults() *SearchEntities200Response`

NewSearchEntities200ResponseWithDefaults instantiates a new SearchEntities200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *SearchEntities200Response) GetData() []EntityResponse`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *SearchEntities200Response) GetDataOk() (*[]EntityResponse, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *SearchEntities200Response) SetData(v []EntityResponse)`

SetData sets Data field to given value.

### HasData

`func (o *SearchEntities200Response) HasData() bool`

HasData returns a boolean if a field has been set.

### GetTotal

`func (o *SearchEntities200Response) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *SearchEntities200Response) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *SearchEntities200Response) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *SearchEntities200Response) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetLimit

`func (o *SearchEntities200Response) GetLimit() int32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *SearchEntities200Response) GetLimitOk() (*int32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *SearchEntities200Response) SetLimit(v int32)`

SetLimit sets Limit field to given value.

### HasLimit

`func (o *SearchEntities200Response) HasLimit() bool`

HasLimit returns a boolean if a field has been set.

### GetOffset

`func (o *SearchEntities200Response) GetOffset() int32`

GetOffset returns the Offset field if non-nil, zero value otherwise.

### GetOffsetOk

`func (o *SearchEntities200Response) GetOffsetOk() (*int32, bool)`

GetOffsetOk returns a tuple with the Offset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOffset

`func (o *SearchEntities200Response) SetOffset(v int32)`

SetOffset sets Offset field to given value.

### HasOffset

`func (o *SearchEntities200Response) HasOffset() bool`

HasOffset returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


