# ScheduleApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformScheduleCreate**](ScheduleApi.md#platformScheduleCreate) | **POST** /v1/platform/schedule/create | Create a scheduled task |
| [**platformScheduleList**](ScheduleApi.md#platformScheduleList) | **GET** /v1/platform/schedule/list | List scheduled tasks |


<a id="platformScheduleCreate"></a>
# **platformScheduleCreate**
> PlatformTRPCResult platformScheduleCreate(platformScheduleCreateRequest)

Create a scheduled task

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScheduleApi()
val platformScheduleCreateRequest : PlatformScheduleCreateRequest =  // PlatformScheduleCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformScheduleCreate(platformScheduleCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScheduleApi#platformScheduleCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScheduleApi#platformScheduleCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformScheduleCreateRequest** | [**PlatformScheduleCreateRequest**](PlatformScheduleCreateRequest.md)|  | |

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

<a id="platformScheduleList"></a>
# **platformScheduleList**
> PlatformTRPCResult platformScheduleList(input)

List scheduled tasks

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ScheduleApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformScheduleList(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ScheduleApi#platformScheduleList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ScheduleApi#platformScheduleList")
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

