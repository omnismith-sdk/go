# AuditLogResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EventId** | Pointer to **string** | Unique audit event identifier (UUIDv7) | [optional] 
**OccurredAt** | Pointer to **time.Time** | Event occurrence timestamp in ISO 8601 format | [optional] 
**EventType** | Pointer to **string** | Action or event identifier (e.g. entity.created, entity.updated, entity.deleted, template.created) | [optional] 
**ResourceType** | Pointer to **string** | Target domain resource type (entity, template, attribute, project) | [optional] 
**ResourceId** | Pointer to **string** | Target resource identifier (UUID) | [optional] 
**Value** | Pointer to **string** | Summary description or serialized payload of the mutation | [optional] 
**AuthorEmail** | Pointer to **NullableString** | Email of the authenticated user who initiated the action | [optional] 
**CorrelationId** | Pointer to **NullableString** | Distributed tracing correlation identifier | [optional] 

## Methods

### NewAuditLogResponse

`func NewAuditLogResponse() *AuditLogResponse`

NewAuditLogResponse instantiates a new AuditLogResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAuditLogResponseWithDefaults

`func NewAuditLogResponseWithDefaults() *AuditLogResponse`

NewAuditLogResponseWithDefaults instantiates a new AuditLogResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEventId

`func (o *AuditLogResponse) GetEventId() string`

GetEventId returns the EventId field if non-nil, zero value otherwise.

### GetEventIdOk

`func (o *AuditLogResponse) GetEventIdOk() (*string, bool)`

GetEventIdOk returns a tuple with the EventId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventId

`func (o *AuditLogResponse) SetEventId(v string)`

SetEventId sets EventId field to given value.

### HasEventId

`func (o *AuditLogResponse) HasEventId() bool`

HasEventId returns a boolean if a field has been set.

### GetOccurredAt

`func (o *AuditLogResponse) GetOccurredAt() time.Time`

GetOccurredAt returns the OccurredAt field if non-nil, zero value otherwise.

### GetOccurredAtOk

`func (o *AuditLogResponse) GetOccurredAtOk() (*time.Time, bool)`

GetOccurredAtOk returns a tuple with the OccurredAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOccurredAt

`func (o *AuditLogResponse) SetOccurredAt(v time.Time)`

SetOccurredAt sets OccurredAt field to given value.

### HasOccurredAt

`func (o *AuditLogResponse) HasOccurredAt() bool`

HasOccurredAt returns a boolean if a field has been set.

### GetEventType

`func (o *AuditLogResponse) GetEventType() string`

GetEventType returns the EventType field if non-nil, zero value otherwise.

### GetEventTypeOk

`func (o *AuditLogResponse) GetEventTypeOk() (*string, bool)`

GetEventTypeOk returns a tuple with the EventType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEventType

`func (o *AuditLogResponse) SetEventType(v string)`

SetEventType sets EventType field to given value.

### HasEventType

`func (o *AuditLogResponse) HasEventType() bool`

HasEventType returns a boolean if a field has been set.

### GetResourceType

`func (o *AuditLogResponse) GetResourceType() string`

GetResourceType returns the ResourceType field if non-nil, zero value otherwise.

### GetResourceTypeOk

`func (o *AuditLogResponse) GetResourceTypeOk() (*string, bool)`

GetResourceTypeOk returns a tuple with the ResourceType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResourceType

`func (o *AuditLogResponse) SetResourceType(v string)`

SetResourceType sets ResourceType field to given value.

### HasResourceType

`func (o *AuditLogResponse) HasResourceType() bool`

HasResourceType returns a boolean if a field has been set.

### GetResourceId

`func (o *AuditLogResponse) GetResourceId() string`

GetResourceId returns the ResourceId field if non-nil, zero value otherwise.

### GetResourceIdOk

`func (o *AuditLogResponse) GetResourceIdOk() (*string, bool)`

GetResourceIdOk returns a tuple with the ResourceId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetResourceId

`func (o *AuditLogResponse) SetResourceId(v string)`

SetResourceId sets ResourceId field to given value.

### HasResourceId

`func (o *AuditLogResponse) HasResourceId() bool`

HasResourceId returns a boolean if a field has been set.

### GetValue

`func (o *AuditLogResponse) GetValue() string`

GetValue returns the Value field if non-nil, zero value otherwise.

### GetValueOk

`func (o *AuditLogResponse) GetValueOk() (*string, bool)`

GetValueOk returns a tuple with the Value field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetValue

`func (o *AuditLogResponse) SetValue(v string)`

SetValue sets Value field to given value.

### HasValue

`func (o *AuditLogResponse) HasValue() bool`

HasValue returns a boolean if a field has been set.

### GetAuthorEmail

`func (o *AuditLogResponse) GetAuthorEmail() string`

GetAuthorEmail returns the AuthorEmail field if non-nil, zero value otherwise.

### GetAuthorEmailOk

`func (o *AuditLogResponse) GetAuthorEmailOk() (*string, bool)`

GetAuthorEmailOk returns a tuple with the AuthorEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthorEmail

`func (o *AuditLogResponse) SetAuthorEmail(v string)`

SetAuthorEmail sets AuthorEmail field to given value.

### HasAuthorEmail

`func (o *AuditLogResponse) HasAuthorEmail() bool`

HasAuthorEmail returns a boolean if a field has been set.

### SetAuthorEmailNil

`func (o *AuditLogResponse) SetAuthorEmailNil(b bool)`

 SetAuthorEmailNil sets the value for AuthorEmail to be an explicit nil

### UnsetAuthorEmail
`func (o *AuditLogResponse) UnsetAuthorEmail()`

UnsetAuthorEmail ensures that no value is present for AuthorEmail, not even an explicit nil
### GetCorrelationId

`func (o *AuditLogResponse) GetCorrelationId() string`

GetCorrelationId returns the CorrelationId field if non-nil, zero value otherwise.

### GetCorrelationIdOk

`func (o *AuditLogResponse) GetCorrelationIdOk() (*string, bool)`

GetCorrelationIdOk returns a tuple with the CorrelationId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCorrelationId

`func (o *AuditLogResponse) SetCorrelationId(v string)`

SetCorrelationId sets CorrelationId field to given value.

### HasCorrelationId

`func (o *AuditLogResponse) HasCorrelationId() bool`

HasCorrelationId returns a boolean if a field has been set.

### SetCorrelationIdNil

`func (o *AuditLogResponse) SetCorrelationIdNil(b bool)`

 SetCorrelationIdNil sets the value for CorrelationId to be an explicit nil

### UnsetCorrelationId
`func (o *AuditLogResponse) UnsetCorrelationId()`

UnsetCorrelationId ensures that no value is present for CorrelationId, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


