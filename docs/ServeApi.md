# ServeApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**engineCreateServingEndpoint**](ServeApi.md#engineCreateServingEndpoint) | **POST** /v1/engine/serve/endpoints | Create serving endpoint |
| [**engineDeleteServingEndpoint**](ServeApi.md#engineDeleteServingEndpoint) | **DELETE** /v1/engine/serve/endpoints/{name} | Delete serving endpoint |
| [**engineGetServingEndpoint**](ServeApi.md#engineGetServingEndpoint) | **GET** /v1/engine/serve/endpoints/{name} | Get serving endpoint |
| [**engineGetServingMetrics**](ServeApi.md#engineGetServingMetrics) | **GET** /v1/engine/serve/endpoints/{name}/metrics | Get serving endpoint metrics |
| [**engineListServingEndpoints**](ServeApi.md#engineListServingEndpoints) | **GET** /v1/engine/serve/endpoints | List serving endpoints |
| [**engineUpdateServingEndpoint**](ServeApi.md#engineUpdateServingEndpoint) | **PUT** /v1/engine/serve/endpoints/{name} | Update serving endpoint |


<a id="engineCreateServingEndpoint"></a>
# **engineCreateServingEndpoint**
> EngineServingEndpoint engineCreateServingEndpoint(engineServingEndpointCreate)

Create serving endpoint

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServeApi()
val engineServingEndpointCreate : EngineServingEndpointCreate =  // EngineServingEndpointCreate | 
try {
    val result : EngineServingEndpoint = apiInstance.engineCreateServingEndpoint(engineServingEndpointCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServeApi#engineCreateServingEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServeApi#engineCreateServingEndpoint")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **engineServingEndpointCreate** | [**EngineServingEndpointCreate**](EngineServingEndpointCreate.md)|  | |

### Return type

[**EngineServingEndpoint**](EngineServingEndpoint.md)

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

<a id="engineDeleteServingEndpoint"></a>
# **engineDeleteServingEndpoint**
> kotlin.Any engineDeleteServingEndpoint(name)

Delete serving endpoint

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServeApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.engineDeleteServingEndpoint(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServeApi#engineDeleteServingEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServeApi#engineDeleteServingEndpoint")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

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

<a id="engineGetServingEndpoint"></a>
# **engineGetServingEndpoint**
> EngineServingEndpoint engineGetServingEndpoint(name)

Get serving endpoint

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServeApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : EngineServingEndpoint = apiInstance.engineGetServingEndpoint(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServeApi#engineGetServingEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServeApi#engineGetServingEndpoint")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**EngineServingEndpoint**](EngineServingEndpoint.md)

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

<a id="engineGetServingMetrics"></a>
# **engineGetServingMetrics**
> kotlin.collections.List&lt;EngineServingMetrics&gt; engineGetServingMetrics(name, from, to, granularity)

Get serving endpoint metrics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServeApi()
val name : kotlin.String = name_example // kotlin.String | 
val from : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val to : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val granularity : kotlin.String = granularity_example // kotlin.String | 
try {
    val result : kotlin.collections.List<EngineServingMetrics> = apiInstance.engineGetServingMetrics(name, from, to, granularity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServeApi#engineGetServingMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServeApi#engineGetServingMetrics")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| **from** | **java.time.OffsetDateTime**|  | [optional] |
| **to** | **java.time.OffsetDateTime**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **granularity** | **kotlin.String**|  | [optional] [default to Granularity.hour] [enum: minute, hour, day] |

### Return type

[**kotlin.collections.List&lt;EngineServingMetrics&gt;**](EngineServingMetrics.md)

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

<a id="engineListServingEndpoints"></a>
# **engineListServingEndpoints**
> EngineListServingEndpoints200Response engineListServingEndpoints(status, page, pageSize)

List serving endpoints

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServeApi()
val status : kotlin.String = status_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : EngineListServingEndpoints200Response = apiInstance.engineListServingEndpoints(status, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServeApi#engineListServingEndpoints")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServeApi#engineListServingEndpoints")
    e.printStackTrace()
}
```

### Parameters
| **status** | **kotlin.String**|  | [optional] [enum: provisioning, running, scaling, failed, stopped] |
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 20] |

### Return type

[**EngineListServingEndpoints200Response**](EngineListServingEndpoints200Response.md)

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

<a id="engineUpdateServingEndpoint"></a>
# **engineUpdateServingEndpoint**
> EngineServingEndpoint engineUpdateServingEndpoint(name, engineUpdateServingEndpointRequest)

Update serving endpoint

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ServeApi()
val name : kotlin.String = name_example // kotlin.String | 
val engineUpdateServingEndpointRequest : EngineUpdateServingEndpointRequest =  // EngineUpdateServingEndpointRequest | 
try {
    val result : EngineServingEndpoint = apiInstance.engineUpdateServingEndpoint(name, engineUpdateServingEndpointRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServeApi#engineUpdateServingEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServeApi#engineUpdateServingEndpoint")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **engineUpdateServingEndpointRequest** | [**EngineUpdateServingEndpointRequest**](EngineUpdateServingEndpointRequest.md)|  | |

### Return type

[**EngineServingEndpoint**](EngineServingEndpoint.md)

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

