# ArtifactsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**registryCreateTag**](ArtifactsApi.md#registryCreateTag) | **POST** /v1/registry/projects/{name}/repositories/{repo}/artifacts/{digest}/tags/{tag} | Create tag |
| [**registryDeleteArtifact**](ArtifactsApi.md#registryDeleteArtifact) | **DELETE** /v1/registry/projects/{name}/repositories/{repo}/artifacts/{digest} | Delete artifact |
| [**registryDeleteTag**](ArtifactsApi.md#registryDeleteTag) | **DELETE** /v1/registry/projects/{name}/repositories/{repo}/artifacts/{digest}/tags/{tag} | Delete tag |
| [**registryGetArtifact**](ArtifactsApi.md#registryGetArtifact) | **GET** /v1/registry/projects/{name}/repositories/{repo}/artifacts/{digest} | Get artifact |
| [**registryListArtifacts**](ArtifactsApi.md#registryListArtifacts) | **GET** /v1/registry/projects/{name}/repositories/{repo}/artifacts | List artifacts |
| [**registryListTags**](ArtifactsApi.md#registryListTags) | **GET** /v1/registry/projects/{name}/repositories/{repo}/artifacts/{digest}/tags | List tags |


<a id="registryCreateTag"></a>
# **registryCreateTag**
> kotlin.Any registryCreateTag(name, repo, digest, tag)

Create tag

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArtifactsApi()
val name : kotlin.String = name_example // kotlin.String | 
val repo : kotlin.String = repo_example // kotlin.String | 
val digest : kotlin.String = digest_example // kotlin.String | 
val tag : kotlin.String = tag_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.registryCreateTag(name, repo, digest, tag)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArtifactsApi#registryCreateTag")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArtifactsApi#registryCreateTag")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| **repo** | **kotlin.String**|  | |
| **digest** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **tag** | **kotlin.String**|  | |

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

<a id="registryDeleteArtifact"></a>
# **registryDeleteArtifact**
> kotlin.Any registryDeleteArtifact(name, repo, digest)

Delete artifact

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArtifactsApi()
val name : kotlin.String = name_example // kotlin.String | 
val repo : kotlin.String = repo_example // kotlin.String | 
val digest : kotlin.String = digest_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.registryDeleteArtifact(name, repo, digest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArtifactsApi#registryDeleteArtifact")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArtifactsApi#registryDeleteArtifact")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| **repo** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **digest** | **kotlin.String**|  | |

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

<a id="registryDeleteTag"></a>
# **registryDeleteTag**
> kotlin.Any registryDeleteTag(name, repo, digest, tag)

Delete tag

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArtifactsApi()
val name : kotlin.String = name_example // kotlin.String | 
val repo : kotlin.String = repo_example // kotlin.String | 
val digest : kotlin.String = digest_example // kotlin.String | 
val tag : kotlin.String = tag_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.registryDeleteTag(name, repo, digest, tag)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArtifactsApi#registryDeleteTag")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArtifactsApi#registryDeleteTag")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| **repo** | **kotlin.String**|  | |
| **digest** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **tag** | **kotlin.String**|  | |

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

<a id="registryGetArtifact"></a>
# **registryGetArtifact**
> RegistryArtifact registryGetArtifact(name, repo, digest, withScanOverview)

Get artifact

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArtifactsApi()
val name : kotlin.String = name_example // kotlin.String | 
val repo : kotlin.String = repo_example // kotlin.String | 
val digest : kotlin.String = digest_example // kotlin.String | Artifact digest (sha256:...)
val withScanOverview : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : RegistryArtifact = apiInstance.registryGetArtifact(name, repo, digest, withScanOverview)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArtifactsApi#registryGetArtifact")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArtifactsApi#registryGetArtifact")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| **repo** | **kotlin.String**|  | |
| **digest** | **kotlin.String**| Artifact digest (sha256:...) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **withScanOverview** | **kotlin.Boolean**|  | [optional] [default to false] |

### Return type

[**RegistryArtifact**](RegistryArtifact.md)

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

<a id="registryListArtifacts"></a>
# **registryListArtifacts**
> kotlin.collections.List&lt;RegistryArtifact&gt; registryListArtifacts(name, repo, type, withTag, withScanOverview, page, pageSize)

List artifacts

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArtifactsApi()
val name : kotlin.String = name_example // kotlin.String | 
val repo : kotlin.String = repo_example // kotlin.String | 
val type : kotlin.String = type_example // kotlin.String | Filter by artifact type
val withTag : kotlin.Boolean = true // kotlin.Boolean | 
val withScanOverview : kotlin.Boolean = true // kotlin.Boolean | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.collections.List<RegistryArtifact> = apiInstance.registryListArtifacts(name, repo, type, withTag, withScanOverview, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArtifactsApi#registryListArtifacts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArtifactsApi#registryListArtifacts")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| **repo** | **kotlin.String**|  | |
| **type** | **kotlin.String**| Filter by artifact type | [optional] [enum: IMAGE, CHART, WASM] |
| **withTag** | **kotlin.Boolean**|  | [optional] [default to true] |
| **withScanOverview** | **kotlin.Boolean**|  | [optional] [default to false] |
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 10] |

### Return type

[**kotlin.collections.List&lt;RegistryArtifact&gt;**](RegistryArtifact.md)

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

<a id="registryListTags"></a>
# **registryListTags**
> kotlin.collections.List&lt;RegistryTag&gt; registryListTags(name, repo, digest, page, pageSize)

List tags

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArtifactsApi()
val name : kotlin.String = name_example // kotlin.String | 
val repo : kotlin.String = repo_example // kotlin.String | 
val digest : kotlin.String = digest_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.collections.List<RegistryTag> = apiInstance.registryListTags(name, repo, digest, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArtifactsApi#registryListTags")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArtifactsApi#registryListTags")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| **repo** | **kotlin.String**|  | |
| **digest** | **kotlin.String**|  | |
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 10] |

### Return type

[**kotlin.collections.List&lt;RegistryTag&gt;**](RegistryTag.md)

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

