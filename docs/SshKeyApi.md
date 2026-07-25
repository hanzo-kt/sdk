# SshKeyApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformSshKeyAll**](SshKeyApi.md#platformSshKeyAll) | **GET** /v1/platform/sshKey/all | List all SSH keys |
| [**platformSshKeyCreate**](SshKeyApi.md#platformSshKeyCreate) | **POST** /v1/platform/sshKey/create | Add an SSH key |
| [**platformSshKeyGenerate**](SshKeyApi.md#platformSshKeyGenerate) | **POST** /v1/platform/sshKey/generate | Generate a new SSH key pair |
| [**platformSshKeyRemove**](SshKeyApi.md#platformSshKeyRemove) | **POST** /v1/platform/sshKey/remove | Remove an SSH key |


<a id="platformSshKeyAll"></a>
# **platformSshKeyAll**
> PlatformTRPCResult platformSshKeyAll()

List all SSH keys

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SshKeyApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformSshKeyAll()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SshKeyApi#platformSshKeyAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SshKeyApi#platformSshKeyAll")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="platformSshKeyCreate"></a>
# **platformSshKeyCreate**
> PlatformTRPCResult platformSshKeyCreate(platformSshKeyCreateRequest)

Add an SSH key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SshKeyApi()
val platformSshKeyCreateRequest : PlatformSshKeyCreateRequest =  // PlatformSshKeyCreateRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformSshKeyCreate(platformSshKeyCreateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SshKeyApi#platformSshKeyCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SshKeyApi#platformSshKeyCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformSshKeyCreateRequest** | [**PlatformSshKeyCreateRequest**](PlatformSshKeyCreateRequest.md)|  | |

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

<a id="platformSshKeyGenerate"></a>
# **platformSshKeyGenerate**
> PlatformTRPCResult platformSshKeyGenerate()

Generate a new SSH key pair

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SshKeyApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformSshKeyGenerate()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SshKeyApi#platformSshKeyGenerate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SshKeyApi#platformSshKeyGenerate")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="platformSshKeyRemove"></a>
# **platformSshKeyRemove**
> PlatformTRPCResult platformSshKeyRemove(platformSshKeyRemoveRequest)

Remove an SSH key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SshKeyApi()
val platformSshKeyRemoveRequest : PlatformSshKeyRemoveRequest =  // PlatformSshKeyRemoveRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformSshKeyRemove(platformSshKeyRemoveRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SshKeyApi#platformSshKeyRemove")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SshKeyApi#platformSshKeyRemove")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformSshKeyRemoveRequest** | [**PlatformSshKeyRemoveRequest**](PlatformSshKeyRemoveRequest.md)|  | |

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

