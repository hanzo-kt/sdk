
# ConsoleObservation

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **traceId** | **kotlin.String** |  |  [optional] |
| **type** | [**inline**](#Type) |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **startTime** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **endTime** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **completionStartTime** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **model** | **kotlin.String** |  |  [optional] |
| **modelParameters** | [**kotlin.Any**](.md) |  |  [optional] |
| **input** | [**kotlin.Any**](.md) |  |  [optional] |
| **output** | [**kotlin.Any**](.md) |  |  [optional] |
| **metadata** | [**kotlin.Any**](.md) |  |  [optional] |
| **level** | [**inline**](#Level) |  |  [optional] |
| **statusMessage** | **kotlin.String** |  |  [optional] |
| **parentObservationId** | **kotlin.String** |  |  [optional] |
| **version** | **kotlin.String** |  |  [optional] |
| **environment** | **kotlin.String** |  |  [optional] |
| **promptId** | **kotlin.String** |  |  [optional] |
| **promptName** | **kotlin.String** |  |  [optional] |
| **promptVersion** | **kotlin.Int** |  |  [optional] |
| **usage** | [**ConsoleUsage**](ConsoleUsage.md) |  |  [optional] |
| **calculatedInputCost** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **calculatedOutputCost** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **calculatedTotalCost** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **latency** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Latency in seconds |  [optional] |
| **timeToFirstToken** | [**java.math.BigDecimal**](java.math.BigDecimal.md) | Time to first token in seconds |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | GENERATION, SPAN, EVENT |


<a id="Level"></a>
## Enum: level
| Name | Value |
| ---- | ----- |
| level | DEBUG, DEFAULT, WARNING, ERROR |



