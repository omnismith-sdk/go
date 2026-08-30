# SearchEntitiesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**GlobalSearch** | Pointer to **NullableString** | Full-text query string searched across all string and text dimension attributes of the template | [optional] 
**Filters** | Pointer to [**[]SearchEntitiesRequestFiltersInner**](SearchEntitiesRequestFiltersInner.md) | List of structured attribute and metadata filter conditions | [optional] 
**AttributeKey** | Pointer to **NullableString** | Format for attribute_values dictionary keys: \&quot;id\&quot; for UUIDs or \&quot;slug\&quot; for attribute slugs | [optional] 

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

`func (o *SearchEntitiesRequest) GetFilters() []SearchEntitiesRequestFiltersInner`

GetFilters returns the Filters field if non-nil, zero value otherwise.

### GetFiltersOk

`func (o *SearchEntitiesRequest) GetFiltersOk() (*[]SearchEntitiesRequestFiltersInner, bool)`

GetFiltersOk returns a tuple with the Filters field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilters

`func (o *SearchEntitiesRequest) SetFilters(v []SearchEntitiesRequestFiltersInner)`

SetFilters sets Filters field to given value.

### HasFilters

`func (o *SearchEntitiesRequest) HasFilters() bool`

HasFilters returns a boolean if a field has been set.

### GetAttributeKey

`func (o *SearchEntitiesRequest) GetAttributeKey() string`

GetAttributeKey returns the AttributeKey field if non-nil, zero value otherwise.

### GetAttributeKeyOk

`func (o *SearchEntitiesRequest) GetAttributeKeyOk() (*string, bool)`

GetAttributeKeyOk returns a tuple with the AttributeKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeKey

`func (o *SearchEntitiesRequest) SetAttributeKey(v string)`

SetAttributeKey sets AttributeKey field to given value.

### HasAttributeKey

`func (o *SearchEntitiesRequest) HasAttributeKey() bool`

HasAttributeKey returns a boolean if a field has been set.

### SetAttributeKeyNil

`func (o *SearchEntitiesRequest) SetAttributeKeyNil(b bool)`

 SetAttributeKeyNil sets the value for AttributeKey to be an explicit nil

### UnsetAttributeKey
`func (o *SearchEntitiesRequest) UnsetAttributeKey()`

UnsetAttributeKey ensures that no value is present for AttributeKey, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


