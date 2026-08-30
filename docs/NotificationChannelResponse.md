# NotificationChannelResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** | Unique notification channel UUID | [optional] 
**Type** | Pointer to **string** | Channel delivery type (telegram, webhook, push) | [optional] 
**Name** | Pointer to **string** | User-friendly display name of the notification channel | [optional] 
**Credentials** | Pointer to **map[string]string** | Sanitized or configured integration credentials for the channel | [optional] 
**CreatedAt** | Pointer to **time.Time** | Creation timestamp | [optional] 
**UpdatedAt** | Pointer to **time.Time** | Last update timestamp | [optional] 

## Methods

### NewNotificationChannelResponse

`func NewNotificationChannelResponse() *NotificationChannelResponse`

NewNotificationChannelResponse instantiates a new NotificationChannelResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewNotificationChannelResponseWithDefaults

`func NewNotificationChannelResponseWithDefaults() *NotificationChannelResponse`

NewNotificationChannelResponseWithDefaults instantiates a new NotificationChannelResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *NotificationChannelResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *NotificationChannelResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *NotificationChannelResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *NotificationChannelResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetType

`func (o *NotificationChannelResponse) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *NotificationChannelResponse) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *NotificationChannelResponse) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *NotificationChannelResponse) HasType() bool`

HasType returns a boolean if a field has been set.

### GetName

`func (o *NotificationChannelResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *NotificationChannelResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *NotificationChannelResponse) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *NotificationChannelResponse) HasName() bool`

HasName returns a boolean if a field has been set.

### GetCredentials

`func (o *NotificationChannelResponse) GetCredentials() map[string]string`

GetCredentials returns the Credentials field if non-nil, zero value otherwise.

### GetCredentialsOk

`func (o *NotificationChannelResponse) GetCredentialsOk() (*map[string]string, bool)`

GetCredentialsOk returns a tuple with the Credentials field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCredentials

`func (o *NotificationChannelResponse) SetCredentials(v map[string]string)`

SetCredentials sets Credentials field to given value.

### HasCredentials

`func (o *NotificationChannelResponse) HasCredentials() bool`

HasCredentials returns a boolean if a field has been set.

### SetCredentialsNil

`func (o *NotificationChannelResponse) SetCredentialsNil(b bool)`

 SetCredentialsNil sets the value for Credentials to be an explicit nil

### UnsetCredentials
`func (o *NotificationChannelResponse) UnsetCredentials()`

UnsetCredentials ensures that no value is present for Credentials, not even an explicit nil
### GetCreatedAt

`func (o *NotificationChannelResponse) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *NotificationChannelResponse) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *NotificationChannelResponse) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *NotificationChannelResponse) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetUpdatedAt

`func (o *NotificationChannelResponse) GetUpdatedAt() time.Time`

GetUpdatedAt returns the UpdatedAt field if non-nil, zero value otherwise.

### GetUpdatedAtOk

`func (o *NotificationChannelResponse) GetUpdatedAtOk() (*time.Time, bool)`

GetUpdatedAtOk returns a tuple with the UpdatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUpdatedAt

`func (o *NotificationChannelResponse) SetUpdatedAt(v time.Time)`

SetUpdatedAt sets UpdatedAt field to given value.

### HasUpdatedAt

`func (o *NotificationChannelResponse) HasUpdatedAt() bool`

HasUpdatedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


