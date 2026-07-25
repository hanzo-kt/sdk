
# ProjectsCompleteDeploymentRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **status** | [**inline**](#Status) | Final status. |  |
| **commit** | **kotlin.String** |  |  [optional] |
| **liveUrl** | **kotlin.String** | Defaults to the project&#39;s canonical live URL when omitted on a live completion. |  [optional] |
| **message** | **kotlin.String** |  |  [optional] |
| **files** | **kotlin.Int** |  |  [optional] |
| **bytes** | **kotlin.Long** |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | live, error |



