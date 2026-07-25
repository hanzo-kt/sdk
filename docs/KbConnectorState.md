
# KbConnectorState

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **provider** | **kotlin.String** |  |  [optional] |
| **configured** | **kotlin.Boolean** | Deployment has OAuth credentials for it |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **docCount** | **kotlin.Int** | Ingested kb-source documents from this provider |  [optional] |
| **kind** | [**inline**](#Kind) |  |  [optional] |
| **account** | **kotlin.String** |  |  [optional] |
| **lastSync** | **kotlin.String** |  |  [optional] |
| **error** | **kotlin.String** |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | disconnected, connected, syncing, error |


<a id="Kind"></a>
## Enum: kind
| Name | Value |
| ---- | ----- |
| kind | native, piece |



