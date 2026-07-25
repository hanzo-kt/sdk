
# DbOperation

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **projectId** | **kotlin.String** |  |  [optional] |
| **branchId** | **kotlin.String** |  |  [optional] |
| **endpointId** | **kotlin.String** |  |  [optional] |
| **action** | [**inline**](#Action) |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **failuresCount** | **kotlin.Int** |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Action"></a>
## Enum: action
| Name | Value |
| ---- | ----- |
| action | create_project, create_branch, delete_branch, create_endpoint, start_compute, suspend_compute, delete_endpoint, apply_config, check_availability, create_timeline, tenant_migrate |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | scheduling, running, finished, failed, cancelling, cancelled, skipping |



