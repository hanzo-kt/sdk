
# CloudAgentsSession

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | Session id (sess_...). |  [optional] |
| **agent** | **kotlin.String** | Agent name/type label (need not be a cloud Agent row). |  [optional] |
| **actor** | **kotlin.String** | The principal that started it. |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **parentSessionId** | **kotlin.String** | Empty for a root (the outer agent). |  [optional] |
| **rootSessionId** | **kotlin.String** | The tree key; equals id for a root. |  [optional] |
| **title** | **kotlin.String** |  |  [optional] |
| **taskWorkflowId** | **kotlin.String** | The hanzoai/tasks workflow that executes this session, when task-backed. |  [optional] |
| **taskRunId** | **kotlin.String** |  |  [optional] |
| **events** | **kotlin.Int** |  |  [optional] |
| **children** | **kotlin.Int** | Direct-child (subagent) fan-out count. |  [optional] |
| **startedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **endedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Set once a terminal status (done/error) is reached. |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | running, paused, done, error |



