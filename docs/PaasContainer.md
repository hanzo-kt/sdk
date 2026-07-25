
# PaasContainer

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **iid** | **kotlin.String** |  |  [optional] |
| **orgId** | **kotlin.String** |  |  [optional] |
| **projectId** | **kotlin.String** |  |  [optional] |
| **envId** | **kotlin.String** |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **type** | [**inline**](#Type) |  |  [optional] |
| **status** | [**PaasContainerStatus**](PaasContainerStatus.md) |  |  [optional] |
| **template** | **kotlin.String** | Template slug (e.g. nodejs, python, go, rust) |  [optional] |
| **repo** | [**PaasContainerRepo**](PaasContainerRepo.md) |  |  [optional] |
| **networking** | [**PaasContainerNetworking**](PaasContainerNetworking.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | deployment, statefulset, cronjob, knativeservice |



