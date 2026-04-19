# SetRoleResourcesRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Resources** | [**[]ResourceAccessInput**](ResourceAccessInput.md) |  | 

## Methods

### NewSetRoleResourcesRequest

`func NewSetRoleResourcesRequest(resources []ResourceAccessInput, ) *SetRoleResourcesRequest`

NewSetRoleResourcesRequest instantiates a new SetRoleResourcesRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSetRoleResourcesRequestWithDefaults

`func NewSetRoleResourcesRequestWithDefaults() *SetRoleResourcesRequest`

NewSetRoleResourcesRequestWithDefaults instantiates a new SetRoleResourcesRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetResources

`func (o *SetRoleResourcesRequest) GetResources() []ResourceAccessInput`

GetResources returns the Resources field if non-nil, zero value otherwise.

### GetResourcesOk

`func (o *SetRoleResourcesRequest) GetResourcesOk() (*[]ResourceAccessInput, bool)`

GetResourcesOk returns a tuple with the Resources field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResources

`func (o *SetRoleResourcesRequest) SetResources(v []ResourceAccessInput)`

SetResources sets Resources field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


