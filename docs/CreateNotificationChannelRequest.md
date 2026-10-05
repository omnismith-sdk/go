# CreateNotificationChannelRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** | Channel delivery type (telegram, webhook, push) | 
**Name** | **string** | Display name of the notification channel | 
**Credentials** | [**CreateNotificationChannelRequestCredentials**](CreateNotificationChannelRequestCredentials.md) |  | 
**RateLimitPerMinute** | Pointer to **int32** | Maximum messages the channel sends per clock minute, across all automations and records; sends over it fail the action (recorded in the execution history) instead of reaching the destination. Defaults to 20, Telegram&#39;s limit for one group. | [optional] [default to 20]

## Methods

### NewCreateNotificationChannelRequest

`func NewCreateNotificationChannelRequest(type_ string, name string, credentials CreateNotificationChannelRequestCredentials, ) *CreateNotificationChannelRequest`

NewCreateNotificationChannelRequest instantiates a new CreateNotificationChannelRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateNotificationChannelRequestWithDefaults

`func NewCreateNotificationChannelRequestWithDefaults() *CreateNotificationChannelRequest`

NewCreateNotificationChannelRequestWithDefaults instantiates a new CreateNotificationChannelRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *CreateNotificationChannelRequest) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *CreateNotificationChannelRequest) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *CreateNotificationChannelRequest) SetType(v string)`

SetType sets Type field to given value.


### GetName

`func (o *CreateNotificationChannelRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateNotificationChannelRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateNotificationChannelRequest) SetName(v string)`

SetName sets Name field to given value.


### GetCredentials

`func (o *CreateNotificationChannelRequest) GetCredentials() CreateNotificationChannelRequestCredentials`

GetCredentials returns the Credentials field if non-nil, zero value otherwise.

### GetCredentialsOk

`func (o *CreateNotificationChannelRequest) GetCredentialsOk() (*CreateNotificationChannelRequestCredentials, bool)`

GetCredentialsOk returns a tuple with the Credentials field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCredentials

`func (o *CreateNotificationChannelRequest) SetCredentials(v CreateNotificationChannelRequestCredentials)`

SetCredentials sets Credentials field to given value.


### GetRateLimitPerMinute

`func (o *CreateNotificationChannelRequest) GetRateLimitPerMinute() int32`

GetRateLimitPerMinute returns the RateLimitPerMinute field if non-nil, zero value otherwise.

### GetRateLimitPerMinuteOk

`func (o *CreateNotificationChannelRequest) GetRateLimitPerMinuteOk() (*int32, bool)`

GetRateLimitPerMinuteOk returns a tuple with the RateLimitPerMinute field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRateLimitPerMinute

`func (o *CreateNotificationChannelRequest) SetRateLimitPerMinute(v int32)`

SetRateLimitPerMinute sets RateLimitPerMinute field to given value.

### HasRateLimitPerMinute

`func (o *CreateNotificationChannelRequest) HasRateLimitPerMinute() bool`

HasRateLimitPerMinute returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


