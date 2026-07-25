# ProjectReleasesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**flowCreateProjectRelease**](ProjectReleasesApi.md#flowCreateProjectRelease) | **POST** /v1/flow/project-releases | Create a release (EE) |
| [**flowListProjectReleases**](ProjectReleasesApi.md#flowListProjectReleases) | **GET** /v1/flow/project-releases | List releases (EE) |


<a id="flowCreateProjectRelease"></a>
# **flowCreateProjectRelease**
> kotlin.Any flowCreateProjectRelease(body)

Create a release (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectReleasesApi()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.flowCreateProjectRelease(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectReleasesApi#flowCreateProjectRelease")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectReleasesApi#flowCreateProjectRelease")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

<a id="flowListProjectReleases"></a>
# **flowListProjectReleases**
> kotlin.Any flowListProjectReleases()

List releases (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectReleasesApi()
try {
    val result : kotlin.Any = apiInstance.flowListProjectReleases()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectReleasesApi#flowListProjectReleases")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectReleasesApi#flowListProjectReleases")
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

