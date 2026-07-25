# LoadBalancersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**doCreateLoadBalancer**](LoadBalancersApi.md#doCreateLoadBalancer) | **POST** /v1/load-balancers | Create a load balancer |
| [**doDeleteLoadBalancer**](LoadBalancersApi.md#doDeleteLoadBalancer) | **DELETE** /v1/load-balancers/{id} | Delete one load balancer (owned) |
| [**doGetLoadBalancer**](LoadBalancersApi.md#doGetLoadBalancer) | **GET** /v1/load-balancers/{id} | Get one load balancer (owned) |
| [**doListLoadBalancers**](LoadBalancersApi.md#doListLoadBalancers) | **GET** /v1/load-balancers | List the caller&#39;s load balancers |


<a id="doCreateLoadBalancer"></a>
# **doCreateLoadBalancer**
> DoLoadBalancer doCreateLoadBalancer(doLoadBalancerCreate)

Create a load balancer

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = LoadBalancersApi()
val doLoadBalancerCreate : DoLoadBalancerCreate =  // DoLoadBalancerCreate | 
try {
    val result : DoLoadBalancer = apiInstance.doCreateLoadBalancer(doLoadBalancerCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LoadBalancersApi#doCreateLoadBalancer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LoadBalancersApi#doCreateLoadBalancer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **doLoadBalancerCreate** | [**DoLoadBalancerCreate**](DoLoadBalancerCreate.md)|  | |

### Return type

[**DoLoadBalancer**](DoLoadBalancer.md)

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

<a id="doDeleteLoadBalancer"></a>
# **doDeleteLoadBalancer**
> doDeleteLoadBalancer(id)

Delete one load balancer (owned)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = LoadBalancersApi()
val id : kotlin.String = id_example // kotlin.String | DO load balancer id
try {
    apiInstance.doDeleteLoadBalancer(id)
} catch (e: ClientException) {
    println("4xx response calling LoadBalancersApi#doDeleteLoadBalancer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LoadBalancersApi#doDeleteLoadBalancer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| DO load balancer id | |

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
 - **Accept**: application/json

<a id="doGetLoadBalancer"></a>
# **doGetLoadBalancer**
> DoLoadBalancer doGetLoadBalancer(id)

Get one load balancer (owned)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = LoadBalancersApi()
val id : kotlin.String = id_example // kotlin.String | DO load balancer id
try {
    val result : DoLoadBalancer = apiInstance.doGetLoadBalancer(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LoadBalancersApi#doGetLoadBalancer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LoadBalancersApi#doGetLoadBalancer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| DO load balancer id | |

### Return type

[**DoLoadBalancer**](DoLoadBalancer.md)

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

<a id="doListLoadBalancers"></a>
# **doListLoadBalancers**
> DoListLoadBalancers200Response doListLoadBalancers()

List the caller&#39;s load balancers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = LoadBalancersApi()
try {
    val result : DoListLoadBalancers200Response = apiInstance.doListLoadBalancers()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LoadBalancersApi#doListLoadBalancers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LoadBalancersApi#doListLoadBalancers")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**DoListLoadBalancers200Response**](DoListLoadBalancers200Response.md)

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

