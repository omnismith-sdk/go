# PreviewInboundMapping200ResponseItemsInner

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Index** | **int32** | Position in the payload&#39;s &#x60;items&#x60; list; 0 without one | 
**ExternalKey** | **NullableString** |  | 
**Action** | **NullableString** | What a delivery would do with this record; null when the record fails before that is known | 
**EntityId** | **NullableString** | The record an update would change | 
**Attributes** | **map[string]interface{}** | Values keyed as in the mapping: a string, null to clear, or &#x60;{value, updated_at}&#x60; for a timed value | 
**Error** | **map[string]interface{}** | The error body a real delivery would meet for this record | 

## Methods

### NewPreviewInboundMapping200ResponseItemsInner

`func NewPreviewInboundMapping200ResponseItemsInner(index int32, externalKey NullableString, action NullableString, entityId NullableString, attributes map[string]interface{}, error_ map[string]interface{}, ) *PreviewInboundMapping200ResponseItemsInner`

NewPreviewInboundMapping200ResponseItemsInner instantiates a new PreviewInboundMapping200ResponseItemsInner object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPreviewInboundMapping200ResponseItemsInnerWithDefaults

`func NewPreviewInboundMapping200ResponseItemsInnerWithDefaults() *PreviewInboundMapping200ResponseItemsInner`

NewPreviewInboundMapping200ResponseItemsInnerWithDefaults instantiates a new PreviewInboundMapping200ResponseItemsInner object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIndex

`func (o *PreviewInboundMapping200ResponseItemsInner) GetIndex() int32`

GetIndex returns the Index field if non-nil, zero value otherwise.

### GetIndexOk

`func (o *PreviewInboundMapping200ResponseItemsInner) GetIndexOk() (*int32, bool)`

GetIndexOk returns a tuple with the Index field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIndex

`func (o *PreviewInboundMapping200ResponseItemsInner) SetIndex(v int32)`

SetIndex sets Index field to given value.


### GetExternalKey

`func (o *PreviewInboundMapping200ResponseItemsInner) GetExternalKey() string`

GetExternalKey returns the ExternalKey field if non-nil, zero value otherwise.

### GetExternalKeyOk

`func (o *PreviewInboundMapping200ResponseItemsInner) GetExternalKeyOk() (*string, bool)`

GetExternalKeyOk returns a tuple with the ExternalKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExternalKey

`func (o *PreviewInboundMapping200ResponseItemsInner) SetExternalKey(v string)`

SetExternalKey sets ExternalKey field to given value.


### SetExternalKeyNil

`func (o *PreviewInboundMapping200ResponseItemsInner) SetExternalKeyNil(b bool)`

 SetExternalKeyNil sets the value for ExternalKey to be an explicit nil

### UnsetExternalKey
`func (o *PreviewInboundMapping200ResponseItemsInner) UnsetExternalKey()`

UnsetExternalKey ensures that no value is present for ExternalKey, not even an explicit nil
### GetAction

`func (o *PreviewInboundMapping200ResponseItemsInner) GetAction() string`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *PreviewInboundMapping200ResponseItemsInner) GetActionOk() (*string, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *PreviewInboundMapping200ResponseItemsInner) SetAction(v string)`

SetAction sets Action field to given value.


### SetActionNil

`func (o *PreviewInboundMapping200ResponseItemsInner) SetActionNil(b bool)`

 SetActionNil sets the value for Action to be an explicit nil

### UnsetAction
`func (o *PreviewInboundMapping200ResponseItemsInner) UnsetAction()`

UnsetAction ensures that no value is present for Action, not even an explicit nil
### GetEntityId

`func (o *PreviewInboundMapping200ResponseItemsInner) GetEntityId() string`

GetEntityId returns the EntityId field if non-nil, zero value otherwise.

### GetEntityIdOk

`func (o *PreviewInboundMapping200ResponseItemsInner) GetEntityIdOk() (*string, bool)`

GetEntityIdOk returns a tuple with the EntityId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityId

`func (o *PreviewInboundMapping200ResponseItemsInner) SetEntityId(v string)`

SetEntityId sets EntityId field to given value.


### SetEntityIdNil

`func (o *PreviewInboundMapping200ResponseItemsInner) SetEntityIdNil(b bool)`

 SetEntityIdNil sets the value for EntityId to be an explicit nil

### UnsetEntityId
`func (o *PreviewInboundMapping200ResponseItemsInner) UnsetEntityId()`

UnsetEntityId ensures that no value is present for EntityId, not even an explicit nil
### GetAttributes

`func (o *PreviewInboundMapping200ResponseItemsInner) GetAttributes() map[string]interface{}`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *PreviewInboundMapping200ResponseItemsInner) GetAttributesOk() (*map[string]interface{}, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *PreviewInboundMapping200ResponseItemsInner) SetAttributes(v map[string]interface{})`

SetAttributes sets Attributes field to given value.


### GetError

`func (o *PreviewInboundMapping200ResponseItemsInner) GetError() map[string]interface{}`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *PreviewInboundMapping200ResponseItemsInner) GetErrorOk() (*map[string]interface{}, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *PreviewInboundMapping200ResponseItemsInner) SetError(v map[string]interface{})`

SetError sets Error field to given value.


### SetErrorNil

`func (o *PreviewInboundMapping200ResponseItemsInner) SetErrorNil(b bool)`

 SetErrorNil sets the value for Error to be an explicit nil

### UnsetError
`func (o *PreviewInboundMapping200ResponseItemsInner) UnsetError()`

UnsetError ensures that no value is present for Error, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


