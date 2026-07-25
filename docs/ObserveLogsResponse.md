
# ObserveLogsResponse

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **product** | **kotlin.String** |  |  [optional] |
| **view** | [**inline**](#View) | \&quot;infra\&quot; (admin) or \&quot;request\&quot; (per-org). |  [optional] |
| **lines** | [**kotlin.collections.List&lt;ObserveLogLine&gt;**](ObserveLogLine.md) |  |  [optional] |
| **nextCursor** | **kotlin.Long** | Pass back as &#x60;sinceNs&#x60; for the next tail poll. |  [optional] |


<a id="View"></a>
## Enum: view
| Name | Value |
| ---- | ----- |
| view | infra, request |



