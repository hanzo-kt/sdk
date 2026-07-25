
# DnsRecordCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** |  |  |
| **type** | [**inline**](#Type) |  |  |
| **content** | **kotlin.String** | Record content varies by type: - A: IPv4 address (e.g. 1.2.3.4) - AAAA: IPv6 address - CNAME: Target hostname - MX: Mail server hostname - TXT: Text value (auto-quoted) - SRV: weight port target (priority set separately) - NS: Nameserver hostname - CAA: flags tag value (e.g. 0 issue letsencrypt.org)  |  |
| **ttl** | **kotlin.Int** |  |  [optional] |
| **priority** | **kotlin.Int** | Required for MX and SRV records |  [optional] |
| **proxied** | **kotlin.Boolean** |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | A, AAAA, CNAME, MX, TXT, SRV, NS, CAA |



