# UpdateNotificationChannelRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **NullableString** |  | [optional] 
**Credentials** | Pointer to [**NullableUpdateNotificationChannelRequestCredentials**](UpdateNotificationChannelRequestCredentials.md) |  | [optional] 

## Methods

### NewUpdateNotificationChannelRequest

`func NewUpdateNotificationChannelRequest() *UpdateNotificationChannelRequest`

NewUpdateNotificationChannelRequest instantiates a new UpdateNotificationChannelRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateNotificationChannelRequestWithDefaults

`func NewUpdateNotificationChannelRequestWithDefaults() *UpdateNotificationChannelRequest`

NewUpdateNotificationChannelRequestWithDefaults instantiates a new UpdateNotificationChannelRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *UpdateNotificationChannelRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateNotificationChannelRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateNotificationChannelRequest) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *UpdateNotificationChannelRequest) HasName() bool`

HasName returns a boolean if a field has been set.

### SetNameNil

`func (o *UpdateNotificationChannelRequest) SetNameNil(b bool)`

 SetNameNil sets the value for Name to be an explicit nil

### UnsetName
`func (o *UpdateNotificationChannelRequest) UnsetName()`

UnsetName ensures that no value is present for Name, not even an explicit nil
### GetCredentials

`func (o *UpdateNotificationChannelRequest) GetCredentials() UpdateNotificationChannelRequestCredentials`

GetCredentials returns the Credentials field if non-nil, zero value otherwise.

### GetCredentialsOk

`func (o *UpdateNotificationChannelRequest) GetCredentialsOk() (*UpdateNotificationChannelRequestCredentials, bool)`

GetCredentialsOk returns a tuple with the Credentials field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCredentials

`func (o *UpdateNotificationChannelRequest) SetCredentials(v UpdateNotificationChannelRequestCredentials)`

SetCredentials sets Credentials field to given value.

### HasCredentials

`func (o *UpdateNotificationChannelRequest) HasCredentials() bool`

HasCredentials returns a boolean if a field has been set.

### SetCredentialsNil

`func (o *UpdateNotificationChannelRequest) SetCredentialsNil(b bool)`

 SetCredentialsNil sets the value for Credentials to be an explicit nil

### UnsetCredentials
`func (o *UpdateNotificationChannelRequest) UnsetCredentials()`

UnsetCredentials ensures that no value is present for Credentials, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


