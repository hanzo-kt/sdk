
# CommerceTransaction

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] [readonly] |
| **destinationId** | **kotlin.String** |  |  [optional] |
| **destinationKind** | **kotlin.String** |  |  [optional] |
| **currency** | **kotlin.String** |  |  [optional] |
| **amount** | **kotlin.Int** |  |  [optional] |
| **type** | [**inline**](#Type) |  |  [optional] |
| **test** | **kotlin.Boolean** |  |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **sourceId** | **kotlin.String** |  |  [optional] |
| **sourceKind** | **kotlin.String** |  |  [optional] |
| **metadata** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] [readonly] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] [readonly] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | hold, hold-removed, transfer, deposit, withdraw |



