
# ConsoleScore

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | **kotlin.String** |  |  [optional] |
| **traceId** | **kotlin.String** |  |  [optional] |
| **observationId** | **kotlin.String** |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **&#x60;value&#x60;** | [**kotlin.Any**](.md) |  |  [optional] |
| **stringValue** | **kotlin.String** |  |  [optional] |
| **dataType** | [**inline**](#DataType) |  |  [optional] |
| **comment** | **kotlin.String** |  |  [optional] |
| **source** | [**inline**](#Source) |  |  [optional] |
| **environment** | **kotlin.String** |  |  [optional] |
| **configId** | **kotlin.String** |  |  [optional] |
| **queueId** | **kotlin.String** |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="DataType"></a>
## Enum: dataType
| Name | Value |
| ---- | ----- |
| dataType | NUMERIC, CATEGORICAL, BOOLEAN |


<a id="Source"></a>
## Enum: source
| Name | Value |
| ---- | ----- |
| source | API, EVAL, ANNOTATION |



