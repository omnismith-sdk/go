# InboundSecret

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**Hint** | **string** | The last four characters of the secret | 
**CreatedAt** | **time.Time** |  | 

## Methods

### NewInboundSecret

`func NewInboundSecret(id string, hint string, createdAt time.Time, ) *InboundSecret`

NewInboundSecret instantiates a new InboundSecret object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInboundSecretWithDefaults

`func NewInboundSecretWithDefaults() *InboundSecret`

NewInboundSecretWithDefaults instantiates a new InboundSecret object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *InboundSecret) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *InboundSecret) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *InboundSecret) SetId(v string)`

SetId sets Id field to given value.


### GetHint

`func (o *InboundSecret) GetHint() string`

GetHint returns the Hint field if non-nil, zero value otherwise.

### GetHintOk

`func (o *InboundSecret) GetHintOk() (*string, bool)`

GetHintOk returns a tuple with the Hint field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHint

`func (o *InboundSecret) SetHint(v string)`

SetHint sets Hint field to given value.


### GetCreatedAt

`func (o *InboundSecret) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *InboundSecret) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *InboundSecret) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


