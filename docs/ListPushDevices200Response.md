# ListPushDevices200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Data** | Pointer to [**[]PushDeviceResponse**](PushDeviceResponse.md) | Array of registered push devices | [optional] 

## Methods

### NewListPushDevices200Response

`func NewListPushDevices200Response() *ListPushDevices200Response`

NewListPushDevices200Response instantiates a new ListPushDevices200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListPushDevices200ResponseWithDefaults

`func NewListPushDevices200ResponseWithDefaults() *ListPushDevices200Response`

NewListPushDevices200ResponseWithDefaults instantiates a new ListPushDevices200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetData

`func (o *ListPushDevices200Response) GetData() []PushDeviceResponse`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *ListPushDevices200Response) GetDataOk() (*[]PushDeviceResponse, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *ListPushDevices200Response) SetData(v []PushDeviceResponse)`

SetData sets Data field to given value.

### HasData

`func (o *ListPushDevices200Response) HasData() bool`

HasData returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


