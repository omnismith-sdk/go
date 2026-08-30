# GetJwks200ResponseKeysInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Kty** | Pointer to **string** | Key type family | [optional] 
**Use** | Pointer to **string** | Intended key usage | [optional] 
**Alg** | Pointer to **string** | Algorithm intended for use with the key | [optional] 
**Kid** | Pointer to **string** | Unique Key ID thumbprint | [optional] 
**N** | Pointer to **string** | Base64URL-encoded RSA public modulus | [optional] 
**E** | Pointer to **string** | Base64URL-encoded RSA public exponent | [optional] 

## Methods

### NewGetJwks200ResponseKeysInner

`func NewGetJwks200ResponseKeysInner() *GetJwks200ResponseKeysInner`

NewGetJwks200ResponseKeysInner instantiates a new GetJwks200ResponseKeysInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGetJwks200ResponseKeysInnerWithDefaults

`func NewGetJwks200ResponseKeysInnerWithDefaults() *GetJwks200ResponseKeysInner`

NewGetJwks200ResponseKeysInnerWithDefaults instantiates a new GetJwks200ResponseKeysInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKty

`func (o *GetJwks200ResponseKeysInner) GetKty() string`

GetKty returns the Kty field if non-nil, zero value otherwise.

### GetKtyOk

`func (o *GetJwks200ResponseKeysInner) GetKtyOk() (*string, bool)`

GetKtyOk returns a tuple with the Kty field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKty

`func (o *GetJwks200ResponseKeysInner) SetKty(v string)`

SetKty sets Kty field to given value.

### HasKty

`func (o *GetJwks200ResponseKeysInner) HasKty() bool`

HasKty returns a boolean if a field has been set.

### GetUse

`func (o *GetJwks200ResponseKeysInner) GetUse() string`

GetUse returns the Use field if non-nil, zero value otherwise.

### GetUseOk

`func (o *GetJwks200ResponseKeysInner) GetUseOk() (*string, bool)`

GetUseOk returns a tuple with the Use field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUse

`func (o *GetJwks200ResponseKeysInner) SetUse(v string)`

SetUse sets Use field to given value.

### HasUse

`func (o *GetJwks200ResponseKeysInner) HasUse() bool`

HasUse returns a boolean if a field has been set.

### GetAlg

`func (o *GetJwks200ResponseKeysInner) GetAlg() string`

GetAlg returns the Alg field if non-nil, zero value otherwise.

### GetAlgOk

`func (o *GetJwks200ResponseKeysInner) GetAlgOk() (*string, bool)`

GetAlgOk returns a tuple with the Alg field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAlg

`func (o *GetJwks200ResponseKeysInner) SetAlg(v string)`

SetAlg sets Alg field to given value.

### HasAlg

`func (o *GetJwks200ResponseKeysInner) HasAlg() bool`

HasAlg returns a boolean if a field has been set.

### GetKid

`func (o *GetJwks200ResponseKeysInner) GetKid() string`

GetKid returns the Kid field if non-nil, zero value otherwise.

### GetKidOk

`func (o *GetJwks200ResponseKeysInner) GetKidOk() (*string, bool)`

GetKidOk returns a tuple with the Kid field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKid

`func (o *GetJwks200ResponseKeysInner) SetKid(v string)`

SetKid sets Kid field to given value.

### HasKid

`func (o *GetJwks200ResponseKeysInner) HasKid() bool`

HasKid returns a boolean if a field has been set.

### GetN

`func (o *GetJwks200ResponseKeysInner) GetN() string`

GetN returns the N field if non-nil, zero value otherwise.

### GetNOk

`func (o *GetJwks200ResponseKeysInner) GetNOk() (*string, bool)`

GetNOk returns a tuple with the N field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetN

`func (o *GetJwks200ResponseKeysInner) SetN(v string)`

SetN sets N field to given value.

### HasN

`func (o *GetJwks200ResponseKeysInner) HasN() bool`

HasN returns a boolean if a field has been set.

### GetE

`func (o *GetJwks200ResponseKeysInner) GetE() string`

GetE returns the E field if non-nil, zero value otherwise.

### GetEOk

`func (o *GetJwks200ResponseKeysInner) GetEOk() (*string, bool)`

GetEOk returns a tuple with the E field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetE

`func (o *GetJwks200ResponseKeysInner) SetE(v string)`

SetE sets E field to given value.

### HasE

`func (o *GetJwks200ResponseKeysInner) HasE() bool`

HasE returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


