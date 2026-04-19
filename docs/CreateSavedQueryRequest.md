# CreateSavedQueryRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | **string** |  | 
**Name** | **string** |  | 
**GlobalSearch** | Pointer to **NullableString** |  | [optional] 
**Filters** | [**[]CreateSavedQueryRequestFiltersInner**](CreateSavedQueryRequestFiltersInner.md) |  | 

## Methods

### NewCreateSavedQueryRequest

`func NewCreateSavedQueryRequest(templateId string, name string, filters []CreateSavedQueryRequestFiltersInner, ) *CreateSavedQueryRequest`

NewCreateSavedQueryRequest instantiates a new CreateSavedQueryRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateSavedQueryRequestWithDefaults

`func NewCreateSavedQueryRequestWithDefaults() *CreateSavedQueryRequest`

NewCreateSavedQueryRequestWithDefaults instantiates a new CreateSavedQueryRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *CreateSavedQueryRequest) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *CreateSavedQueryRequest) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *CreateSavedQueryRequest) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.


### GetName

`func (o *CreateSavedQueryRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateSavedQueryRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateSavedQueryRequest) SetName(v string)`

SetName sets Name field to given value.


### GetGlobalSearch

`func (o *CreateSavedQueryRequest) GetGlobalSearch() string`

GetGlobalSearch returns the GlobalSearch field if non-nil, zero value otherwise.

### GetGlobalSearchOk

`func (o *CreateSavedQueryRequest) GetGlobalSearchOk() (*string, bool)`

GetGlobalSearchOk returns a tuple with the GlobalSearch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGlobalSearch

`func (o *CreateSavedQueryRequest) SetGlobalSearch(v string)`

SetGlobalSearch sets GlobalSearch field to given value.

### HasGlobalSearch

`func (o *CreateSavedQueryRequest) HasGlobalSearch() bool`

HasGlobalSearch returns a boolean if a field has been set.

### SetGlobalSearchNil

`func (o *CreateSavedQueryRequest) SetGlobalSearchNil(b bool)`

 SetGlobalSearchNil sets the value for GlobalSearch to be an explicit nil

### UnsetGlobalSearch
`func (o *CreateSavedQueryRequest) UnsetGlobalSearch()`

UnsetGlobalSearch ensures that no value is present for GlobalSearch, not even an explicit nil
### GetFilters

`func (o *CreateSavedQueryRequest) GetFilters() []CreateSavedQueryRequestFiltersInner`

GetFilters returns the Filters field if non-nil, zero value otherwise.

### GetFiltersOk

`func (o *CreateSavedQueryRequest) GetFiltersOk() (*[]CreateSavedQueryRequestFiltersInner, bool)`

GetFiltersOk returns a tuple with the Filters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilters

`func (o *CreateSavedQueryRequest) SetFilters(v []CreateSavedQueryRequestFiltersInner)`

SetFilters sets Filters field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


