# ExportEntitiesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**GlobalSearch** | Pointer to **NullableString** | Full-text search query string across all string dimension attributes | [optional] 
**FilterGroups** | Pointer to [**[][]EntityFilter**]([]EntityFilter.md) | Filter groups: clauses inside a group are AND-ed, groups are OR-ed. &#x60;[]&#x60; applies no filter, &#x60;[[a, b]]&#x60; is &#x60;a AND b&#x60;, &#x60;[[a], [b, c]]&#x60; is &#x60;a OR (b AND c)&#x60;. | [optional] 

## Methods

### NewExportEntitiesRequest

`func NewExportEntitiesRequest() *ExportEntitiesRequest`

NewExportEntitiesRequest instantiates a new ExportEntitiesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExportEntitiesRequestWithDefaults

`func NewExportEntitiesRequestWithDefaults() *ExportEntitiesRequest`

NewExportEntitiesRequestWithDefaults instantiates a new ExportEntitiesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetGlobalSearch

`func (o *ExportEntitiesRequest) GetGlobalSearch() string`

GetGlobalSearch returns the GlobalSearch field if non-nil, zero value otherwise.

### GetGlobalSearchOk

`func (o *ExportEntitiesRequest) GetGlobalSearchOk() (*string, bool)`

GetGlobalSearchOk returns a tuple with the GlobalSearch field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGlobalSearch

`func (o *ExportEntitiesRequest) SetGlobalSearch(v string)`

SetGlobalSearch sets GlobalSearch field to given value.

### HasGlobalSearch

`func (o *ExportEntitiesRequest) HasGlobalSearch() bool`

HasGlobalSearch returns a boolean if a field has been set.

### SetGlobalSearchNil

`func (o *ExportEntitiesRequest) SetGlobalSearchNil(b bool)`

 SetGlobalSearchNil sets the value for GlobalSearch to be an explicit nil

### UnsetGlobalSearch
`func (o *ExportEntitiesRequest) UnsetGlobalSearch()`

UnsetGlobalSearch ensures that no value is present for GlobalSearch, not even an explicit nil
### GetFilterGroups

`func (o *ExportEntitiesRequest) GetFilterGroups() [][]EntityFilter`

GetFilterGroups returns the FilterGroups field if non-nil, zero value otherwise.

### GetFilterGroupsOk

`func (o *ExportEntitiesRequest) GetFilterGroupsOk() (*[][]EntityFilter, bool)`

GetFilterGroupsOk returns a tuple with the FilterGroups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilterGroups

`func (o *ExportEntitiesRequest) SetFilterGroups(v [][]EntityFilter)`

SetFilterGroups sets FilterGroups field to given value.

### HasFilterGroups

`func (o *ExportEntitiesRequest) HasFilterGroups() bool`

HasFilterGroups returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


