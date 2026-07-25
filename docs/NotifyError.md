
# NotifyError

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **status** | [**inline**](#Status) | Always \&quot;error\&quot; for error responses |  |
| **msg** | **kotlin.String** | Human-readable error message |  |
| **code** | **kotlin.Int** | Application-specific error code |  [optional] |
| **&#x60;data&#x60;** | [**kotlin.Any**](.md) | Additional error context |  [optional] |
| **data2** | [**kotlin.Any**](.md) | Additional error details |  [optional] |
| **requestId** | **kotlin.String** | Request ID for debugging |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | error |



