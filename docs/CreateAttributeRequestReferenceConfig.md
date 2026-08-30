# CreateAttributeRequestReferenceConfig

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TargetTemplateId** | Pointer to **string** | UUID of the target template whose entities can be referenced. | [optional] 
**TargetAttributeId** | Pointer to **string** | UUID of the attribute on the target template to use for entity display label resolution. | [optional] 

## Methods

### NewCreateAttributeRequestReferenceConfig

`func NewCreateAttributeRequestReferenceConfig() *CreateAttributeRequestReferenceConfig`

NewCreateAttributeRequestReferenceConfig instantiates a new CreateAttributeRequestReferenceConfig object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateAttributeRequestReferenceConfigWithDefaults

`func NewCreateAttributeRequestReferenceConfigWithDefaults() *CreateAttributeRequestReferenceConfig`

NewCreateAttributeRequestReferenceConfigWithDefaults instantiates a new CreateAttributeRequestReferenceConfig object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTargetTemplateId

`func (o *CreateAttributeRequestReferenceConfig) GetTargetTemplateId() string`

GetTargetTemplateId returns the TargetTemplateId field if non-nil, zero value otherwise.

### GetTargetTemplateIdOk

`func (o *CreateAttributeRequestReferenceConfig) GetTargetTemplateIdOk() (*string, bool)`

GetTargetTemplateIdOk returns a tuple with the TargetTemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetTemplateId

`func (o *CreateAttributeRequestReferenceConfig) SetTargetTemplateId(v string)`

SetTargetTemplateId sets TargetTemplateId field to given value.

### HasTargetTemplateId

`func (o *CreateAttributeRequestReferenceConfig) HasTargetTemplateId() bool`

HasTargetTemplateId returns a boolean if a field has been set.

### GetTargetAttributeId

`func (o *CreateAttributeRequestReferenceConfig) GetTargetAttributeId() string`

GetTargetAttributeId returns the TargetAttributeId field if non-nil, zero value otherwise.

### GetTargetAttributeIdOk

`func (o *CreateAttributeRequestReferenceConfig) GetTargetAttributeIdOk() (*string, bool)`

GetTargetAttributeIdOk returns a tuple with the TargetAttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetAttributeId

`func (o *CreateAttributeRequestReferenceConfig) SetTargetAttributeId(v string)`

SetTargetAttributeId sets TargetAttributeId field to given value.

### HasTargetAttributeId

`func (o *CreateAttributeRequestReferenceConfig) HasTargetAttributeId() bool`

HasTargetAttributeId returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


