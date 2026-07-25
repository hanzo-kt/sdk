
# MqKVEntry

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **key** | **kotlin.String** | Key name. |  [optional] |
| **&#x60;value&#x60;** | **kotlin.String** | Value (base64-encoded for binary data). |  [optional] |
| **revision** | **kotlin.Int** | Revision number. |  [optional] |
| **created** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Timestamp of this revision. |  [optional] |
| **operation** | [**inline**](#Operation) | Operation that produced this revision. &#x60;delete&#x60; is a tombstone. &#x60;purge&#x60; removes all prior revisions.  |  [optional] |
| **bucket** | **kotlin.String** | Bucket name. |  [optional] |
| **delta** | **kotlin.Int** | Number of revisions since this entry (for watch operations).  |  [optional] |


<a id="Operation"></a>
## Enum: operation
| Name | Value |
| ---- | ----- |
| operation | put, delete, purge |



