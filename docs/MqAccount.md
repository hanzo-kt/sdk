
# MqAccount

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | Account ID. |  [optional] |
| **orgId** | **kotlin.String** | Hanzo IAM organization ID. |  [optional] |
| **name** | **kotlin.String** | Account display name. |  [optional] |
| **connections** | **kotlin.Int** | Number of active connections. |  [optional] |
| **subscriptions** | **kotlin.Int** | Number of active subscriptions. |  [optional] |
| **dataIn** | **kotlin.Long** | Total bytes received. |  [optional] |
| **dataOut** | **kotlin.Long** | Total bytes sent. |  [optional] |
| **slowConsumers** | **kotlin.Int** | Number of slow consumers. |  [optional] |
| **streams** | **kotlin.Int** | Number of JetStream streams. |  [optional] |
| **consumers** | **kotlin.Int** | Number of JetStream consumers. |  [optional] |
| **limits** | [**MqAccountLimits**](MqAccountLimits.md) |  |  [optional] |



