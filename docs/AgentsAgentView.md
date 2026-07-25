
# AgentsAgentView

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **model** | **kotlin.String** |  |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **tools** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **status** | **kotlin.String** |  |  [optional] |
| **executionMode** | [**inline**](#ExecutionMode) |  |  [optional] |
| **schedule** | **kotlin.String** |  |  [optional] |
| **computeRef** | **kotlin.String** |  |  [optional] |
| **serviceAccountId** | **kotlin.String** |  |  [optional] |
| **runs** | **kotlin.Int** | Recorded run count. |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="ExecutionMode"></a>
## Enum: executionMode
| Name | Value |
| ---- | ----- |
| executionMode | one-shot, long-running |



