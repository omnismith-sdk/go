# BiListTemplateRowsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**GlobalSearch** | Pointer to **NullableString** | Full-text query string searched across all string and text dimension attributes of the template | [optional] 
**FilterGroups** | Pointer to [**[][]EntityFilter**]([]EntityFilter.md) | Filter groups: clauses inside a group are AND-ed, groups are OR-ed. &#x60;[]&#x60; applies no filter, &#x60;[[a, b]]&#x60; is &#x60;a AND b&#x60;, &#x60;[[a], [b, c]]&#x60; is &#x60;a OR (b AND c)&#x60;. Each clause is &#x60;{field, operator, value}&#x60; — see the &#x60;EntityFilter&#x60; schema for the shape. Unknown fields, operators that do not fit the field, malformed values, and reference paths into a template you cannot view are refused with 400/403. | [optional] 
**Fields** | Pointer to **[]string** | Optional list of attribute slugs, UUIDs, or standard fields to project (e.g. [\&quot;price\&quot;, \&quot;sku\&quot;]). Excludes non-requested dynamic attributes from column metadata and row outputs, skipping unnecessary attribute hydration and reducing tabular payload size. | [optional] 

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
### GetFilterGroups

`func (o *BiListTemplateRowsRequest) GetFilterGroups() [][]EntityFilter`

GetFilterGroups returns the FilterGroups field if non-nil, zero value otherwise.

### GetFilterGroupsOk

`func (o *BiListTemplateRowsRequest) GetFilterGroupsOk() (*[][]EntityFilter, bool)`

GetFilterGroupsOk returns a tuple with the FilterGroups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilterGroups

`func (o *BiListTemplateRowsRequest) SetFilterGroups(v [][]EntityFilter)`

SetFilterGroups sets FilterGroups field to given value.

### HasFilterGroups

`func (o *BiListTemplateRowsRequest) HasFilterGroups() bool`

HasFilterGroups returns a boolean if a field has been set.

### GetFields

`func (o *BiListTemplateRowsRequest) GetFields() []string`

GetFields returns the Fields field if non-nil, zero value otherwise.

### GetFieldsOk

`func (o *BiListTemplateRowsRequest) GetFieldsOk() (*[]string, bool)`

GetFieldsOk returns a tuple with the Fields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFields

`func (o *BiListTemplateRowsRequest) SetFields(v []string)`

SetFields sets Fields field to given value.

### HasFields

`func (o *BiListTemplateRowsRequest) HasFields() bool`

HasFields returns a boolean if a field has been set.

### SetFieldsNil

`func (o *BiListTemplateRowsRequest) SetFieldsNil(b bool)`

 SetFieldsNil sets the value for Fields to be an explicit nil

### UnsetFields
`func (o *BiListTemplateRowsRequest) UnsetFields()`

UnsetFields ensures that no value is present for Fields, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


