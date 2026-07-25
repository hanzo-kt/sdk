
# O11yLogsResponse

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **product** | **kotlin.String** |  |  [optional] |
| **view** | [**inline**](#View) | infra for a validated SuperAdmin, request for every other org. |  [optional] |
| **lines** | [**kotlin.collections.List&lt;O11yLogLine&gt;**](O11yLogLine.md) |  |  [optional] |
| **nextCursor** | **kotlin.Long** | Max nanosecond cursor. Pass back as sinceNs for the next tail poll. |  [optional] |


<a id="View"></a>
## Enum: view
| Name | Value |
| ---- | ----- |
| view | infra, request |



