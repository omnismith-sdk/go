# CreateEntityActionRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Slug** | **string** | Identifier used in URLs and by agents; unique per template. Lowercase letters, digits and underscores, starting with a letter. | 
**Name** | **string** | Label shown in menus and dialogs | 
**Description** | Pointer to **NullableString** | What the action does, shown in the dialog | [optional] 
**Icon** | Pointer to **NullableString** | Material icon name | [optional] 
**Precondition** | Pointer to [**[]EntityRulePredicate**](EntityRulePredicate.md) | Conditions on the record&#39;s current values that must all hold for the action to be available. Omit or send an empty list for an action that is always available. | [optional] 
**Fields** | Pointer to [**[]EntityActionField**](EntityActionField.md) | Values the operator is asked for, in dialog order. Each attribute may appear once and must not also be a preset. | [optional] 
**Presets** | Pointer to [**[]EntityActionPreset**](EntityActionPreset.md) | Values written silently on execution. Each attribute may appear once and must not also be a field. | [optional] 

## Methods

### NewCreateEntityActionRequest

`func NewCreateEntityActionRequest(slug string, name string, ) *CreateEntityActionRequest`

NewCreateEntityActionRequest instantiates a new CreateEntityActionRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateEntityActionRequestWithDefaults

`func NewCreateEntityActionRequestWithDefaults() *CreateEntityActionRequest`

NewCreateEntityActionRequestWithDefaults instantiates a new CreateEntityActionRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSlug

`func (o *CreateEntityActionRequest) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *CreateEntityActionRequest) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *CreateEntityActionRequest) SetSlug(v string)`

SetSlug sets Slug field to given value.


### GetName

`func (o *CreateEntityActionRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateEntityActionRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateEntityActionRequest) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *CreateEntityActionRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateEntityActionRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateEntityActionRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CreateEntityActionRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *CreateEntityActionRequest) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *CreateEntityActionRequest) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetIcon

`func (o *CreateEntityActionRequest) GetIcon() string`

GetIcon returns the Icon field if non-nil, zero value otherwise.

### GetIconOk

`func (o *CreateEntityActionRequest) GetIconOk() (*string, bool)`

GetIconOk returns a tuple with the Icon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIcon

`func (o *CreateEntityActionRequest) SetIcon(v string)`

SetIcon sets Icon field to given value.

### HasIcon

`func (o *CreateEntityActionRequest) HasIcon() bool`

HasIcon returns a boolean if a field has been set.

### SetIconNil

`func (o *CreateEntityActionRequest) SetIconNil(b bool)`

 SetIconNil sets the value for Icon to be an explicit nil

### UnsetIcon
`func (o *CreateEntityActionRequest) UnsetIcon()`

UnsetIcon ensures that no value is present for Icon, not even an explicit nil
### GetPrecondition

`func (o *CreateEntityActionRequest) GetPrecondition() []EntityRulePredicate`

GetPrecondition returns the Precondition field if non-nil, zero value otherwise.

### GetPreconditionOk

`func (o *CreateEntityActionRequest) GetPreconditionOk() (*[]EntityRulePredicate, bool)`

GetPreconditionOk returns a tuple with the Precondition field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrecondition

`func (o *CreateEntityActionRequest) SetPrecondition(v []EntityRulePredicate)`

SetPrecondition sets Precondition field to given value.

### HasPrecondition

`func (o *CreateEntityActionRequest) HasPrecondition() bool`

HasPrecondition returns a boolean if a field has been set.

### GetFields

`func (o *CreateEntityActionRequest) GetFields() []EntityActionField`

GetFields returns the Fields field if non-nil, zero value otherwise.

### GetFieldsOk

`func (o *CreateEntityActionRequest) GetFieldsOk() (*[]EntityActionField, bool)`

GetFieldsOk returns a tuple with the Fields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFields

`func (o *CreateEntityActionRequest) SetFields(v []EntityActionField)`

SetFields sets Fields field to given value.

### HasFields

`func (o *CreateEntityActionRequest) HasFields() bool`

HasFields returns a boolean if a field has been set.

### GetPresets

`func (o *CreateEntityActionRequest) GetPresets() []EntityActionPreset`

GetPresets returns the Presets field if non-nil, zero value otherwise.

### GetPresetsOk

`func (o *CreateEntityActionRequest) GetPresetsOk() (*[]EntityActionPreset, bool)`

GetPresetsOk returns a tuple with the Presets field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPresets

`func (o *CreateEntityActionRequest) SetPresets(v []EntityActionPreset)`

SetPresets sets Presets field to given value.

### HasPresets

`func (o *CreateEntityActionRequest) HasPresets() bool`

HasPresets returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


