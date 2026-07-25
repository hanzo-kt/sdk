# IngestionApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**consoleIngestOtelMetrics**](IngestionApi.md#consoleIngestOtelMetrics) | **POST** /v1/console/otel/v1/metrics | Ingest OpenTelemetry metrics |
| [**consoleIngestOtelTraces**](IngestionApi.md#consoleIngestOtelTraces) | **POST** /v1/console/otel/v1/traces | Ingest OpenTelemetry traces |


<a id="consoleIngestOtelMetrics"></a>
# **consoleIngestOtelMetrics**
> kotlin.Any consoleIngestOtelMetrics(body)

Ingest OpenTelemetry metrics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IngestionApi()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.consoleIngestOtelMetrics(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IngestionApi#consoleIngestOtelMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IngestionApi#consoleIngestOtelMetrics")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="consoleIngestOtelTraces"></a>
# **consoleIngestOtelTraces**
> kotlin.Any consoleIngestOtelTraces(body)

Ingest OpenTelemetry traces

OTLP/HTTP endpoint for trace ingestion (JSON or protobuf)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IngestionApi()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.consoleIngestOtelTraces(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IngestionApi#consoleIngestOtelTraces")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IngestionApi#consoleIngestOtelTraces")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure bearerAuth statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearerAuth dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

