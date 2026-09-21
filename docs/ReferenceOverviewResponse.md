# ReferenceOverviewResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TargetTemplateId** | **string** | UUID of target template | 
**TargetTemplateSlug** | Pointer to **NullableString** | Slug identifier of target template | [optional] 
**TargetAttributeId** | **string** | UUID of target display attribute | 
**TargetAttributeSlug** | Pointer to **NullableString** | Slug identifier of target display attribute | [optional] 

## Methods

### NewReferenceOverviewResponse

`func NewReferenceOverviewResponse(targetTemplateId string, targetAttributeId string, ) *ReferenceOverviewResponse`

NewReferenceOverviewResponse instantiates a new ReferenceOverviewResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReferenceOverviewResponseWithDefaults

`func NewReferenceOverviewResponseWithDefaults() *ReferenceOverviewResponse`

NewReferenceOverviewResponseWithDefaults instantiates a new ReferenceOverviewResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTargetTemplateId

`func (o *ReferenceOverviewResponse) GetTargetTemplateId() string`

GetTargetTemplateId returns the TargetTemplateId field if non-nil, zero value otherwise.

### GetTargetTemplateIdOk

`func (o *ReferenceOverviewResponse) GetTargetTemplateIdOk() (*string, bool)`

GetTargetTemplateIdOk returns a tuple with the TargetTemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetTemplateId

`func (o *ReferenceOverviewResponse) SetTargetTemplateId(v string)`

SetTargetTemplateId sets TargetTemplateId field to given value.


### GetTargetTemplateSlug

`func (o *ReferenceOverviewResponse) GetTargetTemplateSlug() string`

GetTargetTemplateSlug returns the TargetTemplateSlug field if non-nil, zero value otherwise.

### GetTargetTemplateSlugOk

`func (o *ReferenceOverviewResponse) GetTargetTemplateSlugOk() (*string, bool)`

GetTargetTemplateSlugOk returns a tuple with the TargetTemplateSlug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetTemplateSlug

`func (o *ReferenceOverviewResponse) SetTargetTemplateSlug(v string)`

SetTargetTemplateSlug sets TargetTemplateSlug field to given value.

### HasTargetTemplateSlug

`func (o *ReferenceOverviewResponse) HasTargetTemplateSlug() bool`

HasTargetTemplateSlug returns a boolean if a field has been set.

### SetTargetTemplateSlugNil

`func (o *ReferenceOverviewResponse) SetTargetTemplateSlugNil(b bool)`

 SetTargetTemplateSlugNil sets the value for TargetTemplateSlug to be an explicit nil

### UnsetTargetTemplateSlug
`func (o *ReferenceOverviewResponse) UnsetTargetTemplateSlug()`

UnsetTargetTemplateSlug ensures that no value is present for TargetTemplateSlug, not even an explicit nil
### GetTargetAttributeId

`func (o *ReferenceOverviewResponse) GetTargetAttributeId() string`

GetTargetAttributeId returns the TargetAttributeId field if non-nil, zero value otherwise.

### GetTargetAttributeIdOk

`func (o *ReferenceOverviewResponse) GetTargetAttributeIdOk() (*string, bool)`

GetTargetAttributeIdOk returns a tuple with the TargetAttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetAttributeId

`func (o *ReferenceOverviewResponse) SetTargetAttributeId(v string)`

SetTargetAttributeId sets TargetAttributeId field to given value.


### GetTargetAttributeSlug

`func (o *ReferenceOverviewResponse) GetTargetAttributeSlug() string`

GetTargetAttributeSlug returns the TargetAttributeSlug field if non-nil, zero value otherwise.

### GetTargetAttributeSlugOk

`func (o *ReferenceOverviewResponse) GetTargetAttributeSlugOk() (*string, bool)`

GetTargetAttributeSlugOk returns a tuple with the TargetAttributeSlug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetAttributeSlug

`func (o *ReferenceOverviewResponse) SetTargetAttributeSlug(v string)`

SetTargetAttributeSlug sets TargetAttributeSlug field to given value.

### HasTargetAttributeSlug

`func (o *ReferenceOverviewResponse) HasTargetAttributeSlug() bool`

HasTargetAttributeSlug returns a boolean if a field has been set.

### SetTargetAttributeSlugNil

`func (o *ReferenceOverviewResponse) SetTargetAttributeSlugNil(b bool)`

 SetTargetAttributeSlugNil sets the value for TargetAttributeSlug to be an explicit nil

### UnsetTargetAttributeSlug
`func (o *ReferenceOverviewResponse) UnsetTargetAttributeSlug()`

UnsetTargetAttributeSlug ensures that no value is present for TargetAttributeSlug, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


