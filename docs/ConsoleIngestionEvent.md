
# ConsoleIngestionEvent

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  |
| **type** | [**inline**](#Type) |  |  |
| **timestamp** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **body** | [**kotlin.Any**](.md) |  |  |
| **metadata** | [**kotlin.Any**](.md) |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | trace-create, score-create, span-create, span-update, generation-create, generation-update, event-create, sdk-log |



