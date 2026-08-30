# MarketplaceBlueprintSummaryResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Unique blueprint UUID | [optional] 
**UserId** | Pointer to **string** | UUID of the publisher user | [optional] 
**Title** | Pointer to **string** | Blueprint display title | [optional] 
**Description** | Pointer to **string** | Detailed markdown description of the blueprint | [optional] 
**Metadata** | Pointer to [**MarketplaceBlueprintDetailResponseMetadata**](MarketplaceBlueprintDetailResponseMetadata.md) |  | [optional] 
**IsFeatured** | Pointer to **bool** | Whether the blueprint is featured in the marketplace | [optional] 
**CreatedAt** | Pointer to **time.Time** | Publish timestamp | [optional] 
**UpdatedAt** | Pointer to **time.Time** | Last update timestamp | [optional] 

## Methods

### NewMarketplaceBlueprintSummaryResponse

`func NewMarketplaceBlueprintSummaryResponse() *MarketplaceBlueprintSummaryResponse`

NewMarketplaceBlueprintSummaryResponse instantiates a new MarketplaceBlueprintSummaryResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMarketplaceBlueprintSummaryResponseWithDefaults

`func NewMarketplaceBlueprintSummaryResponseWithDefaults() *MarketplaceBlueprintSummaryResponse`

NewMarketplaceBlueprintSummaryResponseWithDefaults instantiates a new MarketplaceBlueprintSummaryResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *MarketplaceBlueprintSummaryResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *MarketplaceBlueprintSummaryResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *MarketplaceBlueprintSummaryResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *MarketplaceBlueprintSummaryResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetUserId

`func (o *MarketplaceBlueprintSummaryResponse) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *MarketplaceBlueprintSummaryResponse) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *MarketplaceBlueprintSummaryResponse) SetUserId(v string)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *MarketplaceBlueprintSummaryResponse) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetTitle

`func (o *MarketplaceBlueprintSummaryResponse) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *MarketplaceBlueprintSummaryResponse) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *MarketplaceBlueprintSummaryResponse) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *MarketplaceBlueprintSummaryResponse) HasTitle() bool`

HasTitle returns a boolean if a field has been set.

### GetDescription

`func (o *MarketplaceBlueprintSummaryResponse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *MarketplaceBlueprintSummaryResponse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *MarketplaceBlueprintSummaryResponse) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *MarketplaceBlueprintSummaryResponse) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetMetadata

`func (o *MarketplaceBlueprintSummaryResponse) GetMetadata() MarketplaceBlueprintDetailResponseMetadata`

GetMetadata returns the Metadata field if non-nil, zero value otherwise.

### GetMetadataOk

`func (o *MarketplaceBlueprintSummaryResponse) GetMetadataOk() (*MarketplaceBlueprintDetailResponseMetadata, bool)`

GetMetadataOk returns a tuple with the Metadata field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMetadata

`func (o *MarketplaceBlueprintSummaryResponse) SetMetadata(v MarketplaceBlueprintDetailResponseMetadata)`

SetMetadata sets Metadata field to given value.

### HasMetadata

`func (o *MarketplaceBlueprintSummaryResponse) HasMetadata() bool`

HasMetadata returns a boolean if a field has been set.

### GetIsFeatured

`func (o *MarketplaceBlueprintSummaryResponse) GetIsFeatured() bool`

GetIsFeatured returns the IsFeatured field if non-nil, zero value otherwise.

### GetIsFeaturedOk

`func (o *MarketplaceBlueprintSummaryResponse) GetIsFeaturedOk() (*bool, bool)`

GetIsFeaturedOk returns a tuple with the IsFeatured field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsFeatured

`func (o *MarketplaceBlueprintSummaryResponse) SetIsFeatured(v bool)`

SetIsFeatured sets IsFeatured field to given value.

### HasIsFeatured

`func (o *MarketplaceBlueprintSummaryResponse) HasIsFeatured() bool`

HasIsFeatured returns a boolean if a field has been set.

### GetCreatedAt

`func (o *MarketplaceBlueprintSummaryResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *MarketplaceBlueprintSummaryResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *MarketplaceBlueprintSummaryResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *MarketplaceBlueprintSummaryResponse) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *MarketplaceBlueprintSummaryResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *MarketplaceBlueprintSummaryResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *MarketplaceBlueprintSummaryResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *MarketplaceBlueprintSummaryResponse) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


