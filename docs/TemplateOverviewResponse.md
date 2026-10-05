# TemplateOverviewResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Template UUID | 
**Slug** | Pointer to **NullableString** | Unique template slug identifier | [optional] 
**Name** | **string** | Human-readable template name | 
**Description** | Pointer to **NullableString** | Template description | [optional] 
**Attributes** | [**[]TemplateAttributeOverviewResponse**](TemplateAttributeOverviewResponse.md) | Ordered list of attributes belonging to this template | 
**Rules** | [**[]EntityRuleOverviewResponse**](EntityRuleOverviewResponse.md) | Business validation rules enforced for this template | 
**Actions** | [**[]EntityActionOverviewResponse**](EntityActionOverviewResponse.md) | Executable workflow actions and transitions for records of this template | 
**InboundEndpoints** | [**[]InboundEndpointOverviewResponse**](InboundEndpointOverviewResponse.md) | Public URLs through which outside systems write records into this template. Empty when the caller cannot view inbound endpoints. | 

## Methods

### NewTemplateOverviewResponse

`func NewTemplateOverviewResponse(id string, name string, attributes []TemplateAttributeOverviewResponse, rules []EntityRuleOverviewResponse, actions []EntityActionOverviewResponse, inboundEndpoints []InboundEndpointOverviewResponse, ) *TemplateOverviewResponse`

NewTemplateOverviewResponse instantiates a new TemplateOverviewResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTemplateOverviewResponseWithDefaults

`func NewTemplateOverviewResponseWithDefaults() *TemplateOverviewResponse`

NewTemplateOverviewResponseWithDefaults instantiates a new TemplateOverviewResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *TemplateOverviewResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *TemplateOverviewResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *TemplateOverviewResponse) SetId(v string)`

SetId sets Id field to given value.


### GetSlug

`func (o *TemplateOverviewResponse) GetSlug() string`

GetSlug returns the Slug field if non-nil, zero value otherwise.

### GetSlugOk

`func (o *TemplateOverviewResponse) GetSlugOk() (*string, bool)`

GetSlugOk returns a tuple with the Slug field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSlug

`func (o *TemplateOverviewResponse) SetSlug(v string)`

SetSlug sets Slug field to given value.

### HasSlug

`func (o *TemplateOverviewResponse) HasSlug() bool`

HasSlug returns a boolean if a field has been set.

### SetSlugNil

`func (o *TemplateOverviewResponse) SetSlugNil(b bool)`

 SetSlugNil sets the value for Slug to be an explicit nil

### UnsetSlug
`func (o *TemplateOverviewResponse) UnsetSlug()`

UnsetSlug ensures that no value is present for Slug, not even an explicit nil
### GetName

`func (o *TemplateOverviewResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *TemplateOverviewResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *TemplateOverviewResponse) SetName(v string)`

SetName sets Name field to given value.


### GetDescription

`func (o *TemplateOverviewResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *TemplateOverviewResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *TemplateOverviewResponse) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *TemplateOverviewResponse) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### SetDescriptionNil

`func (o *TemplateOverviewResponse) SetDescriptionNil(b bool)`

 SetDescriptionNil sets the value for Description to be an explicit nil

### UnsetDescription
`func (o *TemplateOverviewResponse) UnsetDescription()`

UnsetDescription ensures that no value is present for Description, not even an explicit nil
### GetAttributes

`func (o *TemplateOverviewResponse) GetAttributes() []TemplateAttributeOverviewResponse`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *TemplateOverviewResponse) GetAttributesOk() (*[]TemplateAttributeOverviewResponse, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *TemplateOverviewResponse) SetAttributes(v []TemplateAttributeOverviewResponse)`

SetAttributes sets Attributes field to given value.


### GetRules

`func (o *TemplateOverviewResponse) GetRules() []EntityRuleOverviewResponse`

GetRules returns the Rules field if non-nil, zero value otherwise.

### GetRulesOk

`func (o *TemplateOverviewResponse) GetRulesOk() (*[]EntityRuleOverviewResponse, bool)`

GetRulesOk returns a tuple with the Rules field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRules

`func (o *TemplateOverviewResponse) SetRules(v []EntityRuleOverviewResponse)`

SetRules sets Rules field to given value.


### GetActions

`func (o *TemplateOverviewResponse) GetActions() []EntityActionOverviewResponse`

GetActions returns the Actions field if non-nil, zero value otherwise.

### GetActionsOk

`func (o *TemplateOverviewResponse) GetActionsOk() (*[]EntityActionOverviewResponse, bool)`

GetActionsOk returns a tuple with the Actions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActions

`func (o *TemplateOverviewResponse) SetActions(v []EntityActionOverviewResponse)`

SetActions sets Actions field to given value.


### GetInboundEndpoints

`func (o *TemplateOverviewResponse) GetInboundEndpoints() []InboundEndpointOverviewResponse`

GetInboundEndpoints returns the InboundEndpoints field if non-nil, zero value otherwise.

### GetInboundEndpointsOk

`func (o *TemplateOverviewResponse) GetInboundEndpointsOk() (*[]InboundEndpointOverviewResponse, bool)`

GetInboundEndpointsOk returns a tuple with the InboundEndpoints field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInboundEndpoints

`func (o *TemplateOverviewResponse) SetInboundEndpoints(v []InboundEndpointOverviewResponse)`

SetInboundEndpoints sets InboundEndpoints field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


