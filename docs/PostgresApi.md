# PostgresApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformPostgresCreate**](PostgresApi.md#platformPostgresCreate) | **POST** /v1/platform/postgres/create | Create a PostgreSQL service |
| [**platformPostgresOne**](PostgresApi.md#platformPostgresOne) | **GET** /v1/platform/postgres/one | Get PostgreSQL details |


<a id="platformPostgresCreate"></a>
# **platformPostgresCreate**
> PlatformTRPCResult platformPostgresCreate(platformMariadbCreateRequest)

Create a PostgreSQL service

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PostgresApi()
val platformMariadbCreateRequest : PlatformMariadbCreateRequest =  // PlatformMariadbCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformPostgresCreate(platformMariadbCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PostgresApi#platformPostgresCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PostgresApi#platformPostgresCreate")
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

<a id="platformPostgresOne"></a>
# **platformPostgresOne**
> PlatformTRPCResult platformPostgresOne(input)

Get PostgreSQL details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PostgresApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformPostgresOne(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PostgresApi#platformPostgresOne")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PostgresApi#platformPostgresOne")
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

