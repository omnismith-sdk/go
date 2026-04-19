# SetUserTierRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TierId** | **string** |  | 
**Reason** | Pointer to **string** |  | [optional] 

## Methods

### NewSetUserTierRequest

`func NewSetUserTierRequest(tierId string, ) *SetUserTierRequest`

NewSetUserTierRequest instantiates a new SetUserTierRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSetUserTierRequestWithDefaults

`func NewSetUserTierRequestWithDefaults() *SetUserTierRequest`

NewSetUserTierRequestWithDefaults instantiates a new SetUserTierRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTierId

`func (o *SetUserTierRequest) GetTierId() string`

GetTierId returns the TierId field if non-nil, zero value otherwise.

### GetTierIdOk

`func (o *SetUserTierRequest) GetTierIdOk() (*string, bool)`

GetTierIdOk returns a tuple with the TierId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTierId

`func (o *SetUserTierRequest) SetTierId(v string)`

SetTierId sets TierId field to given value.


### GetReason

`func (o *SetUserTierRequest) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *SetUserTierRequest) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *SetUserTierRequest) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *SetUserTierRequest) HasReason() bool`

HasReason returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


