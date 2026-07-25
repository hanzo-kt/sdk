# RoutesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gatewayCreateRoute**](RoutesApi.md#gatewayCreateRoute) | **POST** /v1/gateway/routes | Create routing rule |
| [**gatewayDeleteRoute**](RoutesApi.md#gatewayDeleteRoute) | **DELETE** /v1/gateway/routes/{id} | Delete routing rule |
| [**gatewayGetRoute**](RoutesApi.md#gatewayGetRoute) | **GET** /v1/gateway/routes/{id} | Get routing rule |
| [**gatewayListRoutes**](RoutesApi.md#gatewayListRoutes) | **GET** /v1/gateway/routes | List custom routing rules |
| [**gatewayUpdateRoute**](RoutesApi.md#gatewayUpdateRoute) | **PUT** /v1/gateway/routes/{id} | Update routing rule |


<a id="gatewayCreateRoute"></a>
# **gatewayCreateRoute**
> GatewayRoutingRule gatewayCreateRoute(gatewayRoutingRule)

Create routing rule

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RoutesApi()
val gatewayRoutingRule : GatewayRoutingRule =  // GatewayRoutingRule | 
try {
    val result : GatewayRoutingRule = apiInstance.gatewayCreateRoute(gatewayRoutingRule)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RoutesApi#gatewayCreateRoute")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RoutesApi#gatewayCreateRoute")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayRoutingRule** | [**GatewayRoutingRule**](GatewayRoutingRule.md)|  | |

### Return type

[**GatewayRoutingRule**](GatewayRoutingRule.md)

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

<a id="gatewayDeleteRoute"></a>
# **gatewayDeleteRoute**
> gatewayDeleteRoute(id)

Delete routing rule

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RoutesApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.gatewayDeleteRoute(id)
} catch (e: ClientException) {
    println("4xx response calling RoutesApi#gatewayDeleteRoute")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RoutesApi#gatewayDeleteRoute")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

null (empty response body)

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
 - **Accept**: Not defined

<a id="gatewayGetRoute"></a>
# **gatewayGetRoute**
> GatewayRoutingRule gatewayGetRoute(id)

Get routing rule

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RoutesApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : GatewayRoutingRule = apiInstance.gatewayGetRoute(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RoutesApi#gatewayGetRoute")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RoutesApi#gatewayGetRoute")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**GatewayRoutingRule**](GatewayRoutingRule.md)

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

<a id="gatewayListRoutes"></a>
# **gatewayListRoutes**
> kotlin.collections.List&lt;GatewayRoutingRule&gt; gatewayListRoutes()

List custom routing rules

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RoutesApi()
try {
    val result : kotlin.collections.List<GatewayRoutingRule> = apiInstance.gatewayListRoutes()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RoutesApi#gatewayListRoutes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RoutesApi#gatewayListRoutes")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;GatewayRoutingRule&gt;**](GatewayRoutingRule.md)

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

<a id="gatewayUpdateRoute"></a>
# **gatewayUpdateRoute**
> GatewayRoutingRule gatewayUpdateRoute(id, gatewayRoutingRule)

Update routing rule

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RoutesApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val gatewayRoutingRule : GatewayRoutingRule =  // GatewayRoutingRule | 
try {
    val result : GatewayRoutingRule = apiInstance.gatewayUpdateRoute(id, gatewayRoutingRule)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RoutesApi#gatewayUpdateRoute")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RoutesApi#gatewayUpdateRoute")
    e.printStackTrace()
}
```

### Parameters
| **id** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayRoutingRule** | [**GatewayRoutingRule**](GatewayRoutingRule.md)|  | |

### Return type

[**GatewayRoutingRule**](GatewayRoutingRule.md)

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

