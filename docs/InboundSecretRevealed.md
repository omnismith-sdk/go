# InboundSecretRevealed

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Hint** | **string** | The last four characters of the secret | 
**CreatedAt** | **time.Time** |  | 
**Value** | **string** | The secret to configure in the sender | 

## Methods

### NewInboundSecretRevealed

`func NewInboundSecretRevealed(id string, hint string, createdAt time.Time, value string, ) *InboundSecretRevealed`

NewInboundSecretRevealed instantiates a new InboundSecretRevealed object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInboundSecretRevealedWithDefaults

`func NewInboundSecretRevealedWithDefaults() *InboundSecretRevealed`

NewInboundSecretRevealedWithDefaults instantiates a new InboundSecretRevealed object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *InboundSecretRevealed) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *InboundSecretRevealed) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *InboundSecretRevealed) SetId(v string)`

SetId sets Id field to given value.


### GetHint

`func (o *InboundSecretRevealed) GetHint() string`

GetHint returns the Hint field if non-nil, zero value otherwise.

### GetHintOk

`func (o *InboundSecretRevealed) GetHintOk() (*string, bool)`

GetHintOk returns a tuple with the Hint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHint

`func (o *InboundSecretRevealed) SetHint(v string)`

SetHint sets Hint field to given value.


### GetCreatedAt

`func (o *InboundSecretRevealed) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *InboundSecretRevealed) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *InboundSecretRevealed) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.


### GetValue

`func (o *InboundSecretRevealed) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *InboundSecretRevealed) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *InboundSecretRevealed) SetValue(v string)`

SetValue sets Value field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


