# CreateNotificationChannelRequestCredentials

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**BotToken** | Pointer to **string** | Telegram bot token from BotFather | [optional] 
**Url** | Pointer to **string** | Webhook destination URL | [optional] 
**AuthType** | Pointer to **string** | Webhook HTTP authorization scheme | [optional] 
**Token** | Pointer to **string** | Bearer authentication token for webhook | [optional] 
**Username** | Pointer to **string** | Basic auth username for webhook | [optional] 
**Password** | Pointer to **string** | Basic auth password for webhook | [optional] 
**Headers** | Pointer to **map[string]string** | Custom HTTP header key-value pairs to send with webhook POST requests | [optional] 

## Methods

### NewCreateNotificationChannelRequestCredentials

`func NewCreateNotificationChannelRequestCredentials() *CreateNotificationChannelRequestCredentials`

NewCreateNotificationChannelRequestCredentials instantiates a new CreateNotificationChannelRequestCredentials object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateNotificationChannelRequestCredentialsWithDefaults

`func NewCreateNotificationChannelRequestCredentialsWithDefaults() *CreateNotificationChannelRequestCredentials`

NewCreateNotificationChannelRequestCredentialsWithDefaults instantiates a new CreateNotificationChannelRequestCredentials object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetBotToken

`func (o *CreateNotificationChannelRequestCredentials) GetBotToken() string`

GetBotToken returns the BotToken field if non-nil, zero value otherwise.

### GetBotTokenOk

`func (o *CreateNotificationChannelRequestCredentials) GetBotTokenOk() (*string, bool)`

GetBotTokenOk returns a tuple with the BotToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBotToken

`func (o *CreateNotificationChannelRequestCredentials) SetBotToken(v string)`

SetBotToken sets BotToken field to given value.

### HasBotToken

`func (o *CreateNotificationChannelRequestCredentials) HasBotToken() bool`

HasBotToken returns a boolean if a field has been set.

### GetUrl

`func (o *CreateNotificationChannelRequestCredentials) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *CreateNotificationChannelRequestCredentials) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *CreateNotificationChannelRequestCredentials) SetUrl(v string)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *CreateNotificationChannelRequestCredentials) HasUrl() bool`

HasUrl returns a boolean if a field has been set.

### GetAuthType

`func (o *CreateNotificationChannelRequestCredentials) GetAuthType() string`

GetAuthType returns the AuthType field if non-nil, zero value otherwise.

### GetAuthTypeOk

`func (o *CreateNotificationChannelRequestCredentials) GetAuthTypeOk() (*string, bool)`

GetAuthTypeOk returns a tuple with the AuthType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthType

`func (o *CreateNotificationChannelRequestCredentials) SetAuthType(v string)`

SetAuthType sets AuthType field to given value.

### HasAuthType

`func (o *CreateNotificationChannelRequestCredentials) HasAuthType() bool`

HasAuthType returns a boolean if a field has been set.

### GetToken

`func (o *CreateNotificationChannelRequestCredentials) GetToken() string`

GetToken returns the Token field if non-nil, zero value otherwise.

### GetTokenOk

`func (o *CreateNotificationChannelRequestCredentials) GetTokenOk() (*string, bool)`

GetTokenOk returns a tuple with the Token field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetToken

`func (o *CreateNotificationChannelRequestCredentials) SetToken(v string)`

SetToken sets Token field to given value.

### HasToken

`func (o *CreateNotificationChannelRequestCredentials) HasToken() bool`

HasToken returns a boolean if a field has been set.

### GetUsername

`func (o *CreateNotificationChannelRequestCredentials) GetUsername() string`

GetUsername returns the Username field if non-nil, zero value otherwise.

### GetUsernameOk

`func (o *CreateNotificationChannelRequestCredentials) GetUsernameOk() (*string, bool)`

GetUsernameOk returns a tuple with the Username field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUsername

`func (o *CreateNotificationChannelRequestCredentials) SetUsername(v string)`

SetUsername sets Username field to given value.

### HasUsername

`func (o *CreateNotificationChannelRequestCredentials) HasUsername() bool`

HasUsername returns a boolean if a field has been set.

### GetPassword

`func (o *CreateNotificationChannelRequestCredentials) GetPassword() string`

GetPassword returns the Password field if non-nil, zero value otherwise.

### GetPasswordOk

`func (o *CreateNotificationChannelRequestCredentials) GetPasswordOk() (*string, bool)`

GetPasswordOk returns a tuple with the Password field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPassword

`func (o *CreateNotificationChannelRequestCredentials) SetPassword(v string)`

SetPassword sets Password field to given value.

### HasPassword

`func (o *CreateNotificationChannelRequestCredentials) HasPassword() bool`

HasPassword returns a boolean if a field has been set.

### GetHeaders

`func (o *CreateNotificationChannelRequestCredentials) GetHeaders() map[string]string`

GetHeaders returns the Headers field if non-nil, zero value otherwise.

### GetHeadersOk

`func (o *CreateNotificationChannelRequestCredentials) GetHeadersOk() (*map[string]string, bool)`

GetHeadersOk returns a tuple with the Headers field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHeaders

`func (o *CreateNotificationChannelRequestCredentials) SetHeaders(v map[string]string)`

SetHeaders sets Headers field to given value.

### HasHeaders

`func (o *CreateNotificationChannelRequestCredentials) HasHeaders() bool`

HasHeaders returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


