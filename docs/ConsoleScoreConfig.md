
# ConsoleScoreConfig

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **dataType** | [**inline**](#DataType) |  |  [optional] |
| **categories** | [**kotlin.collections.List&lt;ConsoleCreateScoreConfigRequestCategoriesInner&gt;**](ConsoleCreateScoreConfigRequestCategoriesInner.md) |  |  [optional] |
| **minValue** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **maxValue** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **isArchived** | **kotlin.Boolean** |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="DataType"></a>
## Enum: dataType
| Name | Value |
| ---- | ----- |
| dataType | NUMERIC, CATEGORICAL, BOOLEAN |



