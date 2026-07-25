
# AnalyticsRunGoalsReportRequestGoalsInner

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **type** | [**inline**](#Type) |  |  |
| **&#x60;value&#x60;** | **kotlin.String** |  |  |
| **goal** | [**java.math.BigDecimal**](java.math.BigDecimal.md) |  |  |
| **&#x60;operator&#x60;** | [**inline**](#&#x60;Operator&#x60;) | Required when type is event-data |  [optional] |
| **&#x60;property&#x60;** | **kotlin.String** | Required when type is event-data |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | url, event, event-data |


<a id="`Operator`"></a>
## Enum: operator
| Name | Value |
| ---- | ----- |
| &#x60;operator&#x60; | count, sum, average |



