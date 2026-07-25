
# PaasCreateContainerRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** |  |  |
| **type** | [**inline**](#Type) |  |  |
| **template** | **kotlin.String** | Template slug (nodejs, python, go, rust, etc.) |  [optional] |
| **repo** | [**PaasCreateContainerRequestRepo**](PaasCreateContainerRequestRepo.md) |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | deployment, statefulset, cronjob, knativeservice |



