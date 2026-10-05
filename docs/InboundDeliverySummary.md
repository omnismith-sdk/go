# InboundDeliverySummary

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** |  | 
**ReceivedAt** | **time.Time** |  | 
**DeliveryId** | **NullableString** | The sender&#39;s id for the delivery, when the endpoint names a delivery id source | 
**Outcome** | **string** | &#x60;processed&#x60;: every record was written. &#x60;partial&#x60;: some records of a multi-record delivery failed. &#x60;skipped&#x60;: the match condition did not hold, or the delivery id was already processed. &#x60;rejected&#x60;: the request was wrong (400, 401, 413, 422). &#x60;failed&#x60;: it could not be written right now (409, 429, 5xx). | 
**HttpStatus** | **int32** | The status the sender was answered with | 
**Error** | **map[string]interface{}** | The answer&#39;s error body for a non-2xx delivery, &#x60;{errors, items}&#x60; for a partial one, or &#x60;{\&quot;reason\&quot;: ...}&#x60; for a signature failure | 
**EntityIds** | **[]string** | Records created or updated | 
**BodyTruncated** | **bool** | The stored body was cut at 256 KB | 
**DurationMs** | **int32** |  | 
**ReplayOf** | **NullableString** | The delivery this one replayed | 
**ReplayedBy** | **NullableString** | Email of the user who asked for the replay | 

## Methods

### NewInboundDeliverySummary

`func NewInboundDeliverySummary(id string, receivedAt time.Time, deliveryId NullableString, outcome string, httpStatus int32, error_ map[string]interface{}, entityIds []string, bodyTruncated bool, durationMs int32, replayOf NullableString, replayedBy NullableString, ) *InboundDeliverySummary`

NewInboundDeliverySummary instantiates a new InboundDeliverySummary object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInboundDeliverySummaryWithDefaults

`func NewInboundDeliverySummaryWithDefaults() *InboundDeliverySummary`

NewInboundDeliverySummaryWithDefaults instantiates a new InboundDeliverySummary object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *InboundDeliverySummary) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *InboundDeliverySummary) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *InboundDeliverySummary) SetId(v string)`

SetId sets Id field to given value.


### GetReceivedAt

`func (o *InboundDeliverySummary) GetReceivedAt() time.Time`

GetReceivedAt returns the ReceivedAt field if non-nil, zero value otherwise.

### GetReceivedAtOk

`func (o *InboundDeliverySummary) GetReceivedAtOk() (*time.Time, bool)`

GetReceivedAtOk returns a tuple with the ReceivedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReceivedAt

`func (o *InboundDeliverySummary) SetReceivedAt(v time.Time)`

SetReceivedAt sets ReceivedAt field to given value.


### GetDeliveryId

`func (o *InboundDeliverySummary) GetDeliveryId() string`

GetDeliveryId returns the DeliveryId field if non-nil, zero value otherwise.

### GetDeliveryIdOk

`func (o *InboundDeliverySummary) GetDeliveryIdOk() (*string, bool)`

GetDeliveryIdOk returns a tuple with the DeliveryId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeliveryId

`func (o *InboundDeliverySummary) SetDeliveryId(v string)`

SetDeliveryId sets DeliveryId field to given value.


### SetDeliveryIdNil

`func (o *InboundDeliverySummary) SetDeliveryIdNil(b bool)`

 SetDeliveryIdNil sets the value for DeliveryId to be an explicit nil

### UnsetDeliveryId
`func (o *InboundDeliverySummary) UnsetDeliveryId()`

UnsetDeliveryId ensures that no value is present for DeliveryId, not even an explicit nil
### GetOutcome

`func (o *InboundDeliverySummary) GetOutcome() string`

GetOutcome returns the Outcome field if non-nil, zero value otherwise.

### GetOutcomeOk

`func (o *InboundDeliverySummary) GetOutcomeOk() (*string, bool)`

GetOutcomeOk returns a tuple with the Outcome field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOutcome

`func (o *InboundDeliverySummary) SetOutcome(v string)`

SetOutcome sets Outcome field to given value.


### GetHttpStatus

`func (o *InboundDeliverySummary) GetHttpStatus() int32`

GetHttpStatus returns the HttpStatus field if non-nil, zero value otherwise.

### GetHttpStatusOk

`func (o *InboundDeliverySummary) GetHttpStatusOk() (*int32, bool)`

GetHttpStatusOk returns a tuple with the HttpStatus field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHttpStatus

`func (o *InboundDeliverySummary) SetHttpStatus(v int32)`

SetHttpStatus sets HttpStatus field to given value.


### GetError

`func (o *InboundDeliverySummary) GetError() map[string]interface{}`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *InboundDeliverySummary) GetErrorOk() (*map[string]interface{}, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *InboundDeliverySummary) SetError(v map[string]interface{})`

