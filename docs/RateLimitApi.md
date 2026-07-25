# RateLimitApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**guardGetRateLimitStatus**](RateLimitApi.md#guardGetRateLimitStatus) | **GET** /v1/guard/rate-limit/{user_id} | Check rate limit status |
| [**guardResetRateLimit**](RateLimitApi.md#guardResetRateLimit) | **DELETE** /v1/guard/rate-limit/{user_id} | Reset rate limit |


<a id="guardGetRateLimitStatus"></a>
# **guardGetRateLimitStatus**
> GuardRateLimitStatus guardGetRateLimitStatus(userId)

Check rate limit status

Check remaining rate limit tokens for a user.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RateLimitApi()
val userId : kotlin.String = userId_example // kotlin.String | 
try {
    val result : GuardRateLimitStatus = apiInstance.guardGetRateLimitStatus(userId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RateLimitApi#guardGetRateLimitStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RateLimitApi#guardGetRateLimitStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userId** | **kotlin.String**|  | |

### Return type

[**GuardRateLimitStatus**](GuardRateLimitStatus.md)

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

<a id="guardResetRateLimit"></a>
# **guardResetRateLimit**
> guardResetRateLimit(userId)

Reset rate limit

Reset rate limit counters for a user.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RateLimitApi()
val userId : kotlin.String = userId_example // kotlin.String | 
try {
    apiInstance.guardResetRateLimit(userId)
} catch (e: ClientException) {
    println("4xx response calling RateLimitApi#guardResetRateLimit")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RateLimitApi#guardResetRateLimit")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userId** | **kotlin.String**|  | |

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

