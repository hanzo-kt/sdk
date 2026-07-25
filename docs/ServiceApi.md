# ServiceApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**vectorGetTelemetry**](ServiceApi.md#vectorGetTelemetry) | **GET** /v1/vector/telemetry | Get telemetry |
| [**vectorHealthCheck**](ServiceApi.md#vectorHealthCheck) | **GET** /healthz | Health check |
| [**vectorReadinessCheck**](ServiceApi.md#vectorReadinessCheck) | **GET** /v1/vector/readyz | Readiness check |


<a id="vectorGetTelemetry"></a>
# **vectorGetTelemetry**
> kotlin.Any vectorGetTelemetry()

Get telemetry

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServiceApi()
try {
    val result : kotlin.Any = apiInstance.vectorGetTelemetry()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServiceApi#vectorGetTelemetry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServiceApi#vectorGetTelemetry")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="vectorHealthCheck"></a>
# **vectorHealthCheck**
> kotlin.String vectorHealthCheck()

Health check

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServiceApi()
try {
    val result : kotlin.String = apiInstance.vectorHealthCheck()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServiceApi#vectorHealthCheck")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServiceApi#vectorHealthCheck")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**kotlin.String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain

<a id="vectorReadinessCheck"></a>
# **vectorReadinessCheck**
> kotlin.String vectorReadinessCheck()

Readiness check

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServiceApi()
try {
    val result : kotlin.String = apiInstance.vectorReadinessCheck()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServiceApi#vectorReadinessCheck")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServiceApi#vectorReadinessCheck")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**kotlin.String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain

