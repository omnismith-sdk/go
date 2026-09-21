# TemplateLayoutResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | **string** | Template UUID | 
**Category** | Pointer to **NullableString** | Template category for UI sidebar grouping | [optional] 
**Groups** | [**[]TemplateGroupResponse**](TemplateGroupResponse.md) | Ordered attribute groups for organizing fields into form sections | 

## Methods

### NewTemplateLayoutResponse

`func NewTemplateLayoutResponse(templateId string, groups []TemplateGroupResponse, ) *TemplateLayoutResponse`

NewTemplateLayoutResponse instantiates a new TemplateLayoutResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTemplateLayoutResponseWithDefaults

`func NewTemplateLayoutResponseWithDefaults() *TemplateLayoutResponse`

NewTemplateLayoutResponseWithDefaults instantiates a new TemplateLayoutResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *TemplateLayoutResponse) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *TemplateLayoutResponse) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *TemplateLayoutResponse) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.


### GetCategory

`func (o *TemplateLayoutResponse) GetCategory() string`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *TemplateLayoutResponse) GetCategoryOk() (*string, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *TemplateLayoutResponse) SetCategory(v string)`

SetCategory sets Category field to given value.

### HasCategory

`func (o *TemplateLayoutResponse) HasCategory() bool`

HasCategory returns a boolean if a field has been set.

### SetCategoryNil

`func (o *TemplateLayoutResponse) SetCategoryNil(b bool)`

 SetCategoryNil sets the value for Category to be an explicit nil

### UnsetCategory
`func (o *TemplateLayoutResponse) UnsetCategory()`

UnsetCategory ensures that no value is present for Category, not even an explicit nil
### GetGroups

`func (o *TemplateLayoutResponse) GetGroups() []TemplateGroupResponse`

GetGroups returns the Groups field if non-nil, zero value otherwise.

### GetGroupsOk

`func (o *TemplateLayoutResponse) GetGroupsOk() (*[]TemplateGroupResponse, bool)`

GetGroupsOk returns a tuple with the Groups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGroups

`func (o *TemplateLayoutResponse) SetGroups(v []TemplateGroupResponse)`

SetGroups sets Groups field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


