# GoogleLoginRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Credential** | **string** | Cryptographically signed Google ID token (JWT) issued by Google Identity Services SDK | 

## Methods

### NewGoogleLoginRequest

`func NewGoogleLoginRequest(credential string, ) *GoogleLoginRequest`

NewGoogleLoginRequest instantiates a new GoogleLoginRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewGoogleLoginRequestWithDefaults

`func NewGoogleLoginRequestWithDefaults() *GoogleLoginRequest`

NewGoogleLoginRequestWithDefaults instantiates a new GoogleLoginRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCredential

`func (o *GoogleLoginRequest) GetCredential() string`

GetCredential returns the Credential field if non-nil, zero value otherwise.

### GetCredentialOk

`func (o *GoogleLoginRequest) GetCredentialOk() (*string, bool)`

GetCredentialOk returns a tuple with the Credential field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCredential

`func (o *GoogleLoginRequest) SetCredential(v string)`

SetCredential sets Credential field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


