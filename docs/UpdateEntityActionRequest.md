# UpdateEntityActionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Slug** | **string** | Identifier used in URLs and by agents; unique per template. Lowercase letters, digits and underscores, starting with a letter. | 
**Name** | **string** | Label shown in menus and dialogs | 
**Description** | Pointer to **NullableString** | What the action does, shown in the dialog | [optional] 
**Icon** | Pointer to **NullableString** | Material icon name | [optional] 
**Precondition** | Pointer to [**[]EntityRulePredicate**](EntityRulePredicate.md) | Full replacement of the precondition; empty for an action that is always available | [optional] 
**Fields** | Pointer to [**[]EntityActionField**](EntityActionField.md) | Full replacement of the fields, in dialog order | [optional] 
**Presets** | Pointer to [**[]EntityActionPreset**](EntityActionPreset.md) | Full replacement of the presets | [optional] 

## Methods

### NewUpdateEntityActionRequest

`func NewUpdateEntityActionRequest(slug string, name string, ) *UpdateEntityActionRequest`

NewUpdateEntityActionRequest instantiates a new UpdateEntityActionRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateEntityActionRequestWithDefaults

`func NewUpdateEntityActionRequestWithDefaults() *UpdateEntityActionRequest`

NewUpdateEntityActionRequestWithDefaults instantiates a new UpdateEntityActionRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSlug

`func (o *UpdateEntityActionRequest) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *UpdateEntityActionRequest) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *UpdateEntityActionRequest) SetSlug(v string)`

SetSlug sets Slug field to given value.


### GetName

`func (o *UpdateEntityActionRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateEntityActionRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateEntityActionRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *UpdateEntityActionRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *UpdateEntityActionRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *UpdateEntityActionRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *UpdateEntityActionRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *UpdateEntityActionRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *UpdateEntityActionRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetIcon

`func (o *UpdateEntityActionRequest) GetIcon() string`

GetIcon returns the Icon field if non-nil, zero value otherwise.

### GetIconOk

`func (o *UpdateEntityActionRequest) GetIconOk() (*string, bool)`

GetIconOk returns a tuple with the Icon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIcon

`func (o *UpdateEntityActionRequest) SetIcon(v string)`

SetIcon sets Icon field to given value.

### HasIcon

`func (o *UpdateEntityActionRequest) HasIcon() bool`

HasIcon returns a boolean if a field has been set.

### SetIconNil

`func (o *UpdateEntityActionRequest) SetIconNil(b bool)`

 SetIconNil sets the value for Icon to be an explicit nil

### UnsetIcon
`func (o *UpdateEntityActionRequest) UnsetIcon()`

UnsetIcon ensures that no value is present for Icon, not even an explicit nil
### GetPrecondition

`func (o *UpdateEntityActionRequest) GetPrecondition() []EntityRulePredicate`

GetPrecondition returns the Precondition field if non-nil, zero value otherwise.

### GetPreconditionOk

`func (o *UpdateEntityActionRequest) GetPreconditionOk() (*[]EntityRulePredicate, bool)`

GetPreconditionOk returns a tuple with the Precondition field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrecondition

`func (o *UpdateEntityActionRequest) SetPrecondition(v []EntityRulePredicate)`

SetPrecondition sets Precondition field to given value.

### HasPrecondition

`func (o *UpdateEntityActionRequest) HasPrecondition() bool`

HasPrecondition returns a boolean if a field has been set.

### GetFields

`func (o *UpdateEntityActionRequest) GetFields() []EntityActionField`

GetFields returns the Fields field if non-nil, zero value otherwise.

### GetFieldsOk

`func (o *UpdateEntityActionRequest) GetFieldsOk() (*[]EntityActionField, bool)`

GetFieldsOk returns a tuple with the Fields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFields

`func (o *UpdateEntityActionRequest) SetFields(v []EntityActionField)`

SetFields sets Fields field to given value.

### HasFields

`func (o *UpdateEntityActionRequest) HasFields() bool`

HasFields returns a boolean if a field has been set.

### GetPresets

`func (o *UpdateEntityActionRequest) GetPresets() []EntityActionPreset`

GetPresets returns the Presets field if non-nil, zero value otherwise.

### GetPresetsOk

`func (o *UpdateEntityActionRequest) GetPresetsOk() (*[]EntityActionPreset, bool)`

GetPresetsOk returns a tuple with the Presets field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPresets

`func (o *UpdateEntityActionRequest) SetPresets(v []EntityActionPreset)`

SetPresets sets Presets field to given value.

### HasPresets

`func (o *UpdateEntityActionRequest) HasPresets() bool`

HasPresets returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


