
# AgentsCreateAgentRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Org-unique name; must match ^[A-Za-z0-9][A-Za-z0-9._-]{0,63}$. |  |
| **model** | **kotlin.String** | Served model id. Validated against the gateway catalog; omit to use the deployment default. |  [optional] |
| **instructions** | **kotlin.String** | System prompt (capped at 32 KiB). |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **tools** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **executionMode** | [**inline**](#ExecutionMode) | Defaults to one-shot when empty. |  [optional] |
| **schedule** | **kotlin.String** | Required 5-field cron for a long-running agent; cleared for one-shot. |  [optional] |
| **computeRef** | **kotlin.String** |  |  [optional] |
| **serviceAccountId** | **kotlin.String** |  |  [optional] |


<a id="ExecutionMode"></a>
## Enum: executionMode
| Name | Value |
| ---- | ----- |
| executionMode | one-shot, long-running |



