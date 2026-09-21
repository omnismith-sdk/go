# EntityActionAvailability

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Action UUID | 
**Slug** | **string** | The identifier to execute it with: &#x60;POST /entities/{id}/actions/{slug}&#x60; | 
**Name** | **string** |  | 
**Description** | **NullableString** |  | 
**Icon** | **NullableString** | Material icon name | 
**Available** | **bool** | Whether the precondition holds for the record&#39;s current values. Executing an unavailable action returns 409. | 
**UnavailableReason** | **NullableString** | Why the action cannot run now, naming the attribute, the expectation and the current value. Null when available. | 
**Fields** | [**[]EntityActionAvailableField**](EntityActionAvailableField.md) | Values to submit, in dialog order | 
**Presets** | [**[]EntityActionAvailablePreset**](EntityActionAvailablePreset.md) | Values the action writes on its own | 

## Methods

### NewEntityActionAvailability

`func NewEntityActionAvailability(id string, slug string, name string, description NullableString, icon NullableString, available bool, unavailableReason NullableString, fields []EntityActionAvailableField, presets []EntityActionAvailablePreset, ) *EntityActionAvailability`

NewEntityActionAvailability instantiates a new EntityActionAvailability object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityActionAvailabilityWithDefaults

`func NewEntityActionAvailabilityWithDefaults() *EntityActionAvailability`

NewEntityActionAvailabilityWithDefaults instantiates a new EntityActionAvailability object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *EntityActionAvailability) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *EntityActionAvailability) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *EntityActionAvailability) SetId(v string)`

SetId sets Id field to given value.


### GetSlug

`func (o *EntityActionAvailability) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *EntityActionAvailability) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *EntityActionAvailability) SetSlug(v string)`

SetSlug sets Slug field to given value.


### GetName

`func (o *EntityActionAvailability) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *EntityActionAvailability) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *EntityActionAvailability) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *EntityActionAvailability) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *EntityActionAvailability) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *EntityActionAvailability) SetDescription(v string)`

SetDescription sets Description field to given value.


### SetDescriptionNil

`func (o *EntityActionAvailability) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *EntityActionAvailability) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetIcon

`func (o *EntityActionAvailability) GetIcon() string`

GetIcon returns the Icon field if non-nil, zero value otherwise.

### GetIconOk

`func (o *EntityActionAvailability) GetIconOk() (*string, bool)`

GetIconOk returns a tuple with the Icon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIcon

`func (o *EntityActionAvailability) SetIcon(v string)`

SetIcon sets Icon field to given value.


### SetIconNil

`func (o *EntityActionAvailability) SetIconNil(b bool)`

 SetIconNil sets the value for Icon to be an explicit nil

### UnsetIcon
`func (o *EntityActionAvailability) UnsetIcon()`

UnsetIcon ensures that no value is present for Icon, not even an explicit nil
### GetAvailable

`func (o *EntityActionAvailability) GetAvailable() bool`

GetAvailable returns the Available field if non-nil, zero value otherwise.

### GetAvailableOk

`func (o *EntityActionAvailability) GetAvailableOk() (*bool, bool)`

GetAvailableOk returns a tuple with the Available field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAvailable

`func (o *EntityActionAvailability) SetAvailable(v bool)`

SetAvailable sets Available field to given value.


### GetUnavailableReason

`func (o *EntityActionAvailability) GetUnavailableReason() string`

GetUnavailableReason returns the UnavailableReason field if non-nil, zero value otherwise.

### GetUnavailableReasonOk

`func (o *EntityActionAvailability) GetUnavailableReasonOk() (*string, bool)`

GetUnavailableReasonOk returns a tuple with the UnavailableReason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUnavailableReason

`func (o *EntityActionAvailability) SetUnavailableReason(v string)`

SetUnavailableReason sets UnavailableReason field to given value.


### SetUnavailableReasonNil

`func (o *EntityActionAvailability) SetUnavailableReasonNil(b bool)`

 SetUnavailableReasonNil sets the value for UnavailableReason to be an explicit nil

### UnsetUnavailableReason
`func (o *EntityActionAvailability) UnsetUnavailableReason()`

UnsetUnavailableReason ensures that no value is present for UnavailableReason, not even an explicit nil
### GetFields

`func (o *EntityActionAvailability) GetFields() []EntityActionAvailableField`

GetFields returns the Fields field if non-nil, zero value otherwise.

### GetFieldsOk

`func (o *EntityActionAvailability) GetFieldsOk() (*[]EntityActionAvailableField, bool)`

GetFieldsOk returns a tuple with the Fields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFields

`func (o *EntityActionAvailability) SetFields(v []EntityActionAvailableField)`

SetFields sets Fields field to given value.


### GetPresets

`func (o *EntityActionAvailability) GetPresets() []EntityActionAvailablePreset`

GetPresets returns the Presets field if non-nil, zero value otherwise.

### GetPresetsOk

`func (o *EntityActionAvailability) GetPresetsOk() (*[]EntityActionAvailablePreset, bool)`

GetPresetsOk returns a tuple with the Presets field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPresets

`func (o *EntityActionAvailability) SetPresets(v []EntityActionAvailablePreset)`

SetPresets sets Presets field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


