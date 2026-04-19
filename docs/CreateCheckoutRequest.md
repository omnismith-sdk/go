# CreateCheckoutRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TierId** | **string** | The tier ID to subscribe to (use the id value from GET /billing/tiers) | 

## Methods

### NewCreateCheckoutRequest

`func NewCreateCheckoutRequest(tierId string, ) *CreateCheckoutRequest`

NewCreateCheckoutRequest instantiates a new CreateCheckoutRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateCheckoutRequestWithDefaults

`func NewCreateCheckoutRequestWithDefaults() *CreateCheckoutRequest`

NewCreateCheckoutRequestWithDefaults instantiates a new CreateCheckoutRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTierId

`func (o *CreateCheckoutRequest) GetTierId() string`

GetTierId returns the TierId field if non-nil, zero value otherwise.

### GetTierIdOk

`func (o *CreateCheckoutRequest) GetTierIdOk() (*string, bool)`

GetTierIdOk returns a tuple with the TierId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTierId

`func (o *CreateCheckoutRequest) SetTierId(v string)`

SetTierId sets TierId field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


