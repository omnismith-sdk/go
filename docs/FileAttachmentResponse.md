# FileAttachmentResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**OriginalFilename** | Pointer to **string** |  | [optional] 
**MimeType** | Pointer to **string** |  | [optional] 
**Size** | Pointer to **int32** |  | [optional] 
**Context** | Pointer to **NullableString** |  | [optional] 
**ExpiresAt** | Pointer to **NullableTime** |  | [optional] 

## Methods

### NewFileAttachmentResponse

`func NewFileAttachmentResponse() *FileAttachmentResponse`

NewFileAttachmentResponse instantiates a new FileAttachmentResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewFileAttachmentResponseWithDefaults

`func NewFileAttachmentResponseWithDefaults() *FileAttachmentResponse`

NewFileAttachmentResponseWithDefaults instantiates a new FileAttachmentResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *FileAttachmentResponse) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *FileAttachmentResponse) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *FileAttachmentResponse) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *FileAttachmentResponse) HasId() bool`

HasId returns a boolean if a field has been set.

### GetOriginalFilename

`func (o *FileAttachmentResponse) GetOriginalFilename() string`

GetOriginalFilename returns the OriginalFilename field if non-nil, zero value otherwise.

### GetOriginalFilenameOk

`func (o *FileAttachmentResponse) GetOriginalFilenameOk() (*string, bool)`

GetOriginalFilenameOk returns a tuple with the OriginalFilename field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOriginalFilename

`func (o *FileAttachmentResponse) SetOriginalFilename(v string)`

SetOriginalFilename sets OriginalFilename field to given value.

### HasOriginalFilename

`func (o *FileAttachmentResponse) HasOriginalFilename() bool`

HasOriginalFilename returns a boolean if a field has been set.

### GetMimeType

`func (o *FileAttachmentResponse) GetMimeType() string`

GetMimeType returns the MimeType field if non-nil, zero value otherwise.

### GetMimeTypeOk

`func (o *FileAttachmentResponse) GetMimeTypeOk() (*string, bool)`

GetMimeTypeOk returns a tuple with the MimeType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMimeType

`func (o *FileAttachmentResponse) SetMimeType(v string)`

SetMimeType sets MimeType field to given value.

### HasMimeType

`func (o *FileAttachmentResponse) HasMimeType() bool`

HasMimeType returns a boolean if a field has been set.

### GetSize

`func (o *FileAttachmentResponse) GetSize() int32`

GetSize returns the Size field if non-nil, zero value otherwise.

### GetSizeOk

`func (o *FileAttachmentResponse) GetSizeOk() (*int32, bool)`

GetSizeOk returns a tuple with the Size field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSize

`func (o *FileAttachmentResponse) SetSize(v int32)`

SetSize sets Size field to given value.

### HasSize

`func (o *FileAttachmentResponse) HasSize() bool`

HasSize returns a boolean if a field has been set.

### GetContext

`func (o *FileAttachmentResponse) GetContext() string`

GetContext returns the Context field if non-nil, zero value otherwise.

### GetContextOk

`func (o *FileAttachmentResponse) GetContextOk() (*string, bool)`

GetContextOk returns a tuple with the Context field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetContext

`func (o *FileAttachmentResponse) SetContext(v string)`

SetContext sets Context field to given value.

### HasContext

`func (o *FileAttachmentResponse) HasContext() bool`

HasContext returns a boolean if a field has been set.

### SetContextNil

`func (o *FileAttachmentResponse) SetContextNil(b bool)`

 SetContextNil sets the value for Context to be an explicit nil

### UnsetContext
`func (o *FileAttachmentResponse) UnsetContext()`

UnsetContext ensures that no value is present for Context, not even an explicit nil
### GetExpiresAt

`func (o *FileAttachmentResponse) GetExpiresAt() time.Time`

GetExpiresAt returns the ExpiresAt field if non-nil, zero value otherwise.

### GetExpiresAtOk

`func (o *FileAttachmentResponse) GetExpiresAtOk() (*time.Time, bool)`

GetExpiresAtOk returns a tuple with the ExpiresAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresAt

`func (o *FileAttachmentResponse) SetExpiresAt(v time.Time)`

SetExpiresAt sets ExpiresAt field to given value.

### HasExpiresAt

`func (o *FileAttachmentResponse) HasExpiresAt() bool`

HasExpiresAt returns a boolean if a field has been set.

### SetExpiresAtNil

`func (o *FileAttachmentResponse) SetExpiresAtNil(b bool)`

 SetExpiresAtNil sets the value for ExpiresAt to be an explicit nil

### UnsetExpiresAt
`func (o *FileAttachmentResponse) UnsetExpiresAt()`

UnsetExpiresAt ensures that no value is present for ExpiresAt, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


