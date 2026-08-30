# MarketplaceBlueprintDetailResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Unique blueprint UUID | [optional] 
**UserId** | Pointer to **string** | UUID of the publisher user | [optional] 
**Title** | Pointer to **string** | Blueprint display title | [optional] 
**Description** | Pointer to **string** | Detailed markdown description of the blueprint | [optional] 
**Metadata** | Pointer to [**MarketplaceBlueprintDetailResponseMetadata**](MarketplaceBlueprintDetailResponseMetadata.md) |  | [optional] 
**Blueprint** | Pointer to **map[string]interface{}** | JSONB serialized blueprint payload containing templates, attributes, and optional demo entities | [optional] 
**IsFeatured** | Pointer to **bool** | Whether the blueprint is featured in the marketplace | [optional] 
**CreatedAt** | Pointer to **time.Time** | Publish timestamp | [optional] 
**UpdatedAt** | Pointer to **time.Time** | Last update timestamp | [optional] 

## Methods

### NewMarketplaceBlueprintDetailResponse

`func NewMarketplaceBlueprintDetailResponse() *MarketplaceBlueprintDetailResponse`

NewMarketplaceBlueprintDetailResponse instantiates a new MarketplaceBlueprintDetailResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMarketplaceBlueprintDetailResponseWithDefaults

`func NewMarketplaceBlueprintDetailResponseWithDefaults() *MarketplaceBlueprintDetailResponse`

NewMarketplaceBlueprintDetailResponseWithDefaults instantiates a new MarketplaceBlueprintDetailResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *MarketplaceBlueprintDetailResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *MarketplaceBlueprintDetailResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *MarketplaceBlueprintDetailResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *MarketplaceBlueprintDetailResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetUserId

`func (o *MarketplaceBlueprintDetailResponse) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *MarketplaceBlueprintDetailResponse) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *MarketplaceBlueprintDetailResponse) SetUserId(v string)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *MarketplaceBlueprintDetailResponse) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetTitle

`func (o *MarketplaceBlueprintDetailResponse) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *MarketplaceBlueprintDetailResponse) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *MarketplaceBlueprintDetailResponse) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *MarketplaceBlueprintDetailResponse) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetDescription

`func (o *MarketplaceBlueprintDetailResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *MarketplaceBlueprintDetailResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *MarketplaceBlueprintDetailResponse) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *MarketplaceBlueprintDetailResponse) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetMetadata

`func (o *MarketplaceBlueprintDetailResponse) GetMetadata() MarketplaceBlueprintDetailResponseMetadata`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *MarketplaceBlueprintDetailResponse) GetMetadataOk() (*MarketplaceBlueprintDetailResponseMetadata, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *MarketplaceBlueprintDetailResponse) SetMetadata(v MarketplaceBlueprintDetailResponseMetadata)`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *MarketplaceBlueprintDetailResponse) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.

### GetBlueprint

`func (o *MarketplaceBlueprintDetailResponse) GetBlueprint() map[string]interface{}`

GetBlueprint returns the Blueprint field if non-nil, zero value otherwise.

### GetBlueprintOk

`func (o *MarketplaceBlueprintDetailResponse) GetBlueprintOk() (*map[string]interface{}, bool)`

GetBlueprintOk returns a tuple with the Blueprint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBlueprint

`func (o *MarketplaceBlueprintDetailResponse) SetBlueprint(v map[string]interface{})`

SetBlueprint sets Blueprint field to given value.

### HasBlueprint

`func (o *MarketplaceBlueprintDetailResponse) HasBlueprint() bool`

HasBlueprint returns a boolean if a field has been set.

### GetIsFeatured

`func (o *MarketplaceBlueprintDetailResponse) GetIsFeatured() bool`

GetIsFeatured returns the IsFeatured field if non-nil, zero value otherwise.

### GetIsFeaturedOk

`func (o *MarketplaceBlueprintDetailResponse) GetIsFeaturedOk() (*bool, bool)`

GetIsFeaturedOk returns a tuple with the IsFeatured field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsFeatured

`func (o *MarketplaceBlueprintDetailResponse) SetIsFeatured(v bool)`

SetIsFeatured sets IsFeatured field to given value.

### HasIsFeatured

`func (o *MarketplaceBlueprintDetailResponse) HasIsFeatured() bool`

HasIsFeatured returns a boolean if a field has been set.

### GetCreatedAt

`func (o *MarketplaceBlueprintDetailResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *MarketplaceBlueprintDetailResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *MarketplaceBlueprintDetailResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *MarketplaceBlueprintDetailResponse) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *MarketplaceBlueprintDetailResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *MarketplaceBlueprintDetailResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *MarketplaceBlueprintDetailResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *MarketplaceBlueprintDetailResponse) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


