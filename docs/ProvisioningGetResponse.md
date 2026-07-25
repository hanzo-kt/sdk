
# ProvisioningGetResponse

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  |
| **name** | **kotlin.String** |  |  |
| **kind** | [**inline**](#Kind) |  |  |
| **status** | **kotlin.String** |  |  |
| **host** | **kotlin.String** |  |  |
| **port** | **kotlin.Int** |  |  |
| **database** | **kotlin.String** |  |  |
| **username** | **kotlin.String** | Present only for secretful kinds. |  [optional] |


<a id="Kind"></a>
## Enum: kind
| Name | Value |
| ---- | ----- |
| kind | sql, vector, datastore, kv, search, s3, docdb |



