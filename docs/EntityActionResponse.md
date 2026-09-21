# EntityActionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Action UUID | [optional] 
**TemplateId** | Pointer to **string** | UUID of the template the action belongs to | [optional] 
**Slug** | Pointer to **string** | Identifier used in URLs and by agents; unique per template | [optional] 
**Name** | Pointer to **string** | Label shown in menus and dialogs | [optional] 
**Description** | Pointer to **NullableString** | What the action does, shown in the dialog | [optional] 
**Icon** | Pointer to **NullableString** | Material icon name | [optional] 
**IsEnabled** | Pointer to **bool** | Disabled actions are stored but neither listed for records nor executable | [optional] 
**Precondition** | Pointer to [**[]EntityRulePredicate**](EntityRulePredicate.md) | Conditions on the record&#39;s current values that must all hold for the action to be available. Empty means always available. | [optional] 
**Fields** | Pointer to [**[]EntityActionField**](EntityActionField.md) | Values the operator is asked for, in dialog order | [optional] 
**Presets** | Pointer to [**[]EntityActionPreset**](EntityActionPreset.md) | Values written silently on execution | [optional] 
**SortOrder** | Pointer to **int32** | Position among the template&#39;s actions, zero-based | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**UpdatedAt** | Pointer to **time.Time** |  | [optional] 

## Methods

### NewEntityActionResponse

`func NewEntityActionResponse() *EntityActionResponse`

NewEntityActionResponse instantiates a new EntityActionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityActionResponseWithDefaults

`func NewEntityActionResponseWithDefaults() *EntityActionResponse`

NewEntityActionResponseWithDefaults instantiates a new EntityActionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *EntityActionResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *EntityActionResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *EntityActionResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *EntityActionResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetTemplateId

`func (o *EntityActionResponse) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *EntityActionResponse) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *EntityActionResponse) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *EntityActionResponse) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### GetSlug

`func (o *EntityActionResponse) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *EntityActionResponse) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *EntityActionResponse) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *EntityActionResponse) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### GetName

`func (o *EntityActionResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *EntityActionResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *EntityActionResponse) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *EntityActionResponse) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *EntityActionResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *EntityActionResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *EntityActionResponse) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *EntityActionResponse) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *EntityActionResponse) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *EntityActionResponse) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetIcon

`func (o *EntityActionResponse) GetIcon() string`

GetIcon returns the Icon field if non-nil, zero value otherwise.

### GetIconOk

`func (o *EntityActionResponse) GetIconOk() (*string, bool)`

GetIconOk returns a tuple with the Icon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIcon

`func (o *EntityActionResponse) SetIcon(v string)`

SetIcon sets Icon field to given value.

### HasIcon

`func (o *EntityActionResponse) HasIcon() bool`

HasIcon returns a boolean if a field has been set.

### SetIconNil

`func (o *EntityActionResponse) SetIconNil(b bool)`

 SetIconNil sets the value for Icon to be an explicit nil

### UnsetIcon
`func (o *EntityActionResponse) UnsetIcon()`

UnsetIcon ensures that no value is present for Icon, not even an explicit nil
### GetIsEnabled

`func (o *EntityActionResponse) GetIsEnabled() bool`

GetIsEnabled returns the IsEnabled field if non-nil, zero value otherwise.

### GetIsEnabledOk

`func (o *EntityActionResponse) GetIsEnabledOk() (*bool, bool)`

GetIsEnabledOk returns a tuple with the IsEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsEnabled

`func (o *EntityActionResponse) SetIsEnabled(v bool)`

SetIsEnabled sets IsEnabled field to given value.

### HasIsEnabled

`func (o *EntityActionResponse) HasIsEnabled() bool`

HasIsEnabled returns a boolean if a field has been set.

### GetPrecondition

`func (o *EntityActionResponse) GetPrecondition() []EntityRulePredicate`

GetPrecondition returns the Precondition field if non-nil, zero value otherwise.

### GetPreconditionOk

`func (o *EntityActionResponse) GetPreconditionOk() (*[]EntityRulePredicate, bool)`

GetPreconditionOk returns a tuple with the Precondition field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrecondition

`func (o *EntityActionResponse) SetPrecondition(v []EntityRulePredicate)`

SetPrecondition sets Precondition field to given value.

### HasPrecondition

`func (o *EntityActionResponse) HasPrecondition() bool`

HasPrecondition returns a boolean if a field has been set.

### GetFields

`func (o *EntityActionResponse) GetFields() []EntityActionField`

GetFields returns the Fields field if non-nil, zero value otherwise.

### GetFieldsOk

`func (o *EntityActionResponse) GetFieldsOk() (*[]EntityActionField, bool)`

GetFieldsOk returns a tuple with the Fields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFields

`func (o *EntityActionResponse) SetFields(v []EntityActionField)`

SetFields sets Fields field to given value.

### HasFields

`func (o *EntityActionResponse) HasFields() bool`

HasFields returns a boolean if a field has been set.

### GetPresets

`func (o *EntityActionResponse) GetPresets() []EntityActionPreset`

GetPresets returns the Presets field if non-nil, zero value otherwise.

### GetPresetsOk

`func (o *EntityActionResponse) GetPresetsOk() (*[]EntityActionPreset, bool)`

GetPresetsOk returns a tuple with the Presets field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPresets

`func (o *EntityActionResponse) SetPresets(v []EntityActionPreset)`

SetPresets sets Presets field to given value.

### HasPresets

`func (o *EntityActionResponse) HasPresets() bool`

HasPresets returns a boolean if a field has been set.

### GetSortOrder

`func (o *EntityActionResponse) GetSortOrder() int32`

GetSortOrder returns the SortOrder field if non-nil, zero value otherwise.

### GetSortOrderOk

`func (o *EntityActionResponse) GetSortOrderOk() (*int32, bool)`

GetSortOrderOk returns a tuple with the SortOrder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortOrder

`func (o *EntityActionResponse) SetSortOrder(v int32)`

SetSortOrder sets SortOrder field to given value.

### HasSortOrder

`func (o *EntityActionResponse) HasSortOrder() bool`

HasSortOrder returns a boolean if a field has been set.

### GetCreatedAt

`func (o *EntityActionResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *EntityActionResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *EntityActionResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *EntityActionResponse) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *EntityActionResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *EntityActionResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *EntityActionResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *EntityActionResponse) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


