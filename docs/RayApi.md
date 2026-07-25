# RayApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**engineCreateRayCluster**](RayApi.md#engineCreateRayCluster) | **POST** /v1/engine/ray/clusters | Create Ray cluster |
| [**engineDeleteRayCluster**](RayApi.md#engineDeleteRayCluster) | **DELETE** /v1/engine/ray/clusters/{name} | Delete Ray cluster |
| [**engineGetRayCluster**](RayApi.md#engineGetRayCluster) | **GET** /v1/engine/ray/clusters/{name} | Get Ray cluster |
| [**engineGetRayClusterStatus**](RayApi.md#engineGetRayClusterStatus) | **GET** /v1/engine/ray/clusters/{name}/status | Get Ray cluster status |
| [**engineGetRayDashboard**](RayApi.md#engineGetRayDashboard) | **GET** /v1/engine/ray/clusters/{name}/dashboard | Get Ray dashboard URL |
| [**engineListRayClusters**](RayApi.md#engineListRayClusters) | **GET** /v1/engine/ray/clusters | List Ray clusters |
| [**engineScaleRayCluster**](RayApi.md#engineScaleRayCluster) | **PUT** /v1/engine/ray/clusters/{name}/scale | Scale Ray workers |


<a id="engineCreateRayCluster"></a>
# **engineCreateRayCluster**
> EngineRayCluster engineCreateRayCluster(engineRayClusterCreate)

Create Ray cluster

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RayApi()
val engineRayClusterCreate : EngineRayClusterCreate =  // EngineRayClusterCreate | 
try {
    val result : EngineRayCluster = apiInstance.engineCreateRayCluster(engineRayClusterCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RayApi#engineCreateRayCluster")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RayApi#engineCreateRayCluster")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **engineRayClusterCreate** | [**EngineRayClusterCreate**](EngineRayClusterCreate.md)|  | |

### Return type

[**EngineRayCluster**](EngineRayCluster.md)

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

<a id="engineDeleteRayCluster"></a>
# **engineDeleteRayCluster**
> kotlin.Any engineDeleteRayCluster(name)

Delete Ray cluster

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RayApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.engineDeleteRayCluster(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RayApi#engineDeleteRayCluster")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RayApi#engineDeleteRayCluster")
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

<a id="engineGetRayCluster"></a>
# **engineGetRayCluster**
> EngineRayCluster engineGetRayCluster(name)

Get Ray cluster

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RayApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : EngineRayCluster = apiInstance.engineGetRayCluster(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RayApi#engineGetRayCluster")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RayApi#engineGetRayCluster")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**EngineRayCluster**](EngineRayCluster.md)

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

<a id="engineGetRayClusterStatus"></a>
# **engineGetRayClusterStatus**
> EngineRayCluster engineGetRayClusterStatus(name)

Get Ray cluster status

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RayApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : EngineRayCluster = apiInstance.engineGetRayClusterStatus(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RayApi#engineGetRayClusterStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RayApi#engineGetRayClusterStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**EngineRayCluster**](EngineRayCluster.md)

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

<a id="engineGetRayDashboard"></a>
# **engineGetRayDashboard**
> EngineGetRayDashboard200Response engineGetRayDashboard(name)

Get Ray dashboard URL

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RayApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : EngineGetRayDashboard200Response = apiInstance.engineGetRayDashboard(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RayApi#engineGetRayDashboard")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RayApi#engineGetRayDashboard")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**EngineGetRayDashboard200Response**](EngineGetRayDashboard200Response.md)

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

<a id="engineListRayClusters"></a>
# **engineListRayClusters**
> EngineListRayClusters200Response engineListRayClusters(namespace, status)

List Ray clusters

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RayApi()
val namespace : kotlin.String = namespace_example // kotlin.String | 
val status : kotlin.String = status_example // kotlin.String | 
try {
    val result : EngineListRayClusters200Response = apiInstance.engineListRayClusters(namespace, status)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RayApi#engineListRayClusters")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RayApi#engineListRayClusters")
    e.printStackTrace()
}
```

### Parameters
| **namespace** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | **kotlin.String**|  | [optional] [enum: creating, running, suspended, failed, deleting] |

### Return type

[**EngineListRayClusters200Response**](EngineListRayClusters200Response.md)

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

<a id="engineScaleRayCluster"></a>
# **engineScaleRayCluster**
> EngineRayCluster engineScaleRayCluster(name, engineRayClusterScale)

Scale Ray workers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RayApi()
val name : kotlin.String = name_example // kotlin.String | 
val engineRayClusterScale : EngineRayClusterScale =  // EngineRayClusterScale | 
try {
    val result : EngineRayCluster = apiInstance.engineScaleRayCluster(name, engineRayClusterScale)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RayApi#engineScaleRayCluster")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RayApi#engineScaleRayCluster")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **engineRayClusterScale** | [**EngineRayClusterScale**](EngineRayClusterScale.md)|  | |

### Return type

[**EngineRayCluster**](EngineRayCluster.md)

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

