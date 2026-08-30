# SetReferenceConfigRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TargetTemplateId** | **string** | UUID of the target template whose entities can be referenced. | 
**TargetAttributeId** | **string** | UUID of the attribute on the target template to display as reference label. | 

## Methods

### NewSetReferenceConfigRequest

`func NewSetReferenceConfigRequest(targetTemplateId string, targetAttributeId string, ) *SetReferenceConfigRequest`

NewSetReferenceConfigRequest instantiates a new SetReferenceConfigRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSetReferenceConfigRequestWithDefaults

`func NewSetReferenceConfigRequestWithDefaults() *SetReferenceConfigRequest`

NewSetReferenceConfigRequestWithDefaults instantiates a new SetReferenceConfigRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTargetTemplateId

`func (o *SetReferenceConfigRequest) GetTargetTemplateId() string`

GetTargetTemplateId returns the TargetTemplateId field if non-nil, zero value otherwise.

### GetTargetTemplateIdOk

`func (o *SetReferenceConfigRequest) GetTargetTemplateIdOk() (*string, bool)`

GetTargetTemplateIdOk returns a tuple with the TargetTemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetTemplateId

`func (o *SetReferenceConfigRequest) SetTargetTemplateId(v string)`

SetTargetTemplateId sets TargetTemplateId field to given value.


### GetTargetAttributeId

`func (o *SetReferenceConfigRequest) GetTargetAttributeId() string`

GetTargetAttributeId returns the TargetAttributeId field if non-nil, zero value otherwise.

### GetTargetAttributeIdOk

`func (o *SetReferenceConfigRequest) GetTargetAttributeIdOk() (*string, bool)`

GetTargetAttributeIdOk returns a tuple with the TargetAttributeId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTargetAttributeId

`func (o *SetReferenceConfigRequest) SetTargetAttributeId(v string)`

SetTargetAttributeId sets TargetAttributeId field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


