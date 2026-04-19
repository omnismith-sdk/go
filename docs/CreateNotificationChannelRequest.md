# CreateNotificationChannelRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** | Channel type: telegram, webhook or push | 
**Name** | **string** |  | 
**Credentials** | [**CreateNotificationChannelRequestCredentials**](CreateNotificationChannelRequestCredentials.md) |  | 

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



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


