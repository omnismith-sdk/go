# ScopeAccessInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | **string** |  | 
**Conditions** | [**[]ScopeConditionInput**](ScopeConditionInput.md) |  | 

## Methods

### NewScopeAccessInput

`func NewScopeAccessInput(templateId string, conditions []ScopeConditionInput, ) *ScopeAccessInput`

NewScopeAccessInput instantiates a new ScopeAccessInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewScopeAccessInputWithDefaults

`func NewScopeAccessInputWithDefaults() *ScopeAccessInput`

NewScopeAccessInputWithDefaults instantiates a new ScopeAccessInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *ScopeAccessInput) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *ScopeAccessInput) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *ScopeAccessInput) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.


### GetConditions

`func (o *ScopeAccessInput) GetConditions() []ScopeConditionInput`

GetConditions returns the Conditions field if non-nil, zero value otherwise.

### GetConditionsOk

`func (o *ScopeAccessInput) GetConditionsOk() (*[]ScopeConditionInput, bool)`

GetConditionsOk returns a tuple with the Conditions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConditions

`func (o *ScopeAccessInput) SetConditions(v []ScopeConditionInput)`

SetConditions sets Conditions field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


