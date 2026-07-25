
# AnalyticsTeamUser

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **teamId** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **userId** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **role** | [**inline**](#Role) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **user** | [**AnalyticsUser**](AnalyticsUser.md) |  |  [optional] |


<a id="Role"></a>
## Enum: role
| Name | Value |
| ---- | ----- |
| role | team-member, team-view-only, team-manager, team-owner |



