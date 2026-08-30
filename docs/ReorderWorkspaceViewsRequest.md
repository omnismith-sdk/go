# ReorderWorkspaceViewsRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ViewIds** | **[]string** | Ordered array of view unique identifiers (UUIDs) defining the new pane sequence | 

## Methods

### NewReorderWorkspaceViewsRequest

`func NewReorderWorkspaceViewsRequest(viewIds []string, ) *ReorderWorkspaceViewsRequest`

NewReorderWorkspaceViewsRequest instantiates a new ReorderWorkspaceViewsRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReorderWorkspaceViewsRequestWithDefaults

`func NewReorderWorkspaceViewsRequestWithDefaults() *ReorderWorkspaceViewsRequest`

NewReorderWorkspaceViewsRequestWithDefaults instantiates a new ReorderWorkspaceViewsRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetViewIds

`func (o *ReorderWorkspaceViewsRequest) GetViewIds() []string`

GetViewIds returns the ViewIds field if non-nil, zero value otherwise.

### GetViewIdsOk

`func (o *ReorderWorkspaceViewsRequest) GetViewIdsOk() (*[]string, bool)`

GetViewIdsOk returns a tuple with the ViewIds field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetViewIds

`func (o *ReorderWorkspaceViewsRequest) SetViewIds(v []string)`

SetViewIds sets ViewIds field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


