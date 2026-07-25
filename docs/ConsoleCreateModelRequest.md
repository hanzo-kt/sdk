
# ConsoleCreateModelRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **modelName** | **kotlin.String** |  |  |
| **matchPattern** | **kotlin.String** |  |  |
| **startDate** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **unit** | [**inline**](#Unit) |  |  [optional] |
| **inputPrice** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **outputPrice** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **totalPrice** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **tokenizerId** | **kotlin.String** |  |  [optional] |
| **tokenizerConfig** | [**kotlin.Any**](.md) |  |  [optional] |


<a id="Unit"></a>
## Enum: unit
| Name | Value |
| ---- | ----- |
| unit | TOKENS, CHARACTERS, MILLISECONDS, SECONDS, IMAGES, REQUESTS |



