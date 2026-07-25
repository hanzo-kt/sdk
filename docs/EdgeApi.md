# EdgeApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gatewayInvokeEdgeFunction**](EdgeApi.md#gatewayInvokeEdgeFunction) | **POST** /v1/gateway/edge/{slug} | Invoke edge function via gateway |
| [**gatewayInvokeEdgeFunctionGet**](EdgeApi.md#gatewayInvokeEdgeFunctionGet) | **GET** /v1/gateway/edge/{slug} | Invoke edge function (GET) |
| [**ztListEdgeNodes**](EdgeApi.md#ztListEdgeNodes) | **GET** /v1/edge/nodes | List the org&#39;s ZT edge-routers |


<a id="gatewayInvokeEdgeFunction"></a>
# **gatewayInvokeEdgeFunction**
> kotlin.Any gatewayInvokeEdgeFunction(slug, body)

Invoke edge function via gateway

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EdgeApi()
val slug : kotlin.String = slug_example // kotlin.String | Function slug
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.gatewayInvokeEdgeFunction(slug, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EdgeApi#gatewayInvokeEdgeFunction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EdgeApi#gatewayInvokeEdgeFunction")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**| Function slug | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | [optional] |

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

<a id="gatewayInvokeEdgeFunctionGet"></a>
# **gatewayInvokeEdgeFunctionGet**
> kotlin.Any gatewayInvokeEdgeFunctionGet(slug)

Invoke edge function (GET)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EdgeApi()
val slug : kotlin.String = slug_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.gatewayInvokeEdgeFunctionGet(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EdgeApi#gatewayInvokeEdgeFunctionGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EdgeApi#gatewayInvokeEdgeFunctionGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**|  | |

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

<a id="ztListEdgeNodes"></a>
# **ztListEdgeNodes**
> ZtListEdgeNodes200Response ztListEdgeNodes()

List the org&#39;s ZT edge-routers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EdgeApi()
try {
    val result : ZtListEdgeNodes200Response = apiInstance.ztListEdgeNodes()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EdgeApi#ztListEdgeNodes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EdgeApi#ztListEdgeNodes")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ZtListEdgeNodes200Response**](ZtListEdgeNodes200Response.md)

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

