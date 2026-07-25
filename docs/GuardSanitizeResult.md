
# GuardSanitizeResult

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **status** | [**inline**](#Status) | Sanitization result status |  [optional] |
| **text** | **kotlin.String** | Sanitized text (present for clean and redacted) |  [optional] |
| **reason** | **kotlin.String** | Block reason (present only for blocked) |  [optional] |
| **redactions** | [**kotlin.collections.List&lt;GuardSanitizeResultRedactionsInner&gt;**](GuardSanitizeResultRedactionsInner.md) | PII redactions applied |  [optional] |
| **injection** | [**GuardSanitizeResultInjection**](GuardSanitizeResultInjection.md) |  |  [optional] |
| **contentFilter** | [**GuardSanitizeResultContentFilter**](GuardSanitizeResultContentFilter.md) |  |  [optional] |
| **processingTimeUs** | **kotlin.Int** | Processing time in microseconds |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | clean, redacted, blocked |



