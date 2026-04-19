# ValidationErrorResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Type** | **string** |  | 
**Title** | **string** |  | 
**Status** | **int32** |  | 
**Errors** | **map[string][]string** | Map of field names to array of error messages | 

## Methods

### NewValidationErrorResponse

`func NewValidationErrorResponse(type_ string, title string, status int32, errors map[string][]string, ) *ValidationErrorResponse`

NewValidationErrorResponse instantiates a new ValidationErrorResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewValidationErrorResponseWithDefaults

`func NewValidationErrorResponseWithDefaults() *ValidationErrorResponse`

NewValidationErrorResponseWithDefaults instantiates a new ValidationErrorResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetType

`func (o *ValidationErrorResponse) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *ValidationErrorResponse) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *ValidationErrorResponse) SetType(v string)`

SetType sets Type field to given value.


### GetTitle

`func (o *ValidationErrorResponse) GetTitle() string`

GetTitle returns the Title field if non-nil, zero value otherwise.

### GetTitleOk

`func (o *ValidationErrorResponse) GetTitleOk() (*string, bool)`

GetTitleOk returns a tuple with the Title field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTitle

`func (o *ValidationErrorResponse) SetTitle(v string)`

SetTitle sets Title field to given value.


### GetStatus

`func (o *ValidationErrorResponse) GetStatus() int32`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *ValidationErrorResponse) GetStatusOk() (*int32, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *ValidationErrorResponse) SetStatus(v int32)`

SetStatus sets Status field to given value.


### GetErrors

`func (o *ValidationErrorResponse) GetErrors() map[string][]string`

GetErrors returns the Errors field if non-nil, zero value otherwise.

### GetErrorsOk

`func (o *ValidationErrorResponse) GetErrorsOk() (*map[string][]string, bool)`

GetErrorsOk returns a tuple with the Errors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetErrors

`func (o *ValidationErrorResponse) SetErrors(v map[string][]string)`

SetErrors sets Errors field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


