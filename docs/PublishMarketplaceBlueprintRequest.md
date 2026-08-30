# PublishMarketplaceBlueprintRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | **string** | Public display title of the blueprint | 
**Description** | Pointer to **string** | Detailed markdown description explaining what schemas, attributes, and relationships are included in the blueprint | [optional] 
**Keywords** | Pointer to **[]string** | List of categorization tags and keywords for search indexing | [optional] 
**TemplateIds** | **[]string** | Array of entity template UUIDs from the current project to snapshot into the blueprint package | 
**Id** | Pointer to **NullableString** | Optional blueprint UUID when updating an existing published blueprint owned by the user | [optional] 

## Methods

### NewPublishMarketplaceBlueprintRequest

`func NewPublishMarketplaceBlueprintRequest(title string, templateIds []string, ) *PublishMarketplaceBlueprintRequest`

NewPublishMarketplaceBlueprintRequest instantiates a new PublishMarketplaceBlueprintRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPublishMarketplaceBlueprintRequestWithDefaults

`func NewPublishMarketplaceBlueprintRequestWithDefaults() *PublishMarketplaceBlueprintRequest`

NewPublishMarketplaceBlueprintRequestWithDefaults instantiates a new PublishMarketplaceBlueprintRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTitle

`func (o *PublishMarketplaceBlueprintRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *PublishMarketplaceBlueprintRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *PublishMarketplaceBlueprintRequest) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetDescription

`func (o *PublishMarketplaceBlueprintRequest) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *PublishMarketplaceBlueprintRequest) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *PublishMarketplaceBlueprintRequest) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *PublishMarketplaceBlueprintRequest) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetKeywords

`func (o *PublishMarketplaceBlueprintRequest) GetKeywords() []string`

GetKeywords returns the Keywords field if non-nil, zero value otherwise.

### GetKeywordsOk

`func (o *PublishMarketplaceBlueprintRequest) GetKeywordsOk() (*[]string, bool)`

GetKeywordsOk returns a tuple with the Keywords field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKeywords

`func (o *PublishMarketplaceBlueprintRequest) SetKeywords(v []string)`

SetKeywords sets Keywords field to given value.

### HasKeywords

`func (o *PublishMarketplaceBlueprintRequest) HasKeywords() bool`

HasKeywords returns a boolean if a field has been set.

### GetTemplateIds

`func (o *PublishMarketplaceBlueprintRequest) GetTemplateIds() []string`

GetTemplateIds returns the TemplateIds field if non-nil, zero value otherwise.

### GetTemplateIdsOk

`func (o *PublishMarketplaceBlueprintRequest) GetTemplateIdsOk() (*[]string, bool)`

GetTemplateIdsOk returns a tuple with the TemplateIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateIds

`func (o *PublishMarketplaceBlueprintRequest) SetTemplateIds(v []string)`

SetTemplateIds sets TemplateIds field to given value.


### GetId

`func (o *PublishMarketplaceBlueprintRequest) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *PublishMarketplaceBlueprintRequest) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *PublishMarketplaceBlueprintRequest) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *PublishMarketplaceBlueprintRequest) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *PublishMarketplaceBlueprintRequest) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *PublishMarketplaceBlueprintRequest) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


