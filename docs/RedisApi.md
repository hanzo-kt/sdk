# RedisApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformRedisCreate**](RedisApi.md#platformRedisCreate) | **POST** /v1/platform/redis/create | Create a Redis service |
| [**platformRedisOne**](RedisApi.md#platformRedisOne) | **GET** /v1/platform/redis/one | Get Redis details |


<a id="platformRedisCreate"></a>
# **platformRedisCreate**
> PlatformTRPCResult platformRedisCreate(platformMariadbCreateRequest)

Create a Redis service

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RedisApi()
val platformMariadbCreateRequest : PlatformMariadbCreateRequest =  // PlatformMariadbCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformRedisCreate(platformMariadbCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RedisApi#platformRedisCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RedisApi#platformRedisCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformMariadbCreateRequest** | [**PlatformMariadbCreateRequest**](PlatformMariadbCreateRequest.md)|  | |

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

<a id="platformRedisOne"></a>
# **platformRedisOne**
> PlatformTRPCResult platformRedisOne(input)

Get Redis details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RedisApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformRedisOne(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RedisApi#platformRedisOne")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RedisApi#platformRedisOne")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **input** | **kotlin.String**| URL-encoded JSON input for tRPC queries | [optional] |

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

