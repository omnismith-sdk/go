# ListAccessTokens200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | Pointer to [**[]AccessTokenResponse**](AccessTokenResponse.md) |  | [optional] 
**Meta** | Pointer to **map[string]interface{}** |  | [optional] 

## Methods

### NewListAccessTokens200Response

`func NewListAccessTokens200Response() *ListAccessTokens200Response`

NewListAccessTokens200Response instantiates a new ListAccessTokens200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListAccessTokens200ResponseWithDefaults

`func NewListAccessTokens200ResponseWithDefaults() *ListAccessTokens200Response`

NewListAccessTokens200ResponseWithDefaults instantiates a new ListAccessTokens200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *ListAccessTokens200Response) GetData() []AccessTokenResponse`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ListAccessTokens200Response) GetDataOk() (*[]AccessTokenResponse, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ListAccessTokens200Response) SetData(v []AccessTokenResponse)`

SetData sets Data field to given value.

### HasData

`func (o *ListAccessTokens200Response) HasData() bool`

HasData returns a boolean if a field has been set.

### GetMeta

`func (o *ListAccessTokens200Response) GetMeta() map[string]interface{}`

GetMeta returns the Meta field if non-nil, zero value otherwise.

### GetMetaOk

`func (o *ListAccessTokens200Response) GetMetaOk() (*map[string]interface{}, bool)`

GetMetaOk returns a tuple with the Meta field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMeta

`func (o *ListAccessTokens200Response) SetMeta(v map[string]interface{})`

SetMeta sets Meta field to given value.

### HasMeta

`func (o *ListAccessTokens200Response) HasMeta() bool`

HasMeta returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


