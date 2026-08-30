# BiSchemaField

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | Pointer to **string** | Template UUID to which this field belongs | [optional] 
**TemplateName** | Pointer to **string** | Display name of the template schema | [optional] 
**ColumnName** | Pointer to **string** | Sanitized SQL-friendly column identifier for BI connectors | [optional] 
**Label** | Pointer to **string** | Human-readable column header label | [optional] 
**Source** | Pointer to **string** | Field origin (\&quot;system\&quot; for metadata columns, \&quot;attribute\&quot; for dynamic template attributes) | [optional] 
**AttributeId** | Pointer to **NullableString** | Attribute definition UUID if source is attribute | [optional] 
**AttributeName** | Pointer to **NullableString** | Display name of the attribute definition | [optional] 
**AttributeType** | Pointer to **NullableString** | Kind of dynamic attribute (dimension, metric, list, reference) | [optional] 
**DataType** | Pointer to **string** | Canonical data type mapping for BI tooling (string, number, boolean, datetime, date) | [optional] 
**ReferenceTargetTemplateId** | Pointer to **NullableString** | Target template UUID if this is a reference attribute | [optional] 
**ReferenceTargetAttributeId** | Pointer to **NullableString** | Target display attribute UUID if this is a reference attribute | [optional] 
**ListOptions** | Pointer to [**[]BiFieldOption**](BiFieldOption.md) | Allowed selectable options if this is a list attribute | [optional] 

## Methods

### NewBiSchemaField

`func NewBiSchemaField() *BiSchemaField`

NewBiSchemaField instantiates a new BiSchemaField object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBiSchemaFieldWithDefaults

`func NewBiSchemaFieldWithDefaults() *BiSchemaField`

NewBiSchemaFieldWithDefaults instantiates a new BiSchemaField object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *BiSchemaField) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *BiSchemaField) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *BiSchemaField) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *BiSchemaField) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetTemplateName

`func (o *BiSchemaField) GetTemplateName() string`

GetTemplateName returns the TemplateName field if non-nil, zero value otherwise.

### GetTemplateNameOk

`func (o *BiSchemaField) GetTemplateNameOk() (*string, bool)`

GetTemplateNameOk returns a tuple with the TemplateName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateName

`func (o *BiSchemaField) SetTemplateName(v string)`

SetTemplateName sets TemplateName field to given value.

### HasTemplateName

`func (o *BiSchemaField) HasTemplateName() bool`

HasTemplateName returns a boolean if a field has been set.

### GetColumnName

`func (o *BiSchemaField) GetColumnName() string`

GetColumnName returns the ColumnName field if non-nil, zero value otherwise.

### GetColumnNameOk

`func (o *BiSchemaField) GetColumnNameOk() (*string, bool)`

GetColumnNameOk returns a tuple with the ColumnName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColumnName

`func (o *BiSchemaField) SetColumnName(v string)`

SetColumnName sets ColumnName field to given value.

### HasColumnName

`func (o *BiSchemaField) HasColumnName() bool`

HasColumnName returns a boolean if a field has been set.

### GetLabel

`func (o *BiSchemaField) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *BiSchemaField) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *BiSchemaField) SetLabel(v string)`

SetLabel sets Label field to given value.

### HasLabel

`func (o *BiSchemaField) HasLabel() bool`

HasLabel returns a boolean if a field has been set.

### GetSource

`func (o *BiSchemaField) GetSource() string`

GetSource returns the Source field if non-nil, zero value otherwise.

### GetSourceOk

`func (o *BiSchemaField) GetSourceOk() (*string, bool)`

GetSourceOk returns a tuple with the Source field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSource

`func (o *BiSchemaField) SetSource(v string)`

SetSource sets Source field to given value.

### HasSource

`func (o *BiSchemaField) HasSource() bool`

HasSource returns a boolean if a field has been set.

### GetAttributeId

