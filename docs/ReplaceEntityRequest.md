# ReplaceEntityRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Attributes** | [**map[string]EntityAttributesInputValue**](EntityAttributesInputValue.md) | Map of attribute slug or UUID → value. Keys may be mixed freely in one request; each attribute may appear once.  ### Values - **Plain scalar** — &#x60;\&quot;text\&quot;&#x60;, &#x60;42&#x60;, &#x60;129.99&#x60;, &#x60;true&#x60;, or &#x60;null&#x60;. Numbers and booleans are serialized for you (&#x60;42&#x60; → &#x60;\&quot;42\&quot;&#x60;, &#x60;true&#x60; → &#x60;\&quot;true\&quot;&#x60;); floats keep exactly the digits you sent. - **&#x60;null&#x60;** — clears the attribute. - **Backfill object** — &#x60;{ \&quot;value\&quot;: &lt;scalar|null&gt;, \&quot;updated_at\&quot;: \&quot;2026-09-12T12:23:52Z\&quot; }&#x60; records the value as observed at that moment (history import). &#x60;updated_at&#x60; must be RFC 3339 with an explicit offset (&#x60;Z&#x60; or &#x60;±HH:MM&#x60;); it defaults to now when omitted. - **Operation object** — &#x60;{ \&quot;op\&quot;: \&quot;increment\&quot;, \&quot;value\&quot;: 1 }&#x60; adds the number to the stored value instead of overwriting it: you never need to read the current value, and concurrent increments are serialized so none is lost. Allowed on **Number** attributes and **Metrics** only (a metric increment appends &#x60;latest + value&#x60; as a new observation); a never-set attribute counts as &#x60;0&#x60;; a negative &#x60;value&#x60; subtracts. &#x60;op&#x60; cannot be combined with &#x60;updated_at&#x60;. Not accepted on create. The change log records the resolved value, never the operand.  ### Value format by attribute type - **Text / Markdown**: UTF-8 string - **Number**: number or numeric string (&#x60;129.99&#x60;, &#x60;\&quot;42\&quot;&#x60;) - **Boolean**: &#x60;true&#x60; / &#x60;false&#x60; (or &#x60;\&quot;true\&quot;&#x60; / &#x60;\&quot;false\&quot;&#x60;, &#x60;\&quot;1\&quot;&#x60; / &#x60;\&quot;0\&quot;&#x60;) - **Date**: &#x60;YYYY-MM-DD&#x60;; **Datetime**: &#x60;YYYY-MM-DD HH:MM:SS&#x60; or ISO 8601 &#x60;YYYY-MM-DDTHH:MM:SSZ&#x60; - **File / Image**: UUID of a previously uploaded file asset - **List**: UUID of one of the attribute&#39;s list items - **Reference**: UUID of the referenced entity - **Metric**: numeric observation; appended to the time series (never overwritten)  ### Example &#x60;&#x60;&#x60;json {   \&quot;hostname\&quot;: \&quot;edge-fra-01\&quot;,   \&quot;cpu_cores\&quot;: 8,   \&quot;notes\&quot;: null,   \&quot;operational_status\&quot;: { \&quot;value\&quot;: \&quot;Active\&quot;, \&quot;updated_at\&quot;: \&quot;2026-09-12T12:23:52Z\&quot; },   \&quot;restart_count\&quot;: { \&quot;op\&quot;: \&quot;increment\&quot;, \&quot;value\&quot;: 1 } } &#x60;&#x60;&#x60; | 

## Methods

### NewReplaceEntityRequest

`func NewReplaceEntityRequest(attributes map[string]EntityAttributesInputValue, ) *ReplaceEntityRequest`

NewReplaceEntityRequest instantiates a new ReplaceEntityRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewReplaceEntityRequestWithDefaults

`func NewReplaceEntityRequestWithDefaults() *ReplaceEntityRequest`

NewReplaceEntityRequestWithDefaults instantiates a new ReplaceEntityRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAttributes

`func (o *ReplaceEntityRequest) GetAttributes() map[string]EntityAttributesInputValue`

GetAttributes returns the Attributes field if non-nil, zero value otherwise.

### GetAttributesOk

`func (o *ReplaceEntityRequest) GetAttributesOk() (*map[string]EntityAttributesInputValue, bool)`

GetAttributesOk returns a tuple with the Attributes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAttributes

`func (o *ReplaceEntityRequest) SetAttributes(v map[string]EntityAttributesInputValue)`

SetAttributes sets Attributes field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


