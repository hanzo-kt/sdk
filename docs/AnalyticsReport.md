
# AnalyticsReport

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **userId** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **websiteId** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **type** | [**inline**](#Type) |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **parameters** | [**kotlin.Any**](.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | funnel, insights, retention, utm, goals, journey, revenue, attribution |



