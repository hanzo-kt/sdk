
# EdgeFunction

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **slug** | **kotlin.String** | URL-safe function identifier |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **version** | **kotlin.Int** | Current deployed version number |  [optional] |
| **runtime** | [**inline**](#Runtime) |  |  [optional] |
| **entrypoint** | **kotlin.String** |  |  [optional] |
| **importMap** | **kotlin.Boolean** |  |  [optional] |
| **verifyJwt** | **kotlin.Boolean** | Whether to verify JWT tokens on invocation |  [optional] |
| **invokeUrl** | [**java.net.URI**](java.net.URI.md) | Public invocation URL |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | active, inactive, deploying, failed |


<a id="Runtime"></a>
## Enum: runtime
| Name | Value |
| ---- | ----- |
| runtime | deno, node |



