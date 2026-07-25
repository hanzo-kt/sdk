
# PubsubKVEntry

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **key** | **kotlin.String** |  |  [optional] |
| **&#x60;value&#x60;** | **kotlin.String** | Base64-encoded value |  [optional] |
| **revision** | **kotlin.Int** |  |  [optional] |
| **created** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **operation** | [**inline**](#Operation) |  |  [optional] |


<a id="Operation"></a>
## Enum: operation
| Name | Value |
| ---- | ----- |
| operation | PUT, DEL, PURGE |



