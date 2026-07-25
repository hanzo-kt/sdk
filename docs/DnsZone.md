
# DnsZone

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **zone** | **kotlin.String** | Zone name (e.g. example.com.) |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **nameservers** | **kotlin.collections.List&lt;kotlin.String&gt;** | Assigned authoritative nameservers |  [optional] |
| **soa** | [**DnsSOARecord**](DnsSOARecord.md) |  |  [optional] |
| **recordCount** | **kotlin.Int** |  |  [optional] |
| **dnssecEnabled** | **kotlin.Boolean** |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | active, pending, disabled |



