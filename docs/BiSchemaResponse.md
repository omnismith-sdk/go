# BiSchemaResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Templates** | Pointer to [**[]BiTemplateInfo**](BiTemplateInfo.md) | List of template schemas available for BI integration | [optional] 
**Fields** | Pointer to [**[]BiSchemaField**](BiSchemaField.md) | Normalized field definitions across all templates with type mappings | [optional] 

## Methods

### NewBiSchemaResponse

`func NewBiSchemaResponse() *BiSchemaResponse`

NewBiSchemaResponse instantiates a new BiSchemaResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBiSchemaResponseWithDefaults

`func NewBiSchemaResponseWithDefaults() *BiSchemaResponse`

NewBiSchemaResponseWithDefaults instantiates a new BiSchemaResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplates

`func (o *BiSchemaResponse) GetTemplates() []BiTemplateInfo`

GetTemplates returns the Templates field if non-nil, zero value otherwise.

### GetTemplatesOk

`func (o *BiSchemaResponse) GetTemplatesOk() (*[]BiTemplateInfo, bool)`

GetTemplatesOk returns a tuple with the Templates field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplates

`func (o *BiSchemaResponse) SetTemplates(v []BiTemplateInfo)`

SetTemplates sets Templates field to given value.

### HasTemplates

`func (o *BiSchemaResponse) HasTemplates() bool`

HasTemplates returns a boolean if a field has been set.

### GetFields

`func (o *BiSchemaResponse) GetFields() []BiSchemaField`

GetFields returns the Fields field if non-nil, zero value otherwise.

### GetFieldsOk

`func (o *BiSchemaResponse) GetFieldsOk() (*[]BiSchemaField, bool)`

GetFieldsOk returns a tuple with the Fields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFields

`func (o *BiSchemaResponse) SetFields(v []BiSchemaField)`

SetFields sets Fields field to given value.

### HasFields

`func (o *BiSchemaResponse) HasFields() bool`

HasFields returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


