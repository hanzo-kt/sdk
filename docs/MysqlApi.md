# MysqlApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformMysqlCreate**](MysqlApi.md#platformMysqlCreate) | **POST** /v1/platform/mysql/create | Create a MySQL service |
| [**platformMysqlOne**](MysqlApi.md#platformMysqlOne) | **GET** /v1/platform/mysql/one | Get MySQL details |


<a id="platformMysqlCreate"></a>
# **platformMysqlCreate**
> PlatformTRPCResult platformMysqlCreate(platformMariadbCreateRequest)

Create a MySQL service

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MysqlApi()
val platformMariadbCreateRequest : PlatformMariadbCreateRequest =  // PlatformMariadbCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformMysqlCreate(platformMariadbCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MysqlApi#platformMysqlCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MysqlApi#platformMysqlCreate")
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

<a id="platformMysqlOne"></a>
# **platformMysqlOne**
> PlatformTRPCResult platformMysqlOne(input)

Get MySQL details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MysqlApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformMysqlOne(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MysqlApi#platformMysqlOne")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MysqlApi#platformMysqlOne")
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

