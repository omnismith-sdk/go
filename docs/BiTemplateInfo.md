# BiTemplateInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | Pointer to **string** | Template UUID | [optional] 
**TemplateName** | Pointer to **string** | Human-readable template name | [optional] 
**Description** | Pointer to **NullableString** | Optional template description | [optional] 
**Category** | Pointer to **NullableString** | Optional template category grouping | [optional] 

## Methods

### NewBiTemplateInfo

`func NewBiTemplateInfo() *BiTemplateInfo`

NewBiTemplateInfo instantiates a new BiTemplateInfo object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBiTemplateInfoWithDefaults

`func NewBiTemplateInfoWithDefaults() *BiTemplateInfo`

NewBiTemplateInfoWithDefaults instantiates a new BiTemplateInfo object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *BiTemplateInfo) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *BiTemplateInfo) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *BiTemplateInfo) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *BiTemplateInfo) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetTemplateName

`func (o *BiTemplateInfo) GetTemplateName() string`

GetTemplateName returns the TemplateName field if non-nil, zero value otherwise.

### GetTemplateNameOk

`func (o *BiTemplateInfo) GetTemplateNameOk() (*string, bool)`

GetTemplateNameOk returns a tuple with the TemplateName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateName

`func (o *BiTemplateInfo) SetTemplateName(v string)`

SetTemplateName sets TemplateName field to given value.

### HasTemplateName

`func (o *BiTemplateInfo) HasTemplateName() bool`

HasTemplateName returns a boolean if a field has been set.

### GetDescription

`func (o *BiTemplateInfo) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *BiTemplateInfo) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *BiTemplateInfo) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *BiTemplateInfo) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *BiTemplateInfo) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *BiTemplateInfo) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetCategory

`func (o *BiTemplateInfo) GetCategory() string`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *BiTemplateInfo) GetCategoryOk() (*string, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *BiTemplateInfo) SetCategory(v string)`

SetCategory sets Category field to given value.

### HasCategory

`func (o *BiTemplateInfo) HasCategory() bool`

HasCategory returns a boolean if a field has been set.

### SetCategoryNil

`func (o *BiTemplateInfo) SetCategoryNil(b bool)`

 SetCategoryNil sets the value for Category to be an explicit nil

### UnsetCategory
`func (o *BiTemplateInfo) UnsetCategory()`

UnsetCategory ensures that no value is present for Category, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