SetError sets Error field to given value.


### SetErrorNil

`func (o *InboundDeliverySummary) SetErrorNil(b bool)`

 SetErrorNil sets the value for Error to be an explicit nil

### UnsetError
`func (o *InboundDeliverySummary) UnsetError()`

UnsetError ensures that no value is present for Error, not even an explicit nil
### GetEntityIds

`func (o *InboundDeliverySummary) GetEntityIds() []string`

GetEntityIds returns the EntityIds field if non-nil, zero value otherwise.

### GetEntityIdsOk

`func (o *InboundDeliverySummary) GetEntityIdsOk() (*[]string, bool)`

GetEntityIdsOk returns a tuple with the EntityIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEntityIds

`func (o *InboundDeliverySummary) SetEntityIds(v []string)`

SetEntityIds sets EntityIds field to given value.


### GetBodyTruncated

`func (o *InboundDeliverySummary) GetBodyTruncated() bool`

GetBodyTruncated returns the BodyTruncated field if non-nil, zero value otherwise.

### GetBodyTruncatedOk

`func (o *InboundDeliverySummary) GetBodyTruncatedOk() (*bool, bool)`

GetBodyTruncatedOk returns a tuple with the BodyTruncated field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBodyTruncated

`func (o *InboundDeliverySummary) SetBodyTruncated(v bool)`

SetBodyTruncated sets BodyTruncated field to given value.


### GetDurationMs

`func (o *InboundDeliverySummary) GetDurationMs() int32`

GetDurationMs returns the DurationMs field if non-nil, zero value otherwise.

### GetDurationMsOk

`func (o *InboundDeliverySummary) GetDurationMsOk() (*int32, bool)`

GetDurationMsOk returns a tuple with the DurationMs field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDurationMs

`func (o *InboundDeliverySummary) SetDurationMs(v int32)`

SetDurationMs sets DurationMs field to given value.


### GetReplayOf

`func (o *InboundDeliverySummary) GetReplayOf() string`

GetReplayOf returns the ReplayOf field if non-nil, zero value otherwise.

### GetReplayOfOk

`func (o *InboundDeliverySummary) GetReplayOfOk() (*string, bool)`

GetReplayOfOk returns a tuple with the ReplayOf field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplayOf

`func (o *InboundDeliverySummary) SetReplayOf(v string)`

SetReplayOf sets ReplayOf field to given value.


### SetReplayOfNil

`func (o *InboundDeliverySummary) SetReplayOfNil(b bool)`

 SetReplayOfNil sets the value for ReplayOf to be an explicit nil

### UnsetReplayOf
`func (o *InboundDeliverySummary) UnsetReplayOf()`

UnsetReplayOf ensures that no value is present for ReplayOf, not even an explicit nil
### GetReplayedBy

`func (o *InboundDeliverySummary) GetReplayedBy() string`

GetReplayedBy returns the ReplayedBy field if non-nil, zero value otherwise.

### GetReplayedByOk

`func (o *InboundDeliverySummary) GetReplayedByOk() (*string, bool)`

GetReplayedByOk returns a tuple with the ReplayedBy field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReplayedBy

`func (o *InboundDeliverySummary) SetReplayedBy(v string)`

SetReplayedBy sets ReplayedBy field to given value.


### SetReplayedByNil

`func (o *InboundDeliverySummary) SetReplayedByNil(b bool)`

 SetReplayedByNil sets the value for ReplayedBy to be an explicit nil

### UnsetReplayedBy
`func (o *InboundDeliverySummary) UnsetReplayedBy()`

UnsetReplayedBy ensures that no value is present for ReplayedBy, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


