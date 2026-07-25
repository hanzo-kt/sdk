
# GuardSanitizeRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **text** | **kotlin.String** | Text to sanitize |  |
| **direction** | [**inline**](#Direction) | Sanitization direction (input runs all 5 stages, output runs PII + content filter) |  [optional] |
| **userId** | **kotlin.String** | User ID for rate limiting and audit |  [optional] |
| **sessionId** | **kotlin.String** | Session ID for audit correlation |  [optional] |
| **config** | [**GuardSanitizeConfig**](GuardSanitizeConfig.md) |  |  [optional] |


<a id="Direction"></a>
## Enum: direction
| Name | Value |
| ---- | ----- |
| direction | input, output |



