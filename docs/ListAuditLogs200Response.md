# ListAuditLogs200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Items** | Pointer to [**[]AuditLogResponse**](AuditLogResponse.md) | List of immutable audit log entries | [optional] 
**Total** | Pointer to **int32** | Total count of matching audit log records | [optional] 

## Methods

### NewListAuditLogs200Response

`func NewListAuditLogs200Response() *ListAuditLogs200Response`

NewListAuditLogs200Response instantiates a new ListAuditLogs200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListAuditLogs200ResponseWithDefaults

`func NewListAuditLogs200ResponseWithDefaults() *ListAuditLogs200Response`

NewListAuditLogs200ResponseWithDefaults instantiates a new ListAuditLogs200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetItems

`func (o *ListAuditLogs200Response) GetItems() []AuditLogResponse`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *ListAuditLogs200Response) GetItemsOk() (*[]AuditLogResponse, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *ListAuditLogs200Response) SetItems(v []AuditLogResponse)`

SetItems sets Items field to given value.

### HasItems

`func (o *ListAuditLogs200Response) HasItems() bool`

HasItems returns a boolean if a field has been set.

### GetTotal

`func (o *ListAuditLogs200Response) GetTotal() int32`

GetTotal returns the Total field if non-nil, zero value otherwise.

### GetTotalOk

`func (o *ListAuditLogs200Response) GetTotalOk() (*int32, bool)`

GetTotalOk returns a tuple with the Total field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTotal

`func (o *ListAuditLogs200Response) SetTotal(v int32)`

SetTotal sets Total field to given value.

### HasTotal

`func (o *ListAuditLogs200Response) HasTotal() bool`

HasTotal returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


