# SemanticSearchResultItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Entity** | Pointer to [**EntityResponse**](EntityResponse.md) |  | [optional] 
**SimilarityScore** | Pointer to **float32** | Cosine similarity score (0.0 to 1.0, where 1.0 is exact match) | [optional] 

## Methods

### NewSemanticSearchResultItem

`func NewSemanticSearchResultItem() *SemanticSearchResultItem`

NewSemanticSearchResultItem instantiates a new SemanticSearchResultItem object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSemanticSearchResultItemWithDefaults

`func NewSemanticSearchResultItemWithDefaults() *SemanticSearchResultItem`

NewSemanticSearchResultItemWithDefaults instantiates a new SemanticSearchResultItem object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEntity

`func (o *SemanticSearchResultItem) GetEntity() EntityResponse`

GetEntity returns the Entity field if non-nil, zero value otherwise.

### GetEntityOk

`func (o *SemanticSearchResultItem) GetEntityOk() (*EntityResponse, bool)`

GetEntityOk returns a tuple with the Entity field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntity

`func (o *SemanticSearchResultItem) SetEntity(v EntityResponse)`

SetEntity sets Entity field to given value.

### HasEntity

`func (o *SemanticSearchResultItem) HasEntity() bool`

HasEntity returns a boolean if a field has been set.

### GetSimilarityScore

`func (o *SemanticSearchResultItem) GetSimilarityScore() float32`

GetSimilarityScore returns the SimilarityScore field if non-nil, zero value otherwise.

### GetSimilarityScoreOk

`func (o *SemanticSearchResultItem) GetSimilarityScoreOk() (*float32, bool)`

GetSimilarityScoreOk returns a tuple with the SimilarityScore field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSimilarityScore

`func (o *SemanticSearchResultItem) SetSimilarityScore(v float32)`

SetSimilarityScore sets SimilarityScore field to given value.

### HasSimilarityScore

`func (o *SemanticSearchResultItem) HasSimilarityScore() bool`

HasSimilarityScore returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


