# BackupApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformBackupCreate**](BackupApi.md#platformBackupCreate) | **POST** /v1/platform/backup/create | Create a backup schedule |


<a id="platformBackupCreate"></a>
# **platformBackupCreate**
> PlatformTRPCResult platformBackupCreate(platformBackupCreateRequest)

Create a backup schedule

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BackupApi()
val platformBackupCreateRequest : PlatformBackupCreateRequest =  // PlatformBackupCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformBackupCreate(platformBackupCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BackupApi#platformBackupCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BackupApi#platformBackupCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformBackupCreateRequest** | [**PlatformBackupCreateRequest**](PlatformBackupCreateRequest.md)|  | |

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

