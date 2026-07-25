
# CloudAgentsAgent

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | Public handle (agent_...). |  [optional] |
| **name** | **kotlin.String** | Org-unique name matching ^[A-Za-z0-9][A-Za-z0-9._-]{0,63}$. |  [optional] |
| **model** | **kotlin.String** |  |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **tools** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **status** | **kotlin.String** |  |  [optional] |
| **executionMode** | [**inline**](#ExecutionMode) |  |  [optional] |
| **schedule** | **kotlin.String** | 5-field cron; required and evaluated only when long-running. |  [optional] |
| **computeRef** | **kotlin.String** | Optional visor machine id the bot is bound to. |  [optional] |
| **serviceAccountId** | **kotlin.String** | Optional IAM agent service-account (&lt;org&gt;-&lt;agent&gt;) recorded as the actor on scheduled-run billing. |  [optional] |
| **runs** | **kotlin.Int** | Recorded run count. |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="ExecutionMode"></a>
## Enum: executionMode
| Name | Value |
| ---- | ----- |
| executionMode | one-shot, long-running |



