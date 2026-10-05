# InboundEndpointOverviewResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Inbound endpoint UUID | 
**Name** | **string** | Endpoint name | 
**Enabled** | **bool** | Whether the endpoint accepts deliveries | 
**Mode** | **string** | How records are written: &#x60;create&#x60;, &#x60;update&#x60; or &#x60;upsert&#x60; by external key | 
**Preset** | **string** | The sender&#39;s signature preset | 
**Url** | **string** | The receive URL configured in the sender | 

## Methods

### NewInboundEndpointOverviewResponse

`func NewInboundEndpointOverviewResponse(id string, name string, enabled bool, mode string, preset string, url string, ) *InboundEndpointOverviewResponse`

NewInboundEndpointOverviewResponse instantiates a new InboundEndpointOverviewResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewInboundEndpointOverviewResponseWithDefaults

`func NewInboundEndpointOverviewResponseWithDefaults() *InboundEndpointOverviewResponse`

NewInboundEndpointOverviewResponseWithDefaults instantiates a new InboundEndpointOverviewResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *InboundEndpointOverviewResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *InboundEndpointOverviewResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *InboundEndpointOverviewResponse) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *InboundEndpointOverviewResponse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *InboundEndpointOverviewResponse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *InboundEndpointOverviewResponse) SetName(v string)`

SetName sets Name field to given value.


### GetEnabled

`func (o *InboundEndpointOverviewResponse) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *InboundEndpointOverviewResponse) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *InboundEndpointOverviewResponse) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.


### GetMode

`func (o *InboundEndpointOverviewResponse) GetMode() string`

GetMode returns the Mode field if non-nil, zero value otherwise.

### GetModeOk

`func (o *InboundEndpointOverviewResponse) GetModeOk() (*string, bool)`

GetModeOk returns a tuple with the Mode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMode

`func (o *InboundEndpointOverviewResponse) SetMode(v string)`

SetMode sets Mode field to given value.


### GetPreset

`func (o *InboundEndpointOverviewResponse) GetPreset() string`

GetPreset returns the Preset field if non-nil, zero value otherwise.

### GetPresetOk

`func (o *InboundEndpointOverviewResponse) GetPresetOk() (*string, bool)`

GetPresetOk returns a tuple with the Preset field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPreset

`func (o *InboundEndpointOverviewResponse) SetPreset(v string)`

SetPreset sets Preset field to given value.


### GetUrl

`func (o *InboundEndpointOverviewResponse) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *InboundEndpointOverviewResponse) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *InboundEndpointOverviewResponse) SetUrl(v string)`

SetUrl sets Url field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


