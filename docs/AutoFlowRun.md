
# AutoFlowRun

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **projectId** | **kotlin.String** |  |  [optional] |
| **flowId** | **kotlin.String** |  |  [optional] |
| **flowVersionId** | **kotlin.String** |  |  [optional] |
| **flowDisplayName** | **kotlin.String** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **startTime** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **finishTime** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **duration** | **kotlin.Int** |  |  [optional] |
| **tags** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **created** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updated** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | RUNNING, SUCCEEDED, FAILED, TIMEOUT, PAUSED, STOPPED, INTERNAL_ERROR, QUOTA_EXCEEDED |



