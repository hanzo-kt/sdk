
# MlModel

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **version** | **kotlin.String** |  |  [optional] |
| **stage** | [**inline**](#Stage) |  |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **sourceRunId** | **kotlin.String** | Experiment run that produced this model |  [optional] |
| **artifacts** | [**MlRegisterModelRequestArtifacts**](MlRegisterModelRequestArtifacts.md) |  |  [optional] |
| **metrics** | [**kotlin.collections.Map&lt;kotlin.String, java.math.BigDecimal&gt;**](java.math.BigDecimal.md) |  |  [optional] |
| **tags** | **kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt;** |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Stage"></a>
## Enum: stage
| Name | Value |
| ---- | ----- |
| stage | dev, staging, canary, production |



