# AddInboundEndpointSecretRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Secret** | Pointer to **string** | The secret the sender signs with, when the sender issued it (Stripe and Shopify do). Omit it to have one generated, which suits GitHub, custom senders and &#x60;shared_secret_header&#x60; (always generated). The secret is returned once, in this response, and never again. | [optional] 

## Methods

### NewAddInboundEndpointSecretRequest

`func NewAddInboundEndpointSecretRequest() *AddInboundEndpointSecretRequest`

NewAddInboundEndpointSecretRequest instantiates a new AddInboundEndpointSecretRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAddInboundEndpointSecretRequestWithDefaults

`func NewAddInboundEndpointSecretRequestWithDefaults() *AddInboundEndpointSecretRequest`

NewAddInboundEndpointSecretRequestWithDefaults instantiates a new AddInboundEndpointSecretRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSecret

`func (o *AddInboundEndpointSecretRequest) GetSecret() string`

GetSecret returns the Secret field if non-nil, zero value otherwise.

### GetSecretOk

`func (o *AddInboundEndpointSecretRequest) GetSecretOk() (*string, bool)`

GetSecretOk returns a tuple with the Secret field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecret

`func (o *AddInboundEndpointSecretRequest) SetSecret(v string)`

SetSecret sets Secret field to given value.

### HasSecret

`func (o *AddInboundEndpointSecretRequest) HasSecret() bool`

HasSecret returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


