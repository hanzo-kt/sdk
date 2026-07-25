
# AnalyticsAdminListUsers200ResponseInner

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **username** | **kotlin.String** |  |  [optional] |
| **role** | [**inline**](#Role) |  |  [optional] |
| **logoUrl** | **kotlin.String** |  |  [optional] |
| **displayName** | **kotlin.String** |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **deletedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **count** | [**AnalyticsAdminListUsers200ResponseInnerAllOfCount**](AnalyticsAdminListUsers200ResponseInnerAllOfCount.md) |  |  [optional] |


<a id="Role"></a>
## Enum: role
| Name | Value |
| ---- | ----- |
| role | admin, user, view-only |



