
# RegistryArtifact

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.Int** |  |  [optional] |
| **digest** | **kotlin.String** | SHA256 content digest |  [optional] |
| **propertySize** | **kotlin.Long** |  |  [optional] |
| **mediaType** | **kotlin.String** |  |  [optional] |
| **manifestMediaType** | **kotlin.String** |  |  [optional] |
| **type** | [**inline**](#Type) |  |  [optional] |
| **tags** | [**kotlin.collections.List&lt;RegistryTag&gt;**](RegistryTag.md) |  |  [optional] |
| **pushTime** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **pullTime** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **scanOverview** | [**kotlin.collections.Map&lt;kotlin.String, RegistryScanOverview&gt;**](RegistryScanOverview.md) |  |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | IMAGE, CHART, WASM, UNKNOWN |



