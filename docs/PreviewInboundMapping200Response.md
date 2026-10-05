# PreviewInboundMapping200Response

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Mode** | **string** |  | 
**Matched** | **bool** | Whether the &#x60;match&#x60; conditions hold. When they do not, a real delivery is acknowledged and skipped. | 
**Skipped** | **NullableString** | &#x60;match&#x60; when the conditions do not hold, &#x60;no_items&#x60; when the &#x60;items&#x60; list is empty; null when records would be written. | 
**Items** | [**[]PreviewInboundMapping200ResponseItemsInner**](PreviewInboundMapping200ResponseItemsInner.md) |  | 
**Errors** | **map[string][]string** | Every record error by field, &#x60;items[i].attributes.&lt;slug&gt;&#x60; &#x3D;&gt; messages | 

## Methods

### NewPreviewInboundMapping200Response

`func NewPreviewInboundMapping200Response(mode string, matched bool, skipped NullableString, items []PreviewInboundMapping200ResponseItemsInner, errors map[string][]string, ) *PreviewInboundMapping200Response`

NewPreviewInboundMapping200Response instantiates a new PreviewInboundMapping200Response object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPreviewInboundMapping200ResponseWithDefaults

`func NewPreviewInboundMapping200ResponseWithDefaults() *PreviewInboundMapping200Response`

NewPreviewInboundMapping200ResponseWithDefaults instantiates a new PreviewInboundMapping200Response object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetMode

`func (o *PreviewInboundMapping200Response) GetMode() string`

GetMode returns the Mode field if non-nil, zero value otherwise.

### GetModeOk

`func (o *PreviewInboundMapping200Response) GetModeOk() (*string, bool)`

GetModeOk returns a tuple with the Mode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMode

`func (o *PreviewInboundMapping200Response) SetMode(v string)`

SetMode sets Mode field to given value.


### GetMatched

`func (o *PreviewInboundMapping200Response) GetMatched() bool`

GetMatched returns the Matched field if non-nil, zero value otherwise.

### GetMatchedOk

`func (o *PreviewInboundMapping200Response) GetMatchedOk() (*bool, bool)`

GetMatchedOk returns a tuple with the Matched field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMatched

`func (o *PreviewInboundMapping200Response) SetMatched(v bool)`

SetMatched sets Matched field to given value.


### GetSkipped

`func (o *PreviewInboundMapping200Response) GetSkipped() string`

GetSkipped returns the Skipped field if non-nil, zero value otherwise.

### GetSkippedOk

`func (o *PreviewInboundMapping200Response) GetSkippedOk() (*string, bool)`

GetSkippedOk returns a tuple with the Skipped field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSkipped

`func (o *PreviewInboundMapping200Response) SetSkipped(v string)`

SetSkipped sets Skipped field to given value.


### SetSkippedNil

`func (o *PreviewInboundMapping200Response) SetSkippedNil(b bool)`

 SetSkippedNil sets the value for Skipped to be an explicit nil

### UnsetSkipped
`func (o *PreviewInboundMapping200Response) UnsetSkipped()`

UnsetSkipped ensures that no value is present for Skipped, not even an explicit nil
### GetItems

`func (o *PreviewInboundMapping200Response) GetItems() []PreviewInboundMapping200ResponseItemsInner`

GetItems returns the Items field if non-nil, zero value otherwise.

### GetItemsOk

`func (o *PreviewInboundMapping200Response) GetItemsOk() (*[]PreviewInboundMapping200ResponseItemsInner, bool)`

GetItemsOk returns a tuple with the Items field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetItems

`func (o *PreviewInboundMapping200Response) SetItems(v []PreviewInboundMapping200ResponseItemsInner)`

SetItems sets Items field to given value.


### GetErrors

`func (o *PreviewInboundMapping200Response) GetErrors() map[string][]string`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *PreviewInboundMapping200Response) GetErrorsOk() (*map[string][]string, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *PreviewInboundMapping200Response) SetErrors(v map[string][]string)`

SetErrors sets Errors field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


