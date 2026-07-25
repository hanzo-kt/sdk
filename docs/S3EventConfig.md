
# S3EventConfig

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **events** | [**inline**](#kotlin.collections.List&lt;Events&gt;) |  |  [optional] |
| **filter** | [**S3EventConfigFilter**](S3EventConfigFilter.md) |  |  [optional] |
| **destination** | [**S3EventConfigDestination**](S3EventConfigDestination.md) |  |  [optional] |


<a id="kotlin.collections.List<Events>"></a>
## Enum: events
| Name | Value |
| ---- | ----- |
| events | s3:ObjectCreated:*, s3:ObjectRemoved:*, s3:ObjectAccessed:* |



