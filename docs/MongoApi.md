# MongoApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformMongoCreate**](MongoApi.md#platformMongoCreate) | **POST** /v1/platform/mongo/create | Create a MongoDB service |
| [**platformMongoOne**](MongoApi.md#platformMongoOne) | **GET** /v1/platform/mongo/one | Get MongoDB details |


<a id="platformMongoCreate"></a>
# **platformMongoCreate**
> PlatformTRPCResult platformMongoCreate(platformMariadbCreateRequest)

Create a MongoDB service

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MongoApi()
val platformMariadbCreateRequest : PlatformMariadbCreateRequest =  // PlatformMariadbCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformMongoCreate(platformMariadbCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MongoApi#platformMongoCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MongoApi#platformMongoCreate")
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

<a id="platformMongoOne"></a>
# **platformMongoOne**
> PlatformTRPCResult platformMongoOne(input)

Get MongoDB details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MongoApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformMongoOne(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MongoApi#platformMongoOne")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MongoApi#platformMongoOne")
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

