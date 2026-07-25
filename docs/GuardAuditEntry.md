
# GuardAuditEntry

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **timestamp** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **userId** | **kotlin.String** |  |  [optional] |
| **sessionId** | **kotlin.String** |  |  [optional] |
| **sourceIp** | **kotlin.String** |  |  [optional] |
| **direction** | [**inline**](#Direction) |  |  [optional] |
| **result** | [**inline**](#Result) |  |  [optional] |
| **redactionCount** | **kotlin.Int** |  |  [optional] |
| **injectionDetected** | **kotlin.Boolean** |  |  [optional] |
| **injectionConfidence** | **kotlin.Float** |  |  [optional] |
| **contentCategory** | **kotlin.String** |  |  [optional] |
| **contentHash** | **kotlin.String** | SHA-256 hash of original content |  [optional] |
| **processingTimeUs** | **kotlin.Int** |  |  [optional] |


<a id="Direction"></a>
## Enum: direction
| Name | Value |
| ---- | ----- |
| direction | input, output |


<a id="Result"></a>
## Enum: result
| Name | Value |
| ---- | ----- |
| result | clean, redacted, blocked |



