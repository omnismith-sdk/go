# ApproveOAuthAuthorization200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Code** | Pointer to **string** | Single-use authorization code | [optional] 
**RedirectUri** | Pointer to **string** | Client redirection URI | [optional] 
**CallbackUrl** | Pointer to **string** | Complete redirection callback URL with code and state parameters | [optional] 
**State** | Pointer to **NullableString** | Echoed client state parameter | [optional] 

## Methods

### NewApproveOAuthAuthorization200Response

`func NewApproveOAuthAuthorization200Response() *ApproveOAuthAuthorization200Response`

NewApproveOAuthAuthorization200Response instantiates a new ApproveOAuthAuthorization200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewApproveOAuthAuthorization200ResponseWithDefaults

`func NewApproveOAuthAuthorization200ResponseWithDefaults() *ApproveOAuthAuthorization200Response`

NewApproveOAuthAuthorization200ResponseWithDefaults instantiates a new ApproveOAuthAuthorization200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCode

`func (o *ApproveOAuthAuthorization200Response) GetCode() string`

GetCode returns the Code field if non-nil, zero value otherwise.

### GetCodeOk

`func (o *ApproveOAuthAuthorization200Response) GetCodeOk() (*string, bool)`

GetCodeOk returns a tuple with the Code field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCode

`func (o *ApproveOAuthAuthorization200Response) SetCode(v string)`

SetCode sets Code field to given value.

### HasCode

`func (o *ApproveOAuthAuthorization200Response) HasCode() bool`

HasCode returns a boolean if a field has been set.

### GetRedirectUri

`func (o *ApproveOAuthAuthorization200Response) GetRedirectUri() string`

GetRedirectUri returns the RedirectUri field if non-nil, zero value otherwise.

### GetRedirectUriOk

`func (o *ApproveOAuthAuthorization200Response) GetRedirectUriOk() (*string, bool)`

GetRedirectUriOk returns a tuple with the RedirectUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRedirectUri

`func (o *ApproveOAuthAuthorization200Response) SetRedirectUri(v string)`

SetRedirectUri sets RedirectUri field to given value.

### HasRedirectUri

`func (o *ApproveOAuthAuthorization200Response) HasRedirectUri() bool`

HasRedirectUri returns a boolean if a field has been set.

### GetCallbackUrl

`func (o *ApproveOAuthAuthorization200Response) GetCallbackUrl() string`

GetCallbackUrl returns the CallbackUrl field if non-nil, zero value otherwise.

### GetCallbackUrlOk

`func (o *ApproveOAuthAuthorization200Response) GetCallbackUrlOk() (*string, bool)`

GetCallbackUrlOk returns a tuple with the CallbackUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCallbackUrl

`func (o *ApproveOAuthAuthorization200Response) SetCallbackUrl(v string)`

SetCallbackUrl sets CallbackUrl field to given value.

### HasCallbackUrl

`func (o *ApproveOAuthAuthorization200Response) HasCallbackUrl() bool`

HasCallbackUrl returns a boolean if a field has been set.

### GetState

`func (o *ApproveOAuthAuthorization200Response) GetState() string`

GetState returns the State field if non-nil, zero value otherwise.

### GetStateOk

`func (o *ApproveOAuthAuthorization200Response) GetStateOk() (*string, bool)`

GetStateOk returns a tuple with the State field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetState

`func (o *ApproveOAuthAuthorization200Response) SetState(v string)`

SetState sets State field to given value.

### HasState

`func (o *ApproveOAuthAuthorization200Response) HasState() bool`

HasState returns a boolean if a field has been set.

### SetStateNil

`func (o *ApproveOAuthAuthorization200Response) SetStateNil(b bool)`

 SetStateNil sets the value for State to be an explicit nil

### UnsetState
`func (o *ApproveOAuthAuthorization200Response) UnsetState()`

UnsetState ensures that no value is present for State, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


