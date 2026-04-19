# SearchEntitiesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**GlobalSearch** | Pointer to **NullableString** |  | [optional] 
**Filters** | Pointer to [**[]ExportEntitiesRequestFiltersInner**](ExportEntitiesRequestFiltersInner.md) |  | [optional] 

## Methods

### NewSearchEntitiesRequest

`func NewSearchEntitiesRequest() *SearchEntitiesRequest`

NewSearchEntitiesRequest instantiates a new SearchEntitiesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSearchEntitiesRequestWithDefaults

`func NewSearchEntitiesRequestWithDefaults() *SearchEntitiesRequest`

NewSearchEntitiesRequestWithDefaults instantiates a new SearchEntitiesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetGlobalSearch

`func (o *SearchEntitiesRequest) GetGlobalSearch() string`

GetGlobalSearch returns the GlobalSearch field if non-nil, zero value otherwise.

### GetGlobalSearchOk

`func (o *SearchEntitiesRequest) GetGlobalSearchOk() (*string, bool)`

GetGlobalSearchOk returns a tuple with the GlobalSearch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGlobalSearch

`func (o *SearchEntitiesRequest) SetGlobalSearch(v string)`

SetGlobalSearch sets GlobalSearch field to given value.

### HasGlobalSearch

`func (o *SearchEntitiesRequest) HasGlobalSearch() bool`

HasGlobalSearch returns a boolean if a field has been set.

### SetGlobalSearchNil

`func (o *SearchEntitiesRequest) SetGlobalSearchNil(b bool)`

 SetGlobalSearchNil sets the value for GlobalSearch to be an explicit nil

### UnsetGlobalSearch
`func (o *SearchEntitiesRequest) UnsetGlobalSearch()`

UnsetGlobalSearch ensures that no value is present for GlobalSearch, not even an explicit nil
### GetFilters

`func (o *SearchEntitiesRequest) GetFilters() []ExportEntitiesRequestFiltersInner`

GetFilters returns the Filters field if non-nil, zero value otherwise.

### GetFiltersOk

`func (o *SearchEntitiesRequest) GetFiltersOk() (*[]ExportEntitiesRequestFiltersInner, bool)`

GetFiltersOk returns a tuple with the Filters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilters

`func (o *SearchEntitiesRequest) SetFilters(v []ExportEntitiesRequestFiltersInner)`

SetFilters sets Filters field to given value.

### HasFilters

`func (o *SearchEntitiesRequest) HasFilters() bool`

HasFilters returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


