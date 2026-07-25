# ConfigApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatGetConfig**](ConfigApi.md#chatGetConfig) | **GET** /v1/chat/config | Get startup configuration |
| [**guardGetConfig**](ConfigApi.md#guardGetConfig) | **GET** /v1/guard/config | Get current configuration |
| [**guardUpdateConfig**](ConfigApi.md#guardUpdateConfig) | **PUT** /v1/guard/config | Update configuration |


<a id="chatGetConfig"></a>
# **chatGetConfig**
> ChatStartupConfig chatGetConfig()

Get startup configuration

Returns app title, enabled features, social logins, etc.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConfigApi()
try {
    val result : ChatStartupConfig = apiInstance.chatGetConfig()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConfigApi#chatGetConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConfigApi#chatGetConfig")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ChatStartupConfig**](ChatStartupConfig.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="guardGetConfig"></a>
# **guardGetConfig**
> GuardSanitizeConfig guardGetConfig()

Get current configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConfigApi()
try {
    val result : GuardSanitizeConfig = apiInstance.guardGetConfig()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConfigApi#guardGetConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConfigApi#guardGetConfig")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**GuardSanitizeConfig**](GuardSanitizeConfig.md)

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

<a id="guardUpdateConfig"></a>
# **guardUpdateConfig**
> guardUpdateConfig(guardSanitizeConfig)

Update configuration

Update guard configuration at runtime.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConfigApi()
val guardSanitizeConfig : GuardSanitizeConfig =  // GuardSanitizeConfig | 
try {
    apiInstance.guardUpdateConfig(guardSanitizeConfig)
} catch (e: ClientException) {
    println("4xx response calling ConfigApi#guardUpdateConfig")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConfigApi#guardUpdateConfig")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **guardSanitizeConfig** | [**GuardSanitizeConfig**](GuardSanitizeConfig.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: Not defined

