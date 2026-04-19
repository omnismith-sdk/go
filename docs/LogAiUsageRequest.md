# LogAiUsageRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CreditsDeducted** | **int32** | Amount of credits to deduct | 
**Model** | Pointer to **string** | Model used | [optional] 
**InputTokens** | Pointer to **int32** | Input tokens | [optional] 
**OutputTokens** | Pointer to **int32** | Output tokens | [optional] 

## Methods

### NewLogAiUsageRequest

`func NewLogAiUsageRequest(creditsDeducted int32, ) *LogAiUsageRequest`

NewLogAiUsageRequest instantiates a new LogAiUsageRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewLogAiUsageRequestWithDefaults

`func NewLogAiUsageRequestWithDefaults() *LogAiUsageRequest`

NewLogAiUsageRequestWithDefaults instantiates a new LogAiUsageRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCreditsDeducted

`func (o *LogAiUsageRequest) GetCreditsDeducted() int32`

GetCreditsDeducted returns the CreditsDeducted field if non-nil, zero value otherwise.

### GetCreditsDeductedOk

`func (o *LogAiUsageRequest) GetCreditsDeductedOk() (*int32, bool)`

GetCreditsDeductedOk returns a tuple with the CreditsDeducted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreditsDeducted

`func (o *LogAiUsageRequest) SetCreditsDeducted(v int32)`

SetCreditsDeducted sets CreditsDeducted field to given value.


### GetModel

`func (o *LogAiUsageRequest) GetModel() string`

GetModel returns the Model field if non-nil, zero value otherwise.

### GetModelOk

`func (o *LogAiUsageRequest) GetModelOk() (*string, bool)`

GetModelOk returns a tuple with the Model field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModel

`func (o *LogAiUsageRequest) SetModel(v string)`

SetModel sets Model field to given value.

### HasModel

`func (o *LogAiUsageRequest) HasModel() bool`

HasModel returns a boolean if a field has been set.

### GetInputTokens

`func (o *LogAiUsageRequest) GetInputTokens() int32`

GetInputTokens returns the InputTokens field if non-nil, zero value otherwise.

### GetInputTokensOk

`func (o *LogAiUsageRequest) GetInputTokensOk() (*int32, bool)`

GetInputTokensOk returns a tuple with the InputTokens field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInputTokens

`func (o *LogAiUsageRequest) SetInputTokens(v int32)`

SetInputTokens sets InputTokens field to given value.

### HasInputTokens

`func (o *LogAiUsageRequest) HasInputTokens() bool`

HasInputTokens returns a boolean if a field has been set.

### GetOutputTokens

`func (o *LogAiUsageRequest) GetOutputTokens() int32`

GetOutputTokens returns the OutputTokens field if non-nil, zero value otherwise.

### GetOutputTokensOk

`func (o *LogAiUsageRequest) GetOutputTokensOk() (*int32, bool)`

GetOutputTokensOk returns a tuple with the OutputTokens field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOutputTokens

`func (o *LogAiUsageRequest) SetOutputTokens(v int32)`

SetOutputTokens sets OutputTokens field to given value.

### HasOutputTokens

`func (o *LogAiUsageRequest) HasOutputTokens() bool`

HasOutputTokens returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


