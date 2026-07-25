
# AutomationsFlowTrigger

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** |  |  [optional] |
| **type** | [**inline**](#Type) |  |  [optional] |
| **displayName** | **kotlin.String** |  |  [optional] |
| **valid** | **kotlin.Boolean** |  |  [optional] |
| **strategy** | [**inline**](#Strategy) |  |  [optional] |
| **settings** | [**AutomationsStepSettings**](AutomationsStepSettings.md) |  |  [optional] |
| **nextAction** | [**AutomationsFlowAction**](AutomationsFlowAction.md) |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | PIECE_TRIGGER, EMPTY |


<a id="Strategy"></a>
## Enum: strategy
| Name | Value |
| ---- | ----- |
| strategy | POLLING, WEBHOOK, APP_WEBHOOK, MANUAL |



