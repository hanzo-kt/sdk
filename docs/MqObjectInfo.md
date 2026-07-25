
# MqObjectInfo

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Object name. |  [optional] |
| **description** | **kotlin.String** | Optional description. |  [optional] |
| **propertySize** | **kotlin.Long** | Object size in bytes. |  [optional] |
| **chunks** | **kotlin.Int** | Number of chunks. |  [optional] |
| **digest** | **kotlin.String** | SHA-256 digest of the object. |  [optional] |
| **modified** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Last modification timestamp. |  [optional] |
| **deleted** | **kotlin.Boolean** | True if the object has been deleted. |  [optional] |
| **headers** | **kotlin.collections.Map&lt;kotlin.String, kotlin.collections.List&lt;kotlin.String&gt;&gt;** | Optional metadata headers. |  [optional] |



