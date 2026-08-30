# RegisterUserRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Email** | **string** | User email address | 
**Password** | **string** | User password (min 8 chars) | 
**CaptchaToken** | Pointer to **NullableString** | CAPTCHA response token (required for anonymous/public signups) | [optional] 

## Methods

### NewRegisterUserRequest

`func NewRegisterUserRequest(email string, password string, ) *RegisterUserRequest`

NewRegisterUserRequest instantiates a new RegisterUserRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRegisterUserRequestWithDefaults

`func NewRegisterUserRequestWithDefaults() *RegisterUserRequest`

NewRegisterUserRequestWithDefaults instantiates a new RegisterUserRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEmail

`func (o *RegisterUserRequest) GetEmail() string`

GetEmail returns the Email field if non-nil, zero value otherwise.

### GetEmailOk

`func (o *RegisterUserRequest) GetEmailOk() (*string, bool)`

GetEmailOk returns a tuple with the Email field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEmail

`func (o *RegisterUserRequest) SetEmail(v string)`

SetEmail sets Email field to given value.


### GetPassword

`func (o *RegisterUserRequest) GetPassword() string`

GetPassword returns the Password field if non-nil, zero value otherwise.

### GetPasswordOk

`func (o *RegisterUserRequest) GetPasswordOk() (*string, bool)`

GetPasswordOk returns a tuple with the Password field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPassword

`func (o *RegisterUserRequest) SetPassword(v string)`

SetPassword sets Password field to given value.


### GetCaptchaToken

`func (o *RegisterUserRequest) GetCaptchaToken() string`

GetCaptchaToken returns the CaptchaToken field if non-nil, zero value otherwise.

### GetCaptchaTokenOk

`func (o *RegisterUserRequest) GetCaptchaTokenOk() (*string, bool)`

GetCaptchaTokenOk returns a tuple with the CaptchaToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCaptchaToken

`func (o *RegisterUserRequest) SetCaptchaToken(v string)`

SetCaptchaToken sets CaptchaToken field to given value.

### HasCaptchaToken

`func (o *RegisterUserRequest) HasCaptchaToken() bool`

HasCaptchaToken returns a boolean if a field has been set.

### SetCaptchaTokenNil

`func (o *RegisterUserRequest) SetCaptchaTokenNil(b bool)`

 SetCaptchaTokenNil sets the value for CaptchaToken to be an explicit nil

### UnsetCaptchaToken
`func (o *RegisterUserRequest) UnsetCaptchaToken()`

UnsetCaptchaToken ensures that no value is present for CaptchaToken, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


