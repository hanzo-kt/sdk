
# ConsoleCreateScoreConfigRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** |  |  |
| **dataType** | [**inline**](#DataType) |  |  |
| **categories** | [**kotlin.collections.List&lt;ConsoleCreateScoreConfigRequestCategoriesInner&gt;**](ConsoleCreateScoreConfigRequestCategoriesInner.md) |  |  [optional] |
| **minValue** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **maxValue** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |


<a id="DataType"></a>
## Enum: dataType
| Name | Value |
| ---- | ----- |
| dataType | NUMERIC, CATEGORICAL, BOOLEAN |



