
# AgentsRegisterSessionRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **agent** | **kotlin.String** | Agent label (max 128 chars). |  |
| **actor** | **kotlin.String** | Defaults to the validated principal (org/sub). |  [optional] |
| **title** | **kotlin.String** |  |  [optional] |
| **status** | [**inline**](#Status) | Defaults to running. |  [optional] |
| **parentSessionId** | **kotlin.String** | Parent session id in the same org (for subagent linkage). |  [optional] |
| **taskWorkflowId** | **kotlin.String** |  |  [optional] |
| **taskRunId** | **kotlin.String** |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | running, paused, done, error |



