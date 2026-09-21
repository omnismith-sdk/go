# EntityActionOverviewResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Action UUID | 
**Slug** | **string** | Action slug identifier | 
**Name** | **string** | Human-readable action name | 
**Description** | Pointer to **NullableString** | Action description | [optional] 
**IsEnabled** | **bool** | Whether the action is active and executable | 
**Precondition** | [**[]EntityRulePredicateOverviewResponse**](EntityRulePredicateOverviewResponse.md) | Conditions that must hold on the record for the action to be available | 
**Fields** | [**[]EntityActionFieldOverviewResponse**](EntityActionFieldOverviewResponse.md) | Fields prompted from the operator | 
**Presets** | [**[]EntityActionPresetOverviewResponse**](EntityActionPresetOverviewResponse.md) | Values written silently upon execution | 

## Methods

### NewEntityActionOverviewResponse

`func NewEntityActionOverviewResponse(id string, slug string, name string, isEnabled bool, precondition []EntityRulePredicateOverviewResponse, fields []EntityActionFieldOverviewResponse, presets []EntityActionPresetOverviewResponse, ) *EntityActionOverviewResponse`

NewEntityActionOverviewResponse instantiates a new EntityActionOverviewResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityActionOverviewResponseWithDefaults

`func NewEntityActionOverviewResponseWithDefaults() *EntityActionOverviewResponse`

NewEntityActionOverviewResponseWithDefaults instantiates a new EntityActionOverviewResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *EntityActionOverviewResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *EntityActionOverviewResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *EntityActionOverviewResponse) SetId(v string)`

SetId sets Id field to given value.


### GetSlug

`func (o *EntityActionOverviewResponse) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *EntityActionOverviewResponse) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *EntityActionOverviewResponse) SetSlug(v string)`

SetSlug sets Slug field to given value.


### GetName

`func (o *EntityActionOverviewResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *EntityActionOverviewResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *EntityActionOverviewResponse) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *EntityActionOverviewResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *EntityActionOverviewResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *EntityActionOverviewResponse) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *EntityActionOverviewResponse) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *EntityActionOverviewResponse) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *EntityActionOverviewResponse) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetIsEnabled

`func (o *EntityActionOverviewResponse) GetIsEnabled() bool`

GetIsEnabled returns the IsEnabled field if non-nil, zero value otherwise.

### GetIsEnabledOk

`func (o *EntityActionOverviewResponse) GetIsEnabledOk() (*bool, bool)`

GetIsEnabledOk returns a tuple with the IsEnabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsEnabled

`func (o *EntityActionOverviewResponse) SetIsEnabled(v bool)`

SetIsEnabled sets IsEnabled field to given value.


### GetPrecondition

`func (o *EntityActionOverviewResponse) GetPrecondition() []EntityRulePredicateOverviewResponse`

GetPrecondition returns the Precondition field if non-nil, zero value otherwise.

### GetPreconditionOk

`func (o *EntityActionOverviewResponse) GetPreconditionOk() (*[]EntityRulePredicateOverviewResponse, bool)`

GetPreconditionOk returns a tuple with the Precondition field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPrecondition

`func (o *EntityActionOverviewResponse) SetPrecondition(v []EntityRulePredicateOverviewResponse)`

SetPrecondition sets Precondition field to given value.


### GetFields

`func (o *EntityActionOverviewResponse) GetFields() []EntityActionFieldOverviewResponse`

GetFields returns the Fields field if non-nil, zero value otherwise.

### GetFieldsOk

`func (o *EntityActionOverviewResponse) GetFieldsOk() (*[]EntityActionFieldOverviewResponse, bool)`

GetFieldsOk returns a tuple with the Fields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFields

`func (o *EntityActionOverviewResponse) SetFields(v []EntityActionFieldOverviewResponse)`

SetFields sets Fields field to given value.


### GetPresets

`func (o *EntityActionOverviewResponse) GetPresets() []EntityActionPresetOverviewResponse`

GetPresets returns the Presets field if non-nil, zero value otherwise.

### GetPresetsOk

`func (o *EntityActionOverviewResponse) GetPresetsOk() (*[]EntityActionPresetOverviewResponse, bool)`

GetPresetsOk returns a tuple with the Presets field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPresets

`func (o *EntityActionOverviewResponse) SetPresets(v []EntityActionPresetOverviewResponse)`

SetPresets sets Presets field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


