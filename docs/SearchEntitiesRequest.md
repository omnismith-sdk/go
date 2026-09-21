# SearchEntitiesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**GlobalSearch** | Pointer to **NullableString** | Full-text and substring query string, matched across all string and text dimension attributes of the template | [optional] 
**FilterGroups** | Pointer to [**[][]EntityFilter**]([]EntityFilter.md) | Filter groups: clauses inside a group are AND-ed, groups are OR-ed. &#x60;[]&#x60; applies no filter, &#x60;[[a, b]]&#x60; is &#x60;a AND b&#x60;, &#x60;[[a], [b, c]]&#x60; is &#x60;a OR (b AND c)&#x60;. Each clause is &#x60;{field, operator, value}&#x60; — see the &#x60;EntityFilter&#x60; schema for the shape. Unknown fields, operators that do not fit the field, malformed values, and reference paths into a template you cannot view are refused with 400/403. | [optional] 
**Verbose** | Pointer to **bool** | When true, each record&#39;s attribute_values is an array of EntityAttributeValue items (attribute id, slug, raw value, resolved custom_value, reference_entity_id). When false (default), attribute_values is a compact object mapping attribute slug to display value, with the ids behind list, reference and file labels in list_item_ids, reference_entity_ids and file_ids. | [optional] [default to false]
**Fields** | Pointer to **[]string** | Optional list of attribute slugs or UUIDs to project, e.g. [\&quot;title\&quot;, \&quot;status\&quot;]. Standard fields (id, template_id, template_slug, created_at, updated_at) are always included and do not need to be listed. When specified, database queries only hydrate the requested attributes, drastically reducing response payload size and execution latency. If omitted, all attributes defined on the template are returned. | [optional] 

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
### GetFilterGroups

`func (o *SearchEntitiesRequest) GetFilterGroups() [][]EntityFilter`

GetFilterGroups returns the FilterGroups field if non-nil, zero value otherwise.

### GetFilterGroupsOk

`func (o *SearchEntitiesRequest) GetFilterGroupsOk() (*[][]EntityFilter, bool)`

GetFilterGroupsOk returns a tuple with the FilterGroups field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilterGroups

`func (o *SearchEntitiesRequest) SetFilterGroups(v [][]EntityFilter)`

SetFilterGroups sets FilterGroups field to given value.

### HasFilterGroups

`func (o *SearchEntitiesRequest) HasFilterGroups() bool`

HasFilterGroups returns a boolean if a field has been set.

### GetVerbose

`func (o *SearchEntitiesRequest) GetVerbose() bool`

GetVerbose returns the Verbose field if non-nil, zero value otherwise.

### GetVerboseOk

`func (o *SearchEntitiesRequest) GetVerboseOk() (*bool, bool)`

GetVerboseOk returns a tuple with the Verbose field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVerbose

`func (o *SearchEntitiesRequest) SetVerbose(v bool)`

SetVerbose sets Verbose field to given value.

### HasVerbose

`func (o *SearchEntitiesRequest) HasVerbose() bool`

HasVerbose returns a boolean if a field has been set.

### GetFields

`func (o *SearchEntitiesRequest) GetFields() []string`

GetFields returns the Fields field if non-nil, zero value otherwise.

### GetFieldsOk

`func (o *SearchEntitiesRequest) GetFieldsOk() (*[]string, bool)`

GetFieldsOk returns a tuple with the Fields field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFields

`func (o *SearchEntitiesRequest) SetFields(v []string)`

SetFields sets Fields field to given value.

### HasFields

`func (o *SearchEntitiesRequest) HasFields() bool`

HasFields returns a boolean if a field has been set.

### SetFieldsNil

`func (o *SearchEntitiesRequest) SetFieldsNil(b bool)`

 SetFieldsNil sets the value for Fields to be an explicit nil

### UnsetFields
`func (o *SearchEntitiesRequest) UnsetFields()`

UnsetFields ensures that no value is present for Fields, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


