# MariadbApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformMariadbCreate**](MariadbApi.md#platformMariadbCreate) | **POST** /v1/platform/mariadb/create | Create a MariaDB service |
| [**platformMariadbOne**](MariadbApi.md#platformMariadbOne) | **GET** /v1/platform/mariadb/one | Get MariaDB details |


<a id="platformMariadbCreate"></a>
# **platformMariadbCreate**
> PlatformTRPCResult platformMariadbCreate(platformMariadbCreateRequest)

Create a MariaDB service

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MariadbApi()
val platformMariadbCreateRequest : PlatformMariadbCreateRequest =  // PlatformMariadbCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformMariadbCreate(platformMariadbCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MariadbApi#platformMariadbCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MariadbApi#platformMariadbCreate")
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

<a id="platformMariadbOne"></a>
# **platformMariadbOne**
> PlatformTRPCResult platformMariadbOne(input)

Get MariaDB details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MariadbApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformMariadbOne(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MariadbApi#platformMariadbOne")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MariadbApi#platformMariadbOne")
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

