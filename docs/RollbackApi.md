# RollbackApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformRollbackRollback**](RollbackApi.md#platformRollbackRollback) | **POST** /v1/platform/rollback/rollback | Rollback to a previous deployment |


<a id="platformRollbackRollback"></a>
# **platformRollbackRollback**
> PlatformTRPCResult platformRollbackRollback(platformDeploymentKillProcessRequest)

Rollback to a previous deployment

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RollbackApi()
val platformDeploymentKillProcessRequest : PlatformDeploymentKillProcessRequest =  // PlatformDeploymentKillProcessRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformRollbackRollback(platformDeploymentKillProcessRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RollbackApi#platformRollbackRollback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RollbackApi#platformRollbackRollback")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformDeploymentKillProcessRequest** | [**PlatformDeploymentKillProcessRequest**](PlatformDeploymentKillProcessRequest.md)|  | |

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

