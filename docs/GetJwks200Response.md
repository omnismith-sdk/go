# GetJwks200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Keys** | Pointer to [**[]GetJwks200ResponseKeysInner**](GetJwks200ResponseKeysInner.md) | Array of public cryptographic key descriptors | [optional] 

## Methods

### NewGetJwks200Response

`func NewGetJwks200Response() *GetJwks200Response`

NewGetJwks200Response instantiates a new GetJwks200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetJwks200ResponseWithDefaults

`func NewGetJwks200ResponseWithDefaults() *GetJwks200Response`

NewGetJwks200ResponseWithDefaults instantiates a new GetJwks200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKeys

`func (o *GetJwks200Response) GetKeys() []GetJwks200ResponseKeysInner`

GetKeys returns the Keys field if non-nil, zero value otherwise.

### GetKeysOk

`func (o *GetJwks200Response) GetKeysOk() (*[]GetJwks200ResponseKeysInner, bool)`

GetKeysOk returns a tuple with the Keys field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKeys

`func (o *GetJwks200Response) SetKeys(v []GetJwks200ResponseKeysInner)`

SetKeys sets Keys field to given value.

### HasKeys

`func (o *GetJwks200Response) HasKeys() bool`

HasKeys returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


