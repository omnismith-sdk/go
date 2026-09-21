# BatchOperationInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Op** | **string** | Which write to perform for this entry. | 
**Id** | Pointer to **NullableString** | Entity identifier to act on. Required for update, replace, and delete. Optional on create (client-assigned UUIDv7). | [optional] 
**Template** | Pointer to **NullableString** | Template UUID or slug to instantiate on create. Forbidden on other operations. | [optional] 
**Attributes** | Pointer to [**map[string]EntityAttributesInputValue**](EntityAttributesInputValue.md) | Map of attribute slug or UUID → value. Keys may be mixed freely in one request; each attribute may appear once.  ### Values - **Plain scalar** — &#x60;\&quot;text\&quot;&#x60;, &#x60;42&#x60;, &#x60;129.99&#x60;, &#x60;true&#x60;, or &#x60;null&#x60;. Numbers and booleans are serialized for you (&#x60;42&#x60; → &#x60;\&quot;42\&quot;&#x60;, &#x60;true&#x60; → &#x60;\&quot;true\&quot;&#x60;); floats keep exactly the digits you sent. - **&#x60;null&#x60;** — clears the attribute. - **Backfill object** — &#x60;{ \&quot;value\&quot;: &lt;scalar|null&gt;, \&quot;updated_at\&quot;: \&quot;2026-09-12T12:23:52Z\&quot; }&#x60; records the value as observed at that moment (history import). &#x60;updated_at&#x60; must be RFC 3339 with an explicit offset (&#x60;Z&#x60; or &#x60;±HH:MM&#x60;); it defaults to now when omitted. - **Operation object** — &#x60;{ \&quot;op\&quot;: \&quot;increment\&quot;, \&quot;value\&quot;: 1 }&#x60; adds the number to the stored value instead of overwriting it: you never need to read the current value, and concurrent increments are serialized so none is lost. Allowed on **Number** attributes and **Metrics** only (a metric increment appends &#x60;latest + value&#x60; as a new observation); a never-set attribute counts as &#x60;0&#x60;; a negative &#x60;value&#x60; subtracts. &#x60;op&#x60; cannot be combined with &#x60;updated_at&#x60;. Not accepted on create. The change log records the resolved value, never the operand.  ### Value format by attribute type - **Text / Markdown**: UTF-8 string - **Number**: number or numeric string (&#x60;129.99&#x60;, &#x60;\&quot;42\&quot;&#x60;) - **Boolean**: &#x60;true&#x60; / &#x60;false&#x60; (or &#x60;\&quot;true\&quot;&#x60; / &#x60;\&quot;false\&quot;&#x60;, &#x60;\&quot;1\&quot;&#x60; / &#x60;\&quot;0\&quot;&#x60;) - **Date**: &#x60;YYYY-MM-DD&#x60;; **Datetime**: &#x60;YYYY-MM-DD HH:MM:SS&#x60; or ISO 8601 &#x60;YYYY-MM-DDTHH:MM:SSZ&#x60; - **File / Image**: UUID of a previously uploaded file asset - **List**: UUID of one of the attribute&#39;s list items - **Reference**: UUID of the referenced entity - **Metric**: numeric observation; appended to the time series (never overwritten)  ### Example &#x60;&#x60;&#x60;json {   \&quot;hostname\&quot;: \&quot;edge-fra-01\&quot;,   \&quot;cpu_cores\&quot;: 8,   \&quot;notes\&quot;: null,   \&quot;operational_status\&quot;: { \&quot;value\&quot;: \&quot;Active\&quot;, \&quot;updated_at\&quot;: \&quot;2026-09-12T12:23:52Z\&quot; },   \&quot;restart_count\&quot;: { \&quot;op\&quot;: \&quot;increment\&quot;, \&quot;value\&quot;: 1 } } &#x60;&#x60;&#x60; | [optional] 

## Methods

### NewBatchOperationInput

`func NewBatchOperationInput(op string, ) *BatchOperationInput`

NewBatchOperationInput instantiates a new BatchOperationInput object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewBatchOperationInputWithDefaults

`func NewBatchOperationInputWithDefaults() *BatchOperationInput`

NewBatchOperationInputWithDefaults instantiates a new BatchOperationInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetOp

`func (o *BatchOperationInput) GetOp() string`

GetOp returns the Op field if non-nil, zero value otherwise.

### GetOpOk

`func (o *BatchOperationInput) GetOpOk() (*string, bool)`

GetOpOk returns a tuple with the Op field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOp

`func (o *BatchOperationInput) SetOp(v string)`

SetOp sets Op field to given value.


### GetId

`func (o *BatchOperationInput) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *BatchOperationInput) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *BatchOperationInput) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *BatchOperationInput) HasId() bool`

HasId returns a boolean if a field has been set.

### SetIdNil

`func (o *BatchOperationInput) SetIdNil(b bool)`

 SetIdNil sets the value for Id to be an explicit nil

### UnsetId
`func (o *BatchOperationInput) UnsetId()`

UnsetId ensures that no value is present for Id, not even an explicit nil
### GetTemplate

`func (o *BatchOperationInput) GetTemplate() string`

GetTemplate returns the Template field if non-nil, zero value otherwise.

### GetTemplateOk

`func (o *BatchOperationInput) GetTemplateOk() (*string, bool)`

GetTemplateOk returns a tuple with the Template field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplate

`func (o *BatchOperationInput) SetTemplate(v string)`

SetTemplate sets Template field to given value.

### HasTemplate

`func (o *BatchOperationInput) HasTemplate() bool`

HasTemplate returns a boolean if a field has been set.

### SetTemplateNil

`func (o *BatchOperationInput) SetTemplateNil(b bool)`

 SetTemplateNil sets the value for Template to be an explicit nil

### UnsetTemplate
`func (o *BatchOperationInput) UnsetTemplate()`

UnsetTemplate ensures that no value is present for Template, not even an explicit nil
### GetAttributes

`func (o *BatchOperationInput) GetAttributes() map[string]EntityAttributesInputValue`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *BatchOperationInput) GetAttributesOk() (*map[string]EntityAttributesInputValue, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *BatchOperationInput) SetAttributes(v map[string]EntityAttributesInputValue)`

SetAttributes sets Attributes field to given value.

### HasAttributes

`func (o *BatchOperationInput) HasAttributes() bool`

HasAttributes returns a boolean if a field has been set.

### SetAttributesNil

`func (o *BatchOperationInput) SetAttributesNil(b bool)`

 SetAttributesNil sets the value for Attributes to be an explicit nil

### UnsetAttributes
`func (o *BatchOperationInput) UnsetAttributes()`

UnsetAttributes ensures that no value is present for Attributes, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


