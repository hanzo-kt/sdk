# GPUsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**engineGetGPUAllocations**](GPUsApi.md#engineGetGPUAllocations) | **GET** /v1/engine/gpus/allocations | Get GPU allocations |
| [**engineListGPUTypes**](GPUsApi.md#engineListGPUTypes) | **GET** /v1/engine/gpus | List available GPU types |
| [**visorListGPUs**](GPUsApi.md#visorListGPUs) | **GET** /v1/gpus | List per-accelerator GPU inventory (derived from GPU machines) |
| [**visorListGpuAlerts**](GPUsApi.md#visorListGpuAlerts) | **GET** /v1/gpus/alerts | List GPU alerts (honest empty — Visor carries no alert inventory) |


<a id="engineGetGPUAllocations"></a>
# **engineGetGPUAllocations**
> EngineGetGPUAllocations200Response engineGetGPUAllocations(gpuType, clusterId)

Get GPU allocations

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GPUsApi()
val gpuType : kotlin.String = gpuType_example // kotlin.String | 
val clusterId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : EngineGetGPUAllocations200Response = apiInstance.engineGetGPUAllocations(gpuType, clusterId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GPUsApi#engineGetGPUAllocations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GPUsApi#engineGetGPUAllocations")
    e.printStackTrace()
}
```

### Parameters
| **gpuType** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **clusterId** | **java.util.UUID**|  | [optional] |

### Return type

[**EngineGetGPUAllocations200Response**](EngineGetGPUAllocations200Response.md)

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

<a id="engineListGPUTypes"></a>
# **engineListGPUTypes**
> EngineListGPUTypes200Response engineListGPUTypes()

List available GPU types

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GPUsApi()
try {
    val result : EngineListGPUTypes200Response = apiInstance.engineListGPUTypes()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GPUsApi#engineListGPUTypes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GPUsApi#engineListGPUTypes")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**EngineListGPUTypes200Response**](EngineListGPUTypes200Response.md)

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

<a id="visorListGPUs"></a>
# **visorListGPUs**
> VisorListGPUs200Response visorListGPUs()

List per-accelerator GPU inventory (derived from GPU machines)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GPUsApi()
try {
    val result : VisorListGPUs200Response = apiInstance.visorListGPUs()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GPUsApi#visorListGPUs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GPUsApi#visorListGPUs")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**VisorListGPUs200Response**](VisorListGPUs200Response.md)

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

<a id="visorListGpuAlerts"></a>
# **visorListGpuAlerts**
> VisorListGpuAlerts200Response visorListGpuAlerts()

List GPU alerts (honest empty — Visor carries no alert inventory)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GPUsApi()
try {
    val result : VisorListGpuAlerts200Response = apiInstance.visorListGpuAlerts()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GPUsApi#visorListGpuAlerts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GPUsApi#visorListGpuAlerts")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**VisorListGpuAlerts200Response**](VisorListGpuAlerts200Response.md)

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

