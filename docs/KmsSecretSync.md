
# KmsSecretSync

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **destination** | **kotlin.String** | Sync destination (e.g., aws-parameter-store, github) |  [optional] |
| **sourceEnvironment** | **kotlin.String** |  |  [optional] |
| **sourcePath** | **kotlin.String** |  |  [optional] |
| **connectionId** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **isAutoSyncEnabled** | **kotlin.Boolean** |  |  [optional] |
| **lastSyncedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **syncStatus** | [**inline**](#SyncStatus) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="SyncStatus"></a>
## Enum: syncStatus
| Name | Value |
| ---- | ----- |
| syncStatus | succeeded, failed, pending |



