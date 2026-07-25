# PlatformApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoGetPlatform**](PlatformApi.md#autoGetPlatform) | **GET** /v1/auto/platforms/{id} | Get platform settings |
| [**autoUpdatePlatform**](PlatformApi.md#autoUpdatePlatform) | **POST** /v1/auto/platforms/{id} | Update platform settings |
| [**flowGetAnalytics**](PlatformApi.md#flowGetAnalytics) | **GET** /v1/flow/analytics | Get platform analytics data |
| [**flowGetPlatform**](PlatformApi.md#flowGetPlatform) | **GET** /v1/flow/platforms/{id} | Get platform settings |
| [**flowGetQueueMetrics**](PlatformApi.md#flowGetQueueMetrics) | **GET** /v1/flow/queue-metrics | Get worker queue metrics (EE) |
| [**flowUpdatePlatform**](PlatformApi.md#flowUpdatePlatform) | **POST** /v1/flow/platforms/{id} | Update platform settings |


<a id="autoGetPlatform"></a>
# **autoGetPlatform**
> kotlin.Any autoGetPlatform(id)

Get platform settings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlatformApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoGetPlatform(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlatformApi#autoGetPlatform")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlatformApi#autoGetPlatform")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="autoUpdatePlatform"></a>
# **autoUpdatePlatform**
> kotlin.Any autoUpdatePlatform(id, autoUpdatePlatformRequest)

Update platform settings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlatformApi()
val id : kotlin.String = id_example // kotlin.String | 
val autoUpdatePlatformRequest : AutoUpdatePlatformRequest =  // AutoUpdatePlatformRequest | 
try {
    val result : kotlin.Any = apiInstance.autoUpdatePlatform(id, autoUpdatePlatformRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlatformApi#autoUpdatePlatform")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlatformApi#autoUpdatePlatform")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoUpdatePlatformRequest** | [**AutoUpdatePlatformRequest**](AutoUpdatePlatformRequest.md)|  | |

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

<a id="flowGetAnalytics"></a>
# **flowGetAnalytics**
> kotlin.Any flowGetAnalytics()

Get platform analytics data

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlatformApi()
try {
    val result : kotlin.Any = apiInstance.flowGetAnalytics()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlatformApi#flowGetAnalytics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlatformApi#flowGetAnalytics")
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

<a id="flowGetPlatform"></a>
# **flowGetPlatform**
> FlowPlatform flowGetPlatform(id)

Get platform settings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlatformApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : FlowPlatform = apiInstance.flowGetPlatform(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlatformApi#flowGetPlatform")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlatformApi#flowGetPlatform")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**FlowPlatform**](FlowPlatform.md)

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

<a id="flowGetQueueMetrics"></a>
# **flowGetQueueMetrics**
> kotlin.Any flowGetQueueMetrics()

Get worker queue metrics (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlatformApi()
try {
    val result : kotlin.Any = apiInstance.flowGetQueueMetrics()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlatformApi#flowGetQueueMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlatformApi#flowGetQueueMetrics")
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

<a id="flowUpdatePlatform"></a>
# **flowUpdatePlatform**
> kotlin.Any flowUpdatePlatform(id, flowUpdatePlatformRequest)

Update platform settings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlatformApi()
val id : kotlin.String = id_example // kotlin.String | 
val flowUpdatePlatformRequest : FlowUpdatePlatformRequest =  // FlowUpdatePlatformRequest | 
try {
    val result : kotlin.Any = apiInstance.flowUpdatePlatform(id, flowUpdatePlatformRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlatformApi#flowUpdatePlatform")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlatformApi#flowUpdatePlatform")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowUpdatePlatformRequest** | [**FlowUpdatePlatformRequest**](FlowUpdatePlatformRequest.md)|  | |

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

