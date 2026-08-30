# TemplateGroupResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Unique group UUID | 
**Name** | **string** | Group display title / section heading | 
**Description** | Pointer to **NullableString** | Optional group descriptive subtitle | [optional] 
**Icon** | Pointer to **NullableString** | Optional icon name for the section header | [optional] 
**Columns** | **int32** | Grid column layout count (1 or 2) | 
**AttributeIds** | **[]string** | Ordered list of attribute UUIDs assigned to this section group. | 

## Methods

### NewTemplateGroupResponse

`func NewTemplateGroupResponse(id string, name string, columns int32, attributeIds []string, ) *TemplateGroupResponse`

NewTemplateGroupResponse instantiates a new TemplateGroupResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTemplateGroupResponseWithDefaults

`func NewTemplateGroupResponseWithDefaults() *TemplateGroupResponse`

NewTemplateGroupResponseWithDefaults instantiates a new TemplateGroupResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *TemplateGroupResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *TemplateGroupResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *TemplateGroupResponse) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *TemplateGroupResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *TemplateGroupResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *TemplateGroupResponse) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *TemplateGroupResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *TemplateGroupResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *TemplateGroupResponse) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *TemplateGroupResponse) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *TemplateGroupResponse) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *TemplateGroupResponse) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetIcon

`func (o *TemplateGroupResponse) GetIcon() string`

GetIcon returns the Icon field if non-nil, zero value otherwise.

### GetIconOk

`func (o *TemplateGroupResponse) GetIconOk() (*string, bool)`

GetIconOk returns a tuple with the Icon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIcon

`func (o *TemplateGroupResponse) SetIcon(v string)`

SetIcon sets Icon field to given value.

### HasIcon

`func (o *TemplateGroupResponse) HasIcon() bool`

HasIcon returns a boolean if a field has been set.

### SetIconNil

`func (o *TemplateGroupResponse) SetIconNil(b bool)`

 SetIconNil sets the value for Icon to be an explicit nil

### UnsetIcon
`func (o *TemplateGroupResponse) UnsetIcon()`

UnsetIcon ensures that no value is present for Icon, not even an explicit nil
### GetColumns

`func (o *TemplateGroupResponse) GetColumns() int32`

GetColumns returns the Columns field if non-nil, zero value otherwise.

### GetColumnsOk

`func (o *TemplateGroupResponse) GetColumnsOk() (*int32, bool)`

GetColumnsOk returns a tuple with the Columns field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetColumns

`func (o *TemplateGroupResponse) SetColumns(v int32)`

SetColumns sets Columns field to given value.


### GetAttributeIds

`func (o *TemplateGroupResponse) GetAttributeIds() []string`

GetAttributeIds returns the AttributeIds field if non-nil, zero value otherwise.

### GetAttributeIdsOk

`func (o *TemplateGroupResponse) GetAttributeIdsOk() (*[]string, bool)`

GetAttributeIdsOk returns a tuple with the AttributeIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeIds

`func (o *TemplateGroupResponse) SetAttributeIds(v []string)`

SetAttributeIds sets AttributeIds field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


