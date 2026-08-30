# BiListTemplateRowsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**GlobalSearch** | Pointer to **NullableString** | Full-text query string searched across all string and text dimension attributes of the template | [optional] 
**Filters** | Pointer to [**[]BiListTemplateRowsRequestFiltersInner**](BiListTemplateRowsRequestFiltersInner.md) | List of structured attribute and metadata filter conditions | [optional] 

## Methods

### NewBiListTemplateRowsRequest

`func NewBiListTemplateRowsRequest() *BiListTemplateRowsRequest`

NewBiListTemplateRowsRequest instantiates a new BiListTemplateRowsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBiListTemplateRowsRequestWithDefaults

`func NewBiListTemplateRowsRequestWithDefaults() *BiListTemplateRowsRequest`

NewBiListTemplateRowsRequestWithDefaults instantiates a new BiListTemplateRowsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetGlobalSearch

`func (o *BiListTemplateRowsRequest) GetGlobalSearch() string`

GetGlobalSearch returns the GlobalSearch field if non-nil, zero value otherwise.

### GetGlobalSearchOk

`func (o *BiListTemplateRowsRequest) GetGlobalSearchOk() (*string, bool)`

GetGlobalSearchOk returns a tuple with the GlobalSearch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGlobalSearch

`func (o *BiListTemplateRowsRequest) SetGlobalSearch(v string)`

SetGlobalSearch sets GlobalSearch field to given value.

### HasGlobalSearch

`func (o *BiListTemplateRowsRequest) HasGlobalSearch() bool`

HasGlobalSearch returns a boolean if a field has been set.

### SetGlobalSearchNil

`func (o *BiListTemplateRowsRequest) SetGlobalSearchNil(b bool)`

 SetGlobalSearchNil sets the value for GlobalSearch to be an explicit nil

### UnsetGlobalSearch
`func (o *BiListTemplateRowsRequest) UnsetGlobalSearch()`

UnsetGlobalSearch ensures that no value is present for GlobalSearch, not even an explicit nil
### GetFilters

`func (o *BiListTemplateRowsRequest) GetFilters() []BiListTemplateRowsRequestFiltersInner`

GetFilters returns the Filters field if non-nil, zero value otherwise.

### GetFiltersOk

`func (o *BiListTemplateRowsRequest) GetFiltersOk() (*[]BiListTemplateRowsRequestFiltersInner, bool)`

GetFiltersOk returns a tuple with the Filters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilters

`func (o *BiListTemplateRowsRequest) SetFilters(v []BiListTemplateRowsRequestFiltersInner)`

SetFilters sets Filters field to given value.

### HasFilters

`func (o *BiListTemplateRowsRequest) HasFilters() bool`

HasFilters returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


