# CheckoutResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**CheckoutUrl** | Pointer to **string** | URL to redirect user to complete checkout | [optional] 
**CheckoutId** | Pointer to **string** | LemonSqueezy checkout session ID | [optional] 

## Methods

### NewCheckoutResponse

`func NewCheckoutResponse() *CheckoutResponse`

NewCheckoutResponse instantiates a new CheckoutResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCheckoutResponseWithDefaults

`func NewCheckoutResponseWithDefaults() *CheckoutResponse`

NewCheckoutResponseWithDefaults instantiates a new CheckoutResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCheckoutUrl

`func (o *CheckoutResponse) GetCheckoutUrl() string`

GetCheckoutUrl returns the CheckoutUrl field if non-nil, zero value otherwise.

### GetCheckoutUrlOk

`func (o *CheckoutResponse) GetCheckoutUrlOk() (*string, bool)`

GetCheckoutUrlOk returns a tuple with the CheckoutUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCheckoutUrl

`func (o *CheckoutResponse) SetCheckoutUrl(v string)`

SetCheckoutUrl sets CheckoutUrl field to given value.

### HasCheckoutUrl

`func (o *CheckoutResponse) HasCheckoutUrl() bool`

HasCheckoutUrl returns a boolean if a field has been set.

### GetCheckoutId

`func (o *CheckoutResponse) GetCheckoutId() string`

GetCheckoutId returns the CheckoutId field if non-nil, zero value otherwise.

### GetCheckoutIdOk

`func (o *CheckoutResponse) GetCheckoutIdOk() (*string, bool)`

GetCheckoutIdOk returns a tuple with the CheckoutId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCheckoutId

`func (o *CheckoutResponse) SetCheckoutId(v string)`

SetCheckoutId sets CheckoutId field to given value.

### HasCheckoutId

`func (o *CheckoutResponse) HasCheckoutId() bool`

HasCheckoutId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


