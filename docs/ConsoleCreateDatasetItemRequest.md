
# ConsoleCreateDatasetItemRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **datasetName** | **kotlin.String** |  |  |
| **input** | [**kotlin.Any**](.md) |  |  [optional] |
| **expectedOutput** | [**kotlin.Any**](.md) |  |  [optional] |
| **metadata** | [**kotlin.Any**](.md) |  |  [optional] |
| **sourceTraceId** | **kotlin.String** |  |  [optional] |
| **sourceObservationId** | **kotlin.String** |  |  [optional] |
| **id** | **kotlin.String** | Upsert key. Must be unique within the project. |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | ACTIVE, ARCHIVED |



