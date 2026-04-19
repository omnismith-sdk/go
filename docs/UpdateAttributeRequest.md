# UpdateAttributeRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **string** |  | 
**TemplateIds** | Pointer to **[]string** |  | [optional] 
**ReferenceConfig** | Pointer to [**NullableUpdateAttributeRequestReferenceConfig**](UpdateAttributeRequestReferenceConfig.md) |  | [optional] 

## Methods

### NewUpdateAttributeRequest

`func NewUpdateAttributeRequest(name string, ) *UpdateAttributeRequest`

NewUpdateAttributeRequest instantiates a new UpdateAttributeRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewUpdateAttributeRequestWithDefaults

`func NewUpdateAttributeRequestWithDefaults() *UpdateAttributeRequest`

NewUpdateAttributeRequestWithDefaults instantiates a new UpdateAttributeRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *UpdateAttributeRequest) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *UpdateAttributeRequest) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *UpdateAttributeRequest) SetName(v string)`

SetName sets Name field to given value.


### GetTemplateIds

`func (o *UpdateAttributeRequest) GetTemplateIds() []string`

GetTemplateIds returns the TemplateIds field if non-nil, zero value otherwise.

### GetTemplateIdsOk

`func (o *UpdateAttributeRequest) GetTemplateIdsOk() (*[]string, bool)`

GetTemplateIdsOk returns a tuple with the TemplateIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateIds

`func (o *UpdateAttributeRequest) SetTemplateIds(v []string)`

SetTemplateIds sets TemplateIds field to given value.

### HasTemplateIds

`func (o *UpdateAttributeRequest) HasTemplateIds() bool`

HasTemplateIds returns a boolean if a field has been set.

### GetReferenceConfig

`func (o *UpdateAttributeRequest) GetReferenceConfig() UpdateAttributeRequestReferenceConfig`

GetReferenceConfig returns the ReferenceConfig field if non-nil, zero value otherwise.

### GetReferenceConfigOk

`func (o *UpdateAttributeRequest) GetReferenceConfigOk() (*UpdateAttributeRequestReferenceConfig, bool)`

GetReferenceConfigOk returns a tuple with the ReferenceConfig field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReferenceConfig

`func (o *UpdateAttributeRequest) SetReferenceConfig(v UpdateAttributeRequestReferenceConfig)`

SetReferenceConfig sets ReferenceConfig field to given value.

### HasReferenceConfig

`func (o *UpdateAttributeRequest) HasReferenceConfig() bool`

HasReferenceConfig returns a boolean if a field has been set.

### SetReferenceConfigNil

`func (o *UpdateAttributeRequest) SetReferenceConfigNil(b bool)`

 SetReferenceConfigNil sets the value for ReferenceConfig to be an explicit nil

### UnsetReferenceConfig
`func (o *UpdateAttributeRequest) UnsetReferenceConfig()`

UnsetReferenceConfig ensures that no value is present for ReferenceConfig, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


