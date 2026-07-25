# GithubApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformGithubGetGithubBranches**](GithubApi.md#platformGithubGetGithubBranches) | **GET** /v1/platform/github/getGithubBranches | List branches for a repository |
| [**platformGithubGetGithubRepositories**](GithubApi.md#platformGithubGetGithubRepositories) | **GET** /v1/platform/github/getGithubRepositories | List repos from a GitHub installation |
| [**platformGithubGithubProviders**](GithubApi.md#platformGithubGithubProviders) | **GET** /v1/platform/github/githubProviders | List GitHub installations |


<a id="platformGithubGetGithubBranches"></a>
# **platformGithubGetGithubBranches**
> PlatformTRPCResult platformGithubGetGithubBranches(input)

List branches for a repository

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GithubApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformGithubGetGithubBranches(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GithubApi#platformGithubGetGithubBranches")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GithubApi#platformGithubGetGithubBranches")
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

<a id="platformGithubGetGithubRepositories"></a>
# **platformGithubGetGithubRepositories**
> PlatformTRPCResult platformGithubGetGithubRepositories(input)

List repos from a GitHub installation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GithubApi()
val input : kotlin.String = input_example // kotlin.String | URL-encoded JSON input for tRPC queries
try {
    val result : PlatformTRPCResult = apiInstance.platformGithubGetGithubRepositories(input)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GithubApi#platformGithubGetGithubRepositories")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GithubApi#platformGithubGetGithubRepositories")
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

<a id="platformGithubGithubProviders"></a>
# **platformGithubGithubProviders**
> PlatformTRPCResult platformGithubGithubProviders()

List GitHub installations

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GithubApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformGithubGithubProviders()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GithubApi#platformGithubGithubProviders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GithubApi#platformGithubGithubProviders")
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

