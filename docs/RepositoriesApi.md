# RepositoriesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**registryDeleteRepository**](RepositoriesApi.md#registryDeleteRepository) | **DELETE** /v1/registry/projects/{name}/repositories/{repo} | Delete repository |
| [**registryGetRepository**](RepositoriesApi.md#registryGetRepository) | **GET** /v1/registry/projects/{name}/repositories/{repo} | Get repository |
| [**registryListRepositories**](RepositoriesApi.md#registryListRepositories) | **GET** /v1/registry/projects/{name}/repositories | List repositories |


<a id="registryDeleteRepository"></a>
# **registryDeleteRepository**
> kotlin.Any registryDeleteRepository(name, repo)

Delete repository

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RepositoriesApi()
val name : kotlin.String = name_example // kotlin.String | 
val repo : kotlin.String = repo_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.registryDeleteRepository(name, repo)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RepositoriesApi#registryDeleteRepository")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RepositoriesApi#registryDeleteRepository")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **repo** | **kotlin.String**|  | |

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

<a id="registryGetRepository"></a>
# **registryGetRepository**
> RegistryRepository registryGetRepository(name, repo)

Get repository

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RepositoriesApi()
val name : kotlin.String = name_example // kotlin.String | 
val repo : kotlin.String = repo_example // kotlin.String | 
try {
    val result : RegistryRepository = apiInstance.registryGetRepository(name, repo)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RepositoriesApi#registryGetRepository")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RepositoriesApi#registryGetRepository")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **repo** | **kotlin.String**|  | |

### Return type

[**RegistryRepository**](RegistryRepository.md)

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

<a id="registryListRepositories"></a>
# **registryListRepositories**
> kotlin.collections.List&lt;RegistryRepository&gt; registryListRepositories(name, q, page, pageSize, sort)

List repositories

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RepositoriesApi()
val name : kotlin.String = name_example // kotlin.String | 
val q : kotlin.String = q_example // kotlin.String | Search query
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val sort : kotlin.String = sort_example // kotlin.String | 
try {
    val result : kotlin.collections.List<RegistryRepository> = apiInstance.registryListRepositories(name, q, page, pageSize, sort)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RepositoriesApi#registryListRepositories")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RepositoriesApi#registryListRepositories")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| **q** | **kotlin.String**| Search query | [optional] |
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 10] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sort** | **kotlin.String**|  | [optional] [enum: name, pull_count, update_time] |

### Return type

[**kotlin.collections.List&lt;RegistryRepository&gt;**](RegistryRepository.md)

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