`func (o *BiSchemaField) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *BiSchemaField) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *BiSchemaField) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.

### HasAttributeId

`func (o *BiSchemaField) HasAttributeId() bool`

HasAttributeId returns a boolean if a field has been set.

### SetAttributeIdNil

`func (o *BiSchemaField) SetAttributeIdNil(b bool)`

 SetAttributeIdNil sets the value for AttributeId to be an explicit nil

### UnsetAttributeId
`func (o *BiSchemaField) UnsetAttributeId()`

UnsetAttributeId ensures that no value is present for AttributeId, not even an explicit nil
### GetAttributeName

`func (o *BiSchemaField) GetAttributeName() string`

GetAttributeName returns the AttributeName field if non-nil, zero value otherwise.

### GetAttributeNameOk

`func (o *BiSchemaField) GetAttributeNameOk() (*string, bool)`

GetAttributeNameOk returns a tuple with the AttributeName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeName

`func (o *BiSchemaField) SetAttributeName(v string)`

SetAttributeName sets AttributeName field to given value.

### HasAttributeName

`func (o *BiSchemaField) HasAttributeName() bool`

HasAttributeName returns a boolean if a field has been set.

### SetAttributeNameNil

`func (o *BiSchemaField) SetAttributeNameNil(b bool)`

 SetAttributeNameNil sets the value for AttributeName to be an explicit nil

### UnsetAttributeName
`func (o *BiSchemaField) UnsetAttributeName()`

UnsetAttributeName ensures that no value is present for AttributeName, not even an explicit nil
### GetAttributeType

`func (o *BiSchemaField) GetAttributeType() string`

GetAttributeType returns the AttributeType field if non-nil, zero value otherwise.

### GetAttributeTypeOk

`func (o *BiSchemaField) GetAttributeTypeOk() (*string, bool)`

GetAttributeTypeOk returns a tuple with the AttributeType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeType

`func (o *BiSchemaField) SetAttributeType(v string)`

SetAttributeType sets AttributeType field to given value.

### HasAttributeType

`func (o *BiSchemaField) HasAttributeType() bool`

HasAttributeType returns a boolean if a field has been set.

### SetAttributeTypeNil

`func (o *BiSchemaField) SetAttributeTypeNil(b bool)`

 SetAttributeTypeNil sets the value for AttributeType to be an explicit nil

### UnsetAttributeType
`func (o *BiSchemaField) UnsetAttributeType()`

UnsetAttributeType ensures that no value is present for AttributeType, not even an explicit nil
### GetDataType

`func (o *BiSchemaField) GetDataType() string`

GetDataType returns the DataType field if non-nil, zero value otherwise.

### GetDataTypeOk

`func (o *BiSchemaField) GetDataTypeOk() (*string, bool)`

GetDataTypeOk returns a tuple with the DataType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDataType

`func (o *BiSchemaField) SetDataType(v string)`

SetDataType sets DataType field to given value.

### HasDataType

`func (o *BiSchemaField) HasDataType() bool`

HasDataType returns a boolean if a field has been set.

### GetReferenceTargetTemplateId

`func (o *BiSchemaField) GetReferenceTargetTemplateId() string`

GetReferenceTargetTemplateId returns the ReferenceTargetTemplateId field if non-nil, zero value otherwise.

### GetReferenceTargetTemplateIdOk

`func (o *BiSchemaField) GetReferenceTargetTemplateIdOk() (*string, bool)`

GetReferenceTargetTemplateIdOk returns a tuple with the ReferenceTargetTemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferenceTargetTemplateId

`func (o *BiSchemaField) SetReferenceTargetTemplateId(v string)`

SetReferenceTargetTemplateId sets ReferenceTargetTemplateId field to given value.

### HasReferenceTargetTemplateId

`func (o *BiSchemaField) HasReferenceTargetTemplateId() bool`

HasReferenceTargetTemplateId returns a boolean if a field has been set.

### SetReferenceTargetTemplateIdNil

`func (o *BiSchemaField) SetReferenceTargetTemplateIdNil(b bool)`

 SetReferenceTargetTemplateIdNil sets the value for ReferenceTargetTemplateId to be an explicit nil

### UnsetReferenceTargetTemplateId
`func (o *BiSchemaField) UnsetReferenceTargetTemplateId()`

UnsetReferenceTargetTemplateId ensures that no value is present for ReferenceTargetTemplateId, not even an explicit nil
### GetReferenceTargetAttributeId

`func (o *BiSchemaField) GetReferenceTargetAttributeId() string`

GetReferenceTargetAttributeId returns the ReferenceTargetAttributeId field if non-nil, zero value otherwise.

### GetReferenceTargetAttributeIdOk

`func (o *BiSchemaField) GetReferenceTargetAttributeIdOk() (*string, bool)`

GetReferenceTargetAttributeIdOk returns a tuple with the ReferenceTargetAttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferenceTargetAttributeId

`func (o *BiSchemaField) SetReferenceTargetAttributeId(v string)`

SetReferenceTargetAttributeId sets ReferenceTargetAttributeId field to given value.

### HasReferenceTargetAttributeId

`func (o *BiSchemaField) HasReferenceTargetAttributeId() bool`

HasReferenceTargetAttributeId returns a boolean if a field has been set.

### SetReferenceTargetAttributeIdNil

`func (o *BiSchemaField) SetReferenceTargetAttributeIdNil(b bool)`

 SetReferenceTargetAttributeIdNil sets the value for ReferenceTargetAttributeId to be an explicit nil

### UnsetReferenceTargetAttributeId
`func (o *BiSchemaField) UnsetReferenceTargetAttributeId()`

UnsetReferenceTargetAttributeId ensures that no value is present for ReferenceTargetAttributeId, not even an explicit nil
### GetListOptions

`func (o *BiSchemaField) GetListOptions() []BiFieldOption`

GetListOptions returns the ListOptions field if non-nil, zero value otherwise.

### GetListOptionsOk

`func (o *BiSchemaField) GetListOptionsOk() (*[]BiFieldOption, bool)`

GetListOptionsOk returns a tuple with the ListOptions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetListOptions

`func (o *BiSchemaField) SetListOptions(v []BiFieldOption)`

SetListOptions sets ListOptions field to given value.

### HasListOptions

`func (o *BiSchemaField) HasListOptions() bool`

HasListOptions returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


