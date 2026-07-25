# SmartHTTPApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gitGitInfoRefs**](SmartHTTPApi.md#gitGitInfoRefs) | **GET** /v1/git/{org}/{repo}/info/refs | Git smart-HTTP ref advertisement |
| [**gitGitReceivePack**](SmartHTTPApi.md#gitGitReceivePack) | **POST** /v1/git/{org}/{repo}/git-receive-pack | Git receive-pack (push) |
| [**gitGitUploadPack**](SmartHTTPApi.md#gitGitUploadPack) | **POST** /v1/git/{org}/{repo}/git-upload-pack | Git upload-pack (clone / fetch) |


<a id="gitGitInfoRefs"></a>
# **gitGitInfoRefs**
> java.io.File gitGitInfoRefs(org, repo, service)

Git smart-HTTP ref advertisement

The ref-advertisement phase. &#x60;?service&#x3D;&#x60; selects git-upload-pack (fetch) or git-receive-pack (push).

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SmartHTTPApi()
val org : kotlin.String = org_example // kotlin.String | 
val repo : kotlin.String = repo_example // kotlin.String | 
val service : kotlin.String = service_example // kotlin.String | 
try {
    val result : java.io.File = apiInstance.gitGitInfoRefs(org, repo, service)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SmartHTTPApi#gitGitInfoRefs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SmartHTTPApi#gitGitInfoRefs")
    e.printStackTrace()
}
```

### Parameters
| **org** | **kotlin.String**|  | |
| **repo** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **service** | **kotlin.String**|  | [enum: git-upload-pack, git-receive-pack] |

### Return type

[**java.io.File**](java.io.File.md)

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

<a id="gitGitReceivePack"></a>
# **gitGitReceivePack**
> java.io.File gitGitReceivePack(org, repo, body)

Git receive-pack (push)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SmartHTTPApi()
val org : kotlin.String = org_example // kotlin.String | 
val repo : kotlin.String = repo_example // kotlin.String | 
val body : java.io.File = BINARY_DATA_HERE // java.io.File | 
try {
    val result : java.io.File = apiInstance.gitGitReceivePack(org, repo, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SmartHTTPApi#gitGitReceivePack")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SmartHTTPApi#gitGitReceivePack")
    e.printStackTrace()
}
```

### Parameters
| **org** | **kotlin.String**|  | |
| **repo** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **java.io.File**|  | |

### Return type

[**java.io.File**](java.io.File.md)

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

<a id="gitGitUploadPack"></a>
# **gitGitUploadPack**
> java.io.File gitGitUploadPack(org, repo, body)

Git upload-pack (clone / fetch)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SmartHTTPApi()
val org : kotlin.String = org_example // kotlin.String | 
val repo : kotlin.String = repo_example // kotlin.String | 
val body : java.io.File = BINARY_DATA_HERE // java.io.File | 
try {
    val result : java.io.File = apiInstance.gitGitUploadPack(org, repo, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SmartHTTPApi#gitGitUploadPack")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SmartHTTPApi#gitGitUploadPack")
    e.printStackTrace()
}
```

### Parameters
| **org** | **kotlin.String**|  | |
| **repo** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **java.io.File**|  | |

### Return type

[**java.io.File**](java.io.File.md)

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

