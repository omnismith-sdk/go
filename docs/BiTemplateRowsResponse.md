# BiTemplateRowsResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Columns** | Pointer to [**[]BiSchemaField**](BiSchemaField.md) | Column schema definitions for the tabular dataset | [optional] 
**Data** | Pointer to **[]map[string]interface{}** | Array of flat row objects where keys match column_name | [optional] 
**Total** | Pointer to **int32** | Total row count matching the query filters | [optional] 
**Limit** | Pointer to **int32** | Limit applied to the row set | [optional] 
**Offset** | Pointer to **int32** | Offset applied to the row set | [optional] 

## Methods

### NewBiTemplateRowsResponse

`func NewBiTemplateRowsResponse() *BiTemplateRowsResponse`

NewBiTemplateRowsResponse instantiates a new BiTemplateRowsResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBiTemplateRowsResponseWithDefaults

`func NewBiTemplateRowsResponseWithDefaults() *BiTemplateRowsResponse`

NewBiTemplateRowsResponseWithDefaults instantiates a new BiTemplateRowsResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetColumns

`func (o *BiTemplateRowsResponse) GetColumns() []BiSchemaField`

GetColumns returns the Columns field if non-nil, zero value otherwise.

### GetColumnsOk

`func (o *BiTemplateRowsResponse) GetColumnsOk() (*[]BiSchemaField, bool)`

GetColumnsOk returns a tuple with the Columns field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColumns

`func (o *BiTemplateRowsResponse) SetColumns(v []BiSchemaField)`

SetColumns sets Columns field to given value.

### HasColumns

`func (o *BiTemplateRowsResponse) HasColumns() bool`

HasColumns returns a boolean if a field has been set.

### GetData

`func (o *BiTemplateRowsResponse) GetData() []map[string]interface{}`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *BiTemplateRowsResponse) GetDataOk() (*[]map[string]interface{}, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *BiTemplateRowsResponse) SetData(v []map[string]interface{})`

SetData sets Data field to given value.

### HasData

`func (o *BiTemplateRowsResponse) HasData() bool`

HasData returns a boolean if a field has been set.

### GetTotal

`func (o *BiTemplateRowsResponse) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *BiTemplateRowsResponse) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *BiTemplateRowsResponse) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *BiTemplateRowsResponse) HasTotal() bool`

HasTotal returns a boolean if a field has been set.

### GetLimit

`func (o *BiTemplateRowsResponse) GetLimit() int32`

GetLimit returns the Limit field if non-nil, zero value otherwise.

### GetLimitOk

`func (o *BiTemplateRowsResponse) GetLimitOk() (*int32, bool)`

GetLimitOk returns a tuple with the Limit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimit

`func (o *BiTemplateRowsResponse) SetLimit(v int32)`

SetLimit sets Limit field to given value.

### HasLimit

`func (o *BiTemplateRowsResponse) HasLimit() bool`

HasLimit returns a boolean if a field has been set.

### GetOffset

`func (o *BiTemplateRowsResponse) GetOffset() int32`

GetOffset returns the Offset field if non-nil, zero value otherwise.

### GetOffsetOk

`func (o *BiTemplateRowsResponse) GetOffsetOk() (*int32, bool)`

GetOffsetOk returns a tuple with the Offset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOffset

`func (o *BiTemplateRowsResponse) SetOffset(v int32)`

SetOffset sets Offset field to given value.

### HasOffset

`func (o *BiTemplateRowsResponse) HasOffset() bool`

HasOffset returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


