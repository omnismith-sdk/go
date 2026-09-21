# ExecuteEntityActionResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EntityId** | **string** |  | 
**TemplateId** | **string** |  | 
**Action** | [**ExecuteEntityActionResponseAction**](ExecuteEntityActionResponseAction.md) |  | 
**Attributes** | **map[string]string** | Attribute slug (or UUID for a slugless attribute) → value written, as stored | 

## Methods

### NewExecuteEntityActionResponse

`func NewExecuteEntityActionResponse(entityId string, templateId string, action ExecuteEntityActionResponseAction, attributes map[string]string, ) *ExecuteEntityActionResponse`

NewExecuteEntityActionResponse instantiates a new ExecuteEntityActionResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExecuteEntityActionResponseWithDefaults

`func NewExecuteEntityActionResponseWithDefaults() *ExecuteEntityActionResponse`

NewExecuteEntityActionResponseWithDefaults instantiates a new ExecuteEntityActionResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEntityId

`func (o *ExecuteEntityActionResponse) GetEntityId() string`

GetEntityId returns the EntityId field if non-nil, zero value otherwise.

### GetEntityIdOk

`func (o *ExecuteEntityActionResponse) GetEntityIdOk() (*string, bool)`

GetEntityIdOk returns a tuple with the EntityId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityId

`func (o *ExecuteEntityActionResponse) SetEntityId(v string)`

SetEntityId sets EntityId field to given value.


### GetTemplateId

`func (o *ExecuteEntityActionResponse) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *ExecuteEntityActionResponse) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *ExecuteEntityActionResponse) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.


### GetAction

`func (o *ExecuteEntityActionResponse) GetAction() ExecuteEntityActionResponseAction`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *ExecuteEntityActionResponse) GetActionOk() (*ExecuteEntityActionResponseAction, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *ExecuteEntityActionResponse) SetAction(v ExecuteEntityActionResponseAction)`

SetAction sets Action field to given value.


### GetAttributes

`func (o *ExecuteEntityActionResponse) GetAttributes() map[string]string`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *ExecuteEntityActionResponse) GetAttributesOk() (*map[string]string, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *ExecuteEntityActionResponse) SetAttributes(v map[string]string)`

SetAttributes sets Attributes field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


