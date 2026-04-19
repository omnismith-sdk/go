# SendFeedbackRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Title** | **string** | Feedback subject line | 
**Category** | **string** | Feedback category | 
**Message** | **string** | Detailed feedback message | 

## Methods

### NewSendFeedbackRequest

`func NewSendFeedbackRequest(title string, category string, message string, ) *SendFeedbackRequest`

NewSendFeedbackRequest instantiates a new SendFeedbackRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewSendFeedbackRequestWithDefaults

`func NewSendFeedbackRequestWithDefaults() *SendFeedbackRequest`

NewSendFeedbackRequestWithDefaults instantiates a new SendFeedbackRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTitle

`func (o *SendFeedbackRequest) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *SendFeedbackRequest) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *SendFeedbackRequest) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetCategory

`func (o *SendFeedbackRequest) GetCategory() string`

GetCategory returns the Category field if non-nil, zero value otherwise.

### GetCategoryOk

`func (o *SendFeedbackRequest) GetCategoryOk() (*string, bool)`

GetCategoryOk returns a tuple with the Category field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCategory

`func (o *SendFeedbackRequest) SetCategory(v string)`

SetCategory sets Category field to given value.


### GetMessage

`func (o *SendFeedbackRequest) GetMessage() string`

GetMessage returns the Message field if non-nil, zero value otherwise.

### GetMessageOk

`func (o *SendFeedbackRequest) GetMessageOk() (*string, bool)`

GetMessageOk returns a tuple with the Message field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMessage

`func (o *SendFeedbackRequest) SetMessage(v string)`

SetMessage sets Message field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


