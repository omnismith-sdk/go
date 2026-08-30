# CreateAccessTokenRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** | Friendly human-readable label to identify the token purpose | 
**ExpiresAt** | **time.Time** | Expiration timestamp in ISO 8601 UTC format (e.g. 2026-12-31T23:59:59Z) | 

## Methods

### NewCreateAccessTokenRequest

`func NewCreateAccessTokenRequest(name string, expiresAt time.Time, ) *CreateAccessTokenRequest`

NewCreateAccessTokenRequest instantiates a new CreateAccessTokenRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateAccessTokenRequestWithDefaults

`func NewCreateAccessTokenRequestWithDefaults() *CreateAccessTokenRequest`

NewCreateAccessTokenRequestWithDefaults instantiates a new CreateAccessTokenRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreateAccessTokenRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateAccessTokenRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateAccessTokenRequest) SetName(v string)`

SetName sets Name field to given value.


### GetExpiresAt

`func (o *CreateAccessTokenRequest) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *CreateAccessTokenRequest) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *CreateAccessTokenRequest) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


