
# CloudAgentsCreateAgentRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Org-unique name matching ^[A-Za-z0-9][A-Za-z0-9._-]{0,63}$. |  |
| **model** | **kotlin.String** |  |  |
| **instructions** | **kotlin.String** | System prompt (max 32 KiB). |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **tools** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **executionMode** | [**inline**](#ExecutionMode) | Defaults to one-shot. |  [optional] |
| **schedule** | **kotlin.String** | 5-field cron; required when executionMode is long-running. |  [optional] |
| **computeRef** | **kotlin.String** |  |  [optional] |
| **serviceAccountId** | **kotlin.String** |  |  [optional] |


<a id="ExecutionMode"></a>
## Enum: executionMode
| Name | Value |
| ---- | ----- |
| executionMode | one-shot, long-running |



