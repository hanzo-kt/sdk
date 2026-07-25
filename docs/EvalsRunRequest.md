
# EvalsRunRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **dataset** | **kotlin.String** |  |  |
| **model** | **kotlin.String** | Model-under-test (catalog / fine-tuned / BYOM / router) |  |
| **runName** | **kotlin.String** |  |  [optional] |
| **limit** | **kotlin.Int** |  |  [optional] |
| **judge** | [**EvalsJudgeSpec**](EvalsJudgeSpec.md) |  |  [optional] |
| **metrics** | [**kotlin.collections.List&lt;EvalsMetric&gt;**](EvalsMetric.md) |  |  [optional] |
| **backend** | [**inline**](#Backend) | Evaluation backend — native Hanzo engine or DigitalOcean GenAI |  [optional] |
| **preset** | **kotlin.String** | Named preset to reuse a saved configuration |  [optional] |


<a id="Backend"></a>
## Enum: backend
| Name | Value |
| ---- | ----- |
| backend | hanzo, do |



