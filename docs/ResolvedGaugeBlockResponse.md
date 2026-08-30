# ResolvedGaugeBlockResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BlockId** | Pointer to **string** | Dashboard block unique identifier | [optional] 
**Title** | Pointer to **string** | Block header title | [optional] 
**Type** | Pointer to **string** | Block type discriminator | [optional] 
**Value** | Pointer to **float32** | Current aggregated metric value | [optional] 
**Min** | Pointer to **float32** | Configured minimum gauge scale bound | [optional] 
**Max** | Pointer to **float32** | Configured maximum gauge scale bound | [optional] 
**Percentage** | Pointer to **float32** | Computed progress percentage within [min, max] bounds | [optional] 

## Methods

### NewResolvedGaugeBlockResponse

`func NewResolvedGaugeBlockResponse() *ResolvedGaugeBlockResponse`

NewResolvedGaugeBlockResponse instantiates a new ResolvedGaugeBlockResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewResolvedGaugeBlockResponseWithDefaults

`func NewResolvedGaugeBlockResponseWithDefaults() *ResolvedGaugeBlockResponse`

NewResolvedGaugeBlockResponseWithDefaults instantiates a new ResolvedGaugeBlockResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBlockId

`func (o *ResolvedGaugeBlockResponse) GetBlockId() string`

GetBlockId returns the BlockId field if non-nil, zero value otherwise.

### GetBlockIdOk

`func (o *ResolvedGaugeBlockResponse) GetBlockIdOk() (*string, bool)`

GetBlockIdOk returns a tuple with the BlockId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlockId

`func (o *ResolvedGaugeBlockResponse) SetBlockId(v string)`

SetBlockId sets BlockId field to given value.

### HasBlockId

`func (o *ResolvedGaugeBlockResponse) HasBlockId() bool`

HasBlockId returns a boolean if a field has been set.

### GetTitle

`func (o *ResolvedGaugeBlockResponse) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ResolvedGaugeBlockResponse) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ResolvedGaugeBlockResponse) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *ResolvedGaugeBlockResponse) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetType

`func (o *ResolvedGaugeBlockResponse) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ResolvedGaugeBlockResponse) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ResolvedGaugeBlockResponse) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *ResolvedGaugeBlockResponse) HasType() bool`

HasType returns a boolean if a field has been set.

### GetValue

`func (o *ResolvedGaugeBlockResponse) GetValue() float32`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *ResolvedGaugeBlockResponse) GetValueOk() (*float32, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *ResolvedGaugeBlockResponse) SetValue(v float32)`

SetValue sets Value field to given value.

### HasValue

`func (o *ResolvedGaugeBlockResponse) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetMin

`func (o *ResolvedGaugeBlockResponse) GetMin() float32`

GetMin returns the Min field if non-nil, zero value otherwise.

### GetMinOk

`func (o *ResolvedGaugeBlockResponse) GetMinOk() (*float32, bool)`

GetMinOk returns a tuple with the Min field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMin

`func (o *ResolvedGaugeBlockResponse) SetMin(v float32)`

SetMin sets Min field to given value.

### HasMin

`func (o *ResolvedGaugeBlockResponse) HasMin() bool`

HasMin returns a boolean if a field has been set.

### GetMax

`func (o *ResolvedGaugeBlockResponse) GetMax() float32`

GetMax returns the Max field if non-nil, zero value otherwise.

### GetMaxOk

`func (o *ResolvedGaugeBlockResponse) GetMaxOk() (*float32, bool)`

GetMaxOk returns a tuple with the Max field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMax

`func (o *ResolvedGaugeBlockResponse) SetMax(v float32)`

SetMax sets Max field to given value.

### HasMax

`func (o *ResolvedGaugeBlockResponse) HasMax() bool`

HasMax returns a boolean if a field has been set.

### GetPercentage

`func (o *ResolvedGaugeBlockResponse) GetPercentage() float32`

GetPercentage returns the Percentage field if non-nil, zero value otherwise.

### GetPercentageOk

`func (o *ResolvedGaugeBlockResponse) GetPercentageOk() (*float32, bool)`

GetPercentageOk returns a tuple with the Percentage field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPercentage

`func (o *ResolvedGaugeBlockResponse) SetPercentage(v float32)`

SetPercentage sets Percentage field to given value.

### HasPercentage

`func (o *ResolvedGaugeBlockResponse) HasPercentage() bool`

HasPercentage returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


