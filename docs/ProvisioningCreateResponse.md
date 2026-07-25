
# ProvisioningCreateResponse

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** | Server-generated resource id. |  |
| **kind** | [**inline**](#Kind) |  |  |
| **name** | **kotlin.String** |  |  |
| **status** | **kotlin.String** | Resource status (e.g. \&quot;ready\&quot;, or \&quot;provisioning\&quot; for a dedicated instance still coming up). |  |
| **host** | **kotlin.String** | Customer-facing host (public gateway host, or dedicated instance service). |  |
| **port** | **kotlin.Int** |  |  |
| **database** | **kotlin.String** |  |  |
| **connectionString** | **kotlin.String** | Public, routable DSN (internal admin host is remapped out). |  |
| **username** | **kotlin.String** | Present only for secretful kinds. |  [optional] |
| **password** | **kotlin.String** | Present only for secretful kinds; returned ONCE. |  [optional] |


<a id="Kind"></a>
## Enum: kind
| Name | Value |
| ---- | ----- |
| kind | sql, vector, datastore, kv, search, s3, docdb |



