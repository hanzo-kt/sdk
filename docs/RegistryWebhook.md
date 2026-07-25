
# RegistryWebhook

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.Int** |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **projectId** | **kotlin.Int** |  |  [optional] |
| **enabled** | **kotlin.Boolean** |  |  [optional] |
| **eventTypes** | [**inline**](#kotlin.collections.List&lt;EventTypes&gt;) |  |  [optional] |
| **targets** | [**kotlin.collections.List&lt;RegistryWebhookTargetsInner&gt;**](RegistryWebhookTargetsInner.md) |  |  [optional] |
| **creationTime** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="kotlin.collections.List<EventTypes>"></a>
## Enum: event_types
| Name | Value |
| ---- | ----- |
| eventTypes | PUSH_ARTIFACT, PULL_ARTIFACT, DELETE_ARTIFACT, SCANNING_COMPLETED, SCANNING_FAILED, QUOTA_EXCEEDED |



