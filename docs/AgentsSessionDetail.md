
# AgentsSessionDetail

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **agent** | **kotlin.String** |  |  [optional] |
| **actor** | **kotlin.String** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **parentSessionId** | **kotlin.String** |  |  [optional] |
| **rootSessionId** | **kotlin.String** |  |  [optional] |
| **title** | **kotlin.String** |  |  [optional] |
| **taskWorkflowId** | **kotlin.String** |  |  [optional] |
| **taskRunId** | **kotlin.String** |  |  [optional] |
| **events** | **kotlin.Int** |  |  [optional] |
| **children** | **kotlin.Int** | Direct fan-out count. |  [optional] |
| **startedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **endedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **childSessions** | [**kotlin.collections.List&lt;AgentsSessionView&gt;**](AgentsSessionView.md) |  |  [optional] |
| **recentEvents** | [**kotlin.collections.List&lt;AgentsEventView&gt;**](AgentsEventView.md) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | running, paused, done, error |



