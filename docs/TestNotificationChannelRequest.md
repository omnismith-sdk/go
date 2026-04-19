# TestNotificationChannelRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ChatId** | Pointer to **string** | Telegram chat ID (required for Telegram channels) | [optional] 
**Message** | Pointer to **string** |  | [optional] 
**Title** | Pointer to **string** | Notification title (used for push notifications) | [optional] 

## Methods

### NewTestNotificationChannelRequest

`func NewTestNotificationChannelRequest() *TestNotificationChannelRequest`

NewTestNotificationChannelRequest instantiates a new TestNotificationChannelRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTestNotificationChannelRequestWithDefaults

`func NewTestNotificationChannelRequestWithDefaults() *TestNotificationChannelRequest`

NewTestNotificationChannelRequestWithDefaults instantiates a new TestNotificationChannelRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetChatId

`func (o *TestNotificationChannelRequest) GetChatId() string`

GetChatId returns the ChatId field if non-nil, zero value otherwise.

### GetChatIdOk

`func (o *TestNotificationChannelRequest) GetChatIdOk() (*string, bool)`

GetChatIdOk returns a tuple with the ChatId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetChatId

`func (o *TestNotificationChannelRequest) SetChatId(v string)`

SetChatId sets ChatId field to given value.

### HasChatId

`func (o *TestNotificationChannelRequest) HasChatId() bool`

HasChatId returns a boolean if a field has been set.

### GetMessage

`func (o *TestNotificationChannelRequest) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *TestNotificationChannelRequest) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *TestNotificationChannelRequest) SetMessage(v string)`

SetMessage sets Message field to given value.

### HasMessage

`func (o *TestNotificationChannelRequest) HasMessage() bool`

HasMessage returns a boolean if a field has been set.

### GetTitle

`func (o *TestNotificationChannelRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *TestNotificationChannelRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *TestNotificationChannelRequest) SetTitle(v string)`

SetTitle sets Title field to given value.

### HasTitle

`func (o *TestNotificationChannelRequest) HasTitle() bool`

HasTitle returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


