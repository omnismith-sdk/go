# TierResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**Title** | Pointer to **string** |  | [optional] 
**Description** | Pointer to **string** |  | [optional] 
**PriceCents** | Pointer to **int32** |  | [optional] 
**Currency** | Pointer to **string** |  | [optional] 
**Limits** | Pointer to [**TierResponseLimits**](TierResponseLimits.md) |  | [optional] 
**Features** | Pointer to [**TierResponseFeatures**](TierResponseFeatures.md) |  | [optional] 

## Methods

### NewTierResponse

`func NewTierResponse() *TierResponse`

NewTierResponse instantiates a new TierResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTierResponseWithDefaults

`func NewTierResponseWithDefaults() *TierResponse`

NewTierResponseWithDefaults instantiates a new TierResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *TierResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *TierResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *TierResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *TierResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetTitle

`func (o *TierResponse) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *TierResponse) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *TierResponse) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *TierResponse) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetDescription

`func (o *TierResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *TierResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *TierResponse) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *TierResponse) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetPriceCents

`func (o *TierResponse) GetPriceCents() int32`

GetPriceCents returns the PriceCents field if non-nil, zero value otherwise.

### GetPriceCentsOk

`func (o *TierResponse) GetPriceCentsOk() (*int32, bool)`

GetPriceCentsOk returns a tuple with the PriceCents field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPriceCents

`func (o *TierResponse) SetPriceCents(v int32)`

SetPriceCents sets PriceCents field to given value.

### HasPriceCents

`func (o *TierResponse) HasPriceCents() bool`

HasPriceCents returns a boolean if a field has been set.

### GetCurrency

`func (o *TierResponse) GetCurrency() string`

GetCurrency returns the Currency field if non-nil, zero value otherwise.

### GetCurrencyOk

`func (o *TierResponse) GetCurrencyOk() (*string, bool)`

GetCurrencyOk returns a tuple with the Currency field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCurrency

`func (o *TierResponse) SetCurrency(v string)`

SetCurrency sets Currency field to given value.

### HasCurrency

`func (o *TierResponse) HasCurrency() bool`

HasCurrency returns a boolean if a field has been set.

### GetLimits

`func (o *TierResponse) GetLimits() TierResponseLimits`

GetLimits returns the Limits field if non-nil, zero value otherwise.

### GetLimitsOk

`func (o *TierResponse) GetLimitsOk() (*TierResponseLimits, bool)`

GetLimitsOk returns a tuple with the Limits field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLimits

`func (o *TierResponse) SetLimits(v TierResponseLimits)`

SetLimits sets Limits field to given value.

### HasLimits

`func (o *TierResponse) HasLimits() bool`

HasLimits returns a boolean if a field has been set.

### GetFeatures

`func (o *TierResponse) GetFeatures() TierResponseFeatures`

GetFeatures returns the Features field if non-nil, zero value otherwise.

### GetFeaturesOk

`func (o *TierResponse) GetFeaturesOk() (*TierResponseFeatures, bool)`

GetFeaturesOk returns a tuple with the Features field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFeatures

`func (o *TierResponse) SetFeatures(v TierResponseFeatures)`

SetFeatures sets Features field to given value.

### HasFeatures

`func (o *TierResponse) HasFeatures() bool`

HasFeatures returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


