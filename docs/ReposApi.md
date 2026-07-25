# ReposApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gitCreateRepo**](ReposApi.md#gitCreateRepo) | **POST** /v1/git/repos | Create a bare repo |
| [**gitDeleteRepo**](ReposApi.md#gitDeleteRepo) | **DELETE** /v1/git/repos/{name} | Delete a repo and purge its storage |
| [**gitGetRepo**](ReposApi.md#gitGetRepo) | **GET** /v1/git/repos/{name} | Repo detail (branches + resolved HEAD) |
| [**gitGitPush**](ReposApi.md#gitGitPush) | **POST** /v1/git/repos/{name}/push | Client-less push (build a commit from posted files) |
| [**gitListRepos**](ReposApi.md#gitListRepos) | **GET** /v1/git/repos | List the tenant&#39;s repos |


<a id="gitCreateRepo"></a>
# **gitCreateRepo**
> GitRepo gitCreateRepo(gitCreateRepo)

Create a bare repo

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReposApi()
val gitCreateRepo : GitCreateRepo =  // GitCreateRepo | 
try {
    val result : GitRepo = apiInstance.gitCreateRepo(gitCreateRepo)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReposApi#gitCreateRepo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReposApi#gitCreateRepo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gitCreateRepo** | [**GitCreateRepo**](GitCreateRepo.md)|  | |

### Return type

[**GitRepo**](GitRepo.md)

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

<a id="gitDeleteRepo"></a>
# **gitDeleteRepo**
> gitDeleteRepo(name)

Delete a repo and purge its storage

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReposApi()
val name : kotlin.String = name_example // kotlin.String | Repo name (a trailing \".git\" is stripped)
try {
    apiInstance.gitDeleteRepo(name)
} catch (e: ClientException) {
    println("4xx response calling ReposApi#gitDeleteRepo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReposApi#gitDeleteRepo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| Repo name (a trailing \&quot;.git\&quot; is stripped) | |

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
 - **Accept**: application/json

<a id="gitGetRepo"></a>
# **gitGetRepo**
> GitRepo gitGetRepo(name)

Repo detail (branches + resolved HEAD)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReposApi()
val name : kotlin.String = name_example // kotlin.String | Repo name (a trailing \".git\" is stripped)
try {
    val result : GitRepo = apiInstance.gitGetRepo(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReposApi#gitGetRepo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReposApi#gitGetRepo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| Repo name (a trailing \&quot;.git\&quot; is stripped) | |

### Return type

[**GitRepo**](GitRepo.md)

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

<a id="gitGitPush"></a>
# **gitGitPush**
> GitPushResult gitGitPush(name, gitPushRequest)

Client-less push (build a commit from posted files)

Builds a tree + commit from the posted files, advances the branch ref, and fires the git-push-to-deploy build exactly as a real receive-pack would — for builders with no local git client. Creates the repo on the first push. File content is UTF-8 by default, or base64 when the file&#39;s &#x60;encoding&#x60; is &#x60;base64&#x60;. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReposApi()
val name : kotlin.String = name_example // kotlin.String | Repo name (a trailing \".git\" is stripped)
val gitPushRequest : GitPushRequest =  // GitPushRequest | 
try {
    val result : GitPushResult = apiInstance.gitGitPush(name, gitPushRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReposApi#gitGitPush")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReposApi#gitGitPush")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**| Repo name (a trailing \&quot;.git\&quot; is stripped) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gitPushRequest** | [**GitPushRequest**](GitPushRequest.md)|  | |

### Return type

[**GitPushResult**](GitPushResult.md)

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

<a id="gitListRepos"></a>
# **gitListRepos**
> GitListRepos200Response gitListRepos()

List the tenant&#39;s repos

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReposApi()
try {
    val result : GitListRepos200Response = apiInstance.gitListRepos()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReposApi#gitListRepos")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReposApi#gitListRepos")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**GitListRepos200Response**](GitListRepos200Response.md)

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

