# EndpointsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatGetEndpoints**](EndpointsApi.md#chatGetEndpoints) | **GET** /v1/chat/endpoints | Get configured endpoints |
| [**dbCreateEndpoint**](EndpointsApi.md#dbCreateEndpoint) | **POST** /v1/db/projects/{id}/endpoints | Create compute endpoint |
| [**dbDeleteEndpoint**](EndpointsApi.md#dbDeleteEndpoint) | **DELETE** /v1/db/projects/{id}/endpoints/{endpoint_id} | Delete compute endpoint |
| [**dbGetEndpoint**](EndpointsApi.md#dbGetEndpoint) | **GET** /v1/db/projects/{id}/endpoints/{endpoint_id} | Get compute endpoint |
| [**dbListEndpoints**](EndpointsApi.md#dbListEndpoints) | **GET** /v1/db/projects/{id}/endpoints | List compute endpoints |
| [**dbStartEndpoint**](EndpointsApi.md#dbStartEndpoint) | **POST** /v1/db/projects/{id}/endpoints/{endpoint_id}/start | Start compute endpoint |
| [**dbSuspendEndpoint**](EndpointsApi.md#dbSuspendEndpoint) | **POST** /v1/db/projects/{id}/endpoints/{endpoint_id}/suspend | Suspend compute endpoint |
| [**dbUpdateEndpoint**](EndpointsApi.md#dbUpdateEndpoint) | **PUT** /v1/db/projects/{id}/endpoints/{endpoint_id} | Update compute endpoint |


<a id="chatGetEndpoints"></a>
# **chatGetEndpoints**
> kotlin.Any chatGetEndpoints()

Get configured endpoints

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EndpointsApi()
try {
    val result : kotlin.Any = apiInstance.chatGetEndpoints()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EndpointsApi#chatGetEndpoints")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EndpointsApi#chatGetEndpoints")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="dbCreateEndpoint"></a>
# **dbCreateEndpoint**
> DbCreateEndpoint201Response dbCreateEndpoint(id, dbCreateEndpointRequest)

Create compute endpoint

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EndpointsApi()
val id : kotlin.String = id_example // kotlin.String | 
val dbCreateEndpointRequest : DbCreateEndpointRequest =  // DbCreateEndpointRequest | 
try {
    val result : DbCreateEndpoint201Response = apiInstance.dbCreateEndpoint(id, dbCreateEndpointRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EndpointsApi#dbCreateEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EndpointsApi#dbCreateEndpoint")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dbCreateEndpointRequest** | [**DbCreateEndpointRequest**](DbCreateEndpointRequest.md)|  | |

### Return type

[**DbCreateEndpoint201Response**](DbCreateEndpoint201Response.md)

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

<a id="dbDeleteEndpoint"></a>
# **dbDeleteEndpoint**
> DbCreateEndpoint201Response dbDeleteEndpoint(id, endpointId)

Delete compute endpoint

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EndpointsApi()
val id : kotlin.String = id_example // kotlin.String | 
val endpointId : kotlin.String = endpointId_example // kotlin.String | 
try {
    val result : DbCreateEndpoint201Response = apiInstance.dbDeleteEndpoint(id, endpointId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EndpointsApi#dbDeleteEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EndpointsApi#dbDeleteEndpoint")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **endpointId** | **kotlin.String**|  | |

### Return type

[**DbCreateEndpoint201Response**](DbCreateEndpoint201Response.md)

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

<a id="dbGetEndpoint"></a>
# **dbGetEndpoint**
> DbCreateEndpoint201Response dbGetEndpoint(id, endpointId)

Get compute endpoint

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EndpointsApi()
val id : kotlin.String = id_example // kotlin.String | 
val endpointId : kotlin.String = endpointId_example // kotlin.String | 
try {
    val result : DbCreateEndpoint201Response = apiInstance.dbGetEndpoint(id, endpointId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EndpointsApi#dbGetEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EndpointsApi#dbGetEndpoint")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **endpointId** | **kotlin.String**|  | |

### Return type

[**DbCreateEndpoint201Response**](DbCreateEndpoint201Response.md)

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

<a id="dbListEndpoints"></a>
# **dbListEndpoints**
> DbListEndpoints200Response dbListEndpoints(id)

List compute endpoints

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EndpointsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : DbListEndpoints200Response = apiInstance.dbListEndpoints(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EndpointsApi#dbListEndpoints")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EndpointsApi#dbListEndpoints")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**DbListEndpoints200Response**](DbListEndpoints200Response.md)

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

<a id="dbStartEndpoint"></a>
# **dbStartEndpoint**
> DbCreateEndpoint201Response dbStartEndpoint(id, endpointId)

Start compute endpoint

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EndpointsApi()
val id : kotlin.String = id_example // kotlin.String | 
val endpointId : kotlin.String = endpointId_example // kotlin.String | 
try {
    val result : DbCreateEndpoint201Response = apiInstance.dbStartEndpoint(id, endpointId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EndpointsApi#dbStartEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EndpointsApi#dbStartEndpoint")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **endpointId** | **kotlin.String**|  | |

### Return type

[**DbCreateEndpoint201Response**](DbCreateEndpoint201Response.md)

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

<a id="dbSuspendEndpoint"></a>
# **dbSuspendEndpoint**
> DbCreateEndpoint201Response dbSuspendEndpoint(id, endpointId)

Suspend compute endpoint

Suspends the endpoint to save compute costs. It will resume on next connection.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EndpointsApi()
val id : kotlin.String = id_example // kotlin.String | 
val endpointId : kotlin.String = endpointId_example // kotlin.String | 
try {
    val result : DbCreateEndpoint201Response = apiInstance.dbSuspendEndpoint(id, endpointId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EndpointsApi#dbSuspendEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EndpointsApi#dbSuspendEndpoint")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **endpointId** | **kotlin.String**|  | |

### Return type

[**DbCreateEndpoint201Response**](DbCreateEndpoint201Response.md)

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

<a id="dbUpdateEndpoint"></a>
# **dbUpdateEndpoint**
> DbCreateEndpoint201Response dbUpdateEndpoint(id, endpointId, dbUpdateEndpointRequest)

Update compute endpoint

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EndpointsApi()
val id : kotlin.String = id_example // kotlin.String | 
val endpointId : kotlin.String = endpointId_example // kotlin.String | 
val dbUpdateEndpointRequest : DbUpdateEndpointRequest =  // DbUpdateEndpointRequest | 
try {
    val result : DbCreateEndpoint201Response = apiInstance.dbUpdateEndpoint(id, endpointId, dbUpdateEndpointRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EndpointsApi#dbUpdateEndpoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EndpointsApi#dbUpdateEndpoint")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| **endpointId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dbUpdateEndpointRequest** | [**DbUpdateEndpointRequest**](DbUpdateEndpointRequest.md)|  | |

### Return type

[**DbCreateEndpoint201Response**](DbCreateEndpoint201Response.md)

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

