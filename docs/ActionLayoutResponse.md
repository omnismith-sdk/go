# ActionLayoutResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ActionId** | **string** | Action UUID | 
**TemplateId** | **string** | Template UUID | 
**Icon** | Pointer to **NullableString** | Material icon identifier for action buttons and dialogs | [optional] 
**SortOrder** | **int32** | Display sorting rank in action menus | 

## Methods

### NewActionLayoutResponse

`func NewActionLayoutResponse(actionId string, templateId string, sortOrder int32, ) *ActionLayoutResponse`

NewActionLayoutResponse instantiates a new ActionLayoutResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewActionLayoutResponseWithDefaults

`func NewActionLayoutResponseWithDefaults() *ActionLayoutResponse`

NewActionLayoutResponseWithDefaults instantiates a new ActionLayoutResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetActionId

`func (o *ActionLayoutResponse) GetActionId() string`

GetActionId returns the ActionId field if non-nil, zero value otherwise.

### GetActionIdOk

`func (o *ActionLayoutResponse) GetActionIdOk() (*string, bool)`

GetActionIdOk returns a tuple with the ActionId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActionId

`func (o *ActionLayoutResponse) SetActionId(v string)`

SetActionId sets ActionId field to given value.


### GetTemplateId

`func (o *ActionLayoutResponse) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *ActionLayoutResponse) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *ActionLayoutResponse) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.


### GetIcon

`func (o *ActionLayoutResponse) GetIcon() string`

GetIcon returns the Icon field if non-nil, zero value otherwise.

### GetIconOk

`func (o *ActionLayoutResponse) GetIconOk() (*string, bool)`

GetIconOk returns a tuple with the Icon field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIcon

`func (o *ActionLayoutResponse) SetIcon(v string)`

SetIcon sets Icon field to given value.

### HasIcon

`func (o *ActionLayoutResponse) HasIcon() bool`

HasIcon returns a boolean if a field has been set.

### SetIconNil

`func (o *ActionLayoutResponse) SetIconNil(b bool)`

 SetIconNil sets the value for Icon to be an explicit nil

### UnsetIcon
`func (o *ActionLayoutResponse) UnsetIcon()`

UnsetIcon ensures that no value is present for Icon, not even an explicit nil
### GetSortOrder

`func (o *ActionLayoutResponse) GetSortOrder() int32`

GetSortOrder returns the SortOrder field if non-nil, zero value otherwise.

### GetSortOrderOk

`func (o *ActionLayoutResponse) GetSortOrderOk() (*int32, bool)`

GetSortOrderOk returns a tuple with the SortOrder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSortOrder

`func (o *ActionLayoutResponse) SetSortOrder(v int32)`

SetSortOrder sets SortOrder field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


