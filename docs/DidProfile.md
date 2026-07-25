
# DidProfile

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **type** | [**inline**](#Type) |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **email** | **kotlin.String** |  |  [optional] |
| **avatar** | [**java.net.URI**](java.net.URI.md) |  |  [optional] |
| **organization** | **kotlin.String** |  |  [optional] |
| **teams** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  [optional] |
| **metadata** | **kotlin.collections.Map&lt;kotlin.String, kotlin.String&gt;** |  |  [optional] |
| **linkedIdentities** | [**kotlin.collections.List&lt;DidLinkedIdentity&gt;**](DidLinkedIdentity.md) |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | user, service_account, bot |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | active, suspended, deactivated |



