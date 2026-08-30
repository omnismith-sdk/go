# TemplateGroupInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **NullableString** | Optional group UUID. Auto-generated if omitted. | [optional] 
**Name** | **string** | Group display title / section heading | 
**Description** | Pointer to **NullableString** | Optional group descriptive subtitle | [optional] 
**Icon** | Pointer to **NullableString** | Optional icon name for the section header | [optional] 
**Columns** | Pointer to **int32** | Grid column layout count (1 or 2) | [optional] [default to 2]
**AttributeIds** | Pointer to **[]string** | Ordered list of attribute UUIDs assigned to this section group. | [optional] 

## Methods

### NewTemplateGroupInput

`func NewTemplateGroupInput(name string, ) *TemplateGroupInput`

NewTemplateGroupInput instantiates a new TemplateGroupInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTemplateGroupInputWithDefaults

`func NewTemplateGroupInputWithDefaults() *TemplateGroupInput`

NewTemplateGroupInputWithDefaults instantiates a new TemplateGroupInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *TemplateGroupInput) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *TemplateGroupInput) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *TemplateGroupInput) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *TemplateGroupInput) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *TemplateGroupInput) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *TemplateGroupInput) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetName

`func (o *TemplateGroupInput) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *TemplateGroupInput) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *TemplateGroupInput) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *TemplateGroupInput) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *TemplateGroupInput) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *TemplateGroupInput) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *TemplateGroupInput) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *TemplateGroupInput) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *TemplateGroupInput) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetIcon

`func (o *TemplateGroupInput) GetIcon() string`

GetIcon returns the Icon field if non-nil, zero value otherwise.

### GetIconOk

`func (o *TemplateGroupInput) GetIconOk() (*string, bool)`

GetIconOk returns a tuple with the Icon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIcon

`func (o *TemplateGroupInput) SetIcon(v string)`

SetIcon sets Icon field to given value.

### HasIcon

`func (o *TemplateGroupInput) HasIcon() bool`

HasIcon returns a boolean if a field has been set.

### SetIconNil

`func (o *TemplateGroupInput) SetIconNil(b bool)`

 SetIconNil sets the value for Icon to be an explicit nil

### UnsetIcon
`func (o *TemplateGroupInput) UnsetIcon()`

UnsetIcon ensures that no value is present for Icon, not even an explicit nil
### GetColumns

`func (o *TemplateGroupInput) GetColumns() int32`

GetColumns returns the Columns field if non-nil, zero value otherwise.

### GetColumnsOk

`func (o *TemplateGroupInput) GetColumnsOk() (*int32, bool)`

GetColumnsOk returns a tuple with the Columns field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColumns

`func (o *TemplateGroupInput) SetColumns(v int32)`

SetColumns sets Columns field to given value.

### HasColumns

`func (o *TemplateGroupInput) HasColumns() bool`

HasColumns returns a boolean if a field has been set.

### GetAttributeIds

`func (o *TemplateGroupInput) GetAttributeIds() []string`

GetAttributeIds returns the AttributeIds field if non-nil, zero value otherwise.

### GetAttributeIdsOk

`func (o *TemplateGroupInput) GetAttributeIdsOk() (*[]string, bool)`

GetAttributeIdsOk returns a tuple with the AttributeIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeIds

`func (o *TemplateGroupInput) SetAttributeIds(v []string)`

SetAttributeIds sets AttributeIds field to given value.

### HasAttributeIds

`func (o *TemplateGroupInput) HasAttributeIds() bool`

HasAttributeIds returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


