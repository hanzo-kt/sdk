
# BotSkill

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **slug** | **kotlin.String** | URL-safe unique identifier |  [optional] |
| **displayName** | **kotlin.String** |  |  [optional] |
| **summary** | **kotlin.String** |  |  [optional] |
| **ownerUserId** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **forkOf** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **latestVersionId** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **tags** | [**kotlin.Any**](.md) |  |  [optional] |
| **badges** | [**kotlin.Any**](.md) |  |  [optional] |
| **batch** | **kotlin.String** | Grouping key (e.g. \&quot;integration\&quot;) |  [optional] |
| **moderationStatus** | [**inline**](#ModerationStatus) |  |  [optional] |
| **quality** | [**kotlin.Any**](.md) |  |  [optional] |
| **statsDownloads** | **kotlin.Int** |  |  [optional] |
| **statsStars** | **kotlin.Int** |  |  [optional] |
| **statsVersions** | **kotlin.Int** |  |  [optional] |
| **statsComments** | **kotlin.Int** |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **ownerHandle** | **kotlin.String** |  |  [optional] |
| **ownerImage** | **kotlin.String** |  |  [optional] |


<a id="ModerationStatus"></a>
## Enum: moderationStatus
| Name | Value |
| ---- | ----- |
| moderationStatus | active, pending, rejected |



