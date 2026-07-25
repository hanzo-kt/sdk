# GitReposApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoConnectGitRepo**](GitReposApi.md#autoConnectGitRepo) | **POST** /v1/auto/git-repos | Connect a git repo for sync (EE) |
| [**autoListGitRepos**](GitReposApi.md#autoListGitRepos) | **GET** /v1/auto/git-repos | List connected git repos (EE) |
| [**flowConnectGitRepo**](GitReposApi.md#flowConnectGitRepo) | **POST** /v1/flow/git-repos | Connect a git repo for sync (EE) |
| [**flowDisconnectGitRepo**](GitReposApi.md#flowDisconnectGitRepo) | **DELETE** /v1/flow/git-repos/{id} | Disconnect a git repo (EE) |
| [**flowListGitRepos**](GitReposApi.md#flowListGitRepos) | **GET** /v1/flow/git-repos | List connected git repos (EE) |
| [**flowPullFromGitRepo**](GitReposApi.md#flowPullFromGitRepo) | **POST** /v1/flow/git-repos/{id}/pull | Pull flows from git (EE) |
| [**flowPushToGitRepo**](GitReposApi.md#flowPushToGitRepo) | **POST** /v1/flow/git-repos/{id}/push | Push flows to git (EE) |


<a id="autoConnectGitRepo"></a>
# **autoConnectGitRepo**
> kotlin.Any autoConnectGitRepo(autoConnectGitRepoRequest)

Connect a git repo for sync (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GitReposApi()
val autoConnectGitRepoRequest : AutoConnectGitRepoRequest =  // AutoConnectGitRepoRequest | 
try {
    val result : kotlin.Any = apiInstance.autoConnectGitRepo(autoConnectGitRepoRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GitReposApi#autoConnectGitRepo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GitReposApi#autoConnectGitRepo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoConnectGitRepoRequest** | [**AutoConnectGitRepoRequest**](AutoConnectGitRepoRequest.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

<a id="autoListGitRepos"></a>
# **autoListGitRepos**
> kotlin.Any autoListGitRepos()

List connected git repos (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GitReposApi()
try {
    val result : kotlin.Any = apiInstance.autoListGitRepos()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GitReposApi#autoListGitRepos")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GitReposApi#autoListGitRepos")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

<a id="flowConnectGitRepo"></a>
# **flowConnectGitRepo**
> kotlin.Any flowConnectGitRepo(flowConnectGitRepoRequest)

Connect a git repo for sync (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GitReposApi()
val flowConnectGitRepoRequest : FlowConnectGitRepoRequest =  // FlowConnectGitRepoRequest | 
try {
    val result : kotlin.Any = apiInstance.flowConnectGitRepo(flowConnectGitRepoRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GitReposApi#flowConnectGitRepo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GitReposApi#flowConnectGitRepo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowConnectGitRepoRequest** | [**FlowConnectGitRepoRequest**](FlowConnectGitRepoRequest.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

<a id="flowDisconnectGitRepo"></a>
# **flowDisconnectGitRepo**
> flowDisconnectGitRepo(id)

Disconnect a git repo (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GitReposApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.flowDisconnectGitRepo(id)
} catch (e: ClientException) {
    println("4xx response calling GitReposApi#flowDisconnectGitRepo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GitReposApi#flowDisconnectGitRepo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="flowListGitRepos"></a>
# **flowListGitRepos**
> kotlin.Any flowListGitRepos()

List connected git repos (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GitReposApi()
try {
    val result : kotlin.Any = apiInstance.flowListGitRepos()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GitReposApi#flowListGitRepos")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GitReposApi#flowListGitRepos")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

<a id="flowPullFromGitRepo"></a>
# **flowPullFromGitRepo**
> kotlin.Any flowPullFromGitRepo(id)

Pull flows from git (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GitReposApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowPullFromGitRepo(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GitReposApi#flowPullFromGitRepo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GitReposApi#flowPullFromGitRepo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

<a id="flowPushToGitRepo"></a>
# **flowPushToGitRepo**
> kotlin.Any flowPushToGitRepo(id)

Push flows to git (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GitReposApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowPushToGitRepo(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GitReposApi#flowPushToGitRepo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GitReposApi#flowPushToGitRepo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

