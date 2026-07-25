
# DnsRecord

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **name** | **kotlin.String** | Record name (relative to zone, @ for apex) |  [optional] |
| **type** | [**inline**](#Type) |  |  [optional] |
| **ttl** | **kotlin.Int** |  |  [optional] |
| **content** | **kotlin.String** | Record value |  [optional] |
| **priority** | **kotlin.Int** | Priority (MX, SRV records) |  [optional] |
| **proxied** | **kotlin.Boolean** |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | A, AAAA, CNAME, MX, TXT, SRV, NS, SOA, CAA |



