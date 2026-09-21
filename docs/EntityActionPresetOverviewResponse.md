# EntityActionPresetOverviewResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AttributeId** | **string** | Attribute UUID to set | 
**AttributeSlug** | Pointer to **NullableString** | Attribute slug identifier | [optional] 
**Value** | **string** | Value to write silently | 

## Methods

### NewEntityActionPresetOverviewResponse

`func NewEntityActionPresetOverviewResponse(attributeId string, value string, ) *EntityActionPresetOverviewResponse`

NewEntityActionPresetOverviewResponse instantiates a new EntityActionPresetOverviewResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEntityActionPresetOverviewResponseWithDefaults

`func NewEntityActionPresetOverviewResponseWithDefaults() *EntityActionPresetOverviewResponse`

NewEntityActionPresetOverviewResponseWithDefaults instantiates a new EntityActionPresetOverviewResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributeId

`func (o *EntityActionPresetOverviewResponse) GetAttributeId() string`

GetAttributeId returns the AttributeId field if non-nil, zero value otherwise.

### GetAttributeIdOk

`func (o *EntityActionPresetOverviewResponse) GetAttributeIdOk() (*string, bool)`

GetAttributeIdOk returns a tuple with the AttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeId

`func (o *EntityActionPresetOverviewResponse) SetAttributeId(v string)`

SetAttributeId sets AttributeId field to given value.


### GetAttributeSlug

`func (o *EntityActionPresetOverviewResponse) GetAttributeSlug() string`

GetAttributeSlug returns the AttributeSlug field if non-nil, zero value otherwise.

### GetAttributeSlugOk

`func (o *EntityActionPresetOverviewResponse) GetAttributeSlugOk() (*string, bool)`

GetAttributeSlugOk returns a tuple with the AttributeSlug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributeSlug

`func (o *EntityActionPresetOverviewResponse) SetAttributeSlug(v string)`

SetAttributeSlug sets AttributeSlug field to given value.

### HasAttributeSlug

`func (o *EntityActionPresetOverviewResponse) HasAttributeSlug() bool`

HasAttributeSlug returns a boolean if a field has been set.

### SetAttributeSlugNil

`func (o *EntityActionPresetOverviewResponse) SetAttributeSlugNil(b bool)`

 SetAttributeSlugNil sets the value for AttributeSlug to be an explicit nil

### UnsetAttributeSlug
`func (o *EntityActionPresetOverviewResponse) UnsetAttributeSlug()`

UnsetAttributeSlug ensures that no value is present for AttributeSlug, not even an explicit nil
### GetValue

`func (o *EntityActionPresetOverviewResponse) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *EntityActionPresetOverviewResponse) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *EntityActionPresetOverviewResponse) SetValue(v string)`

SetValue sets Value field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


