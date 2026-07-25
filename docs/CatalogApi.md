# CatalogApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**promptsPromptCatalog**](CatalogApi.md#promptsPromptCatalog) | **GET** /v1/prompts/catalog | Read-only starter prompt library |
| [**visorListRegions**](CatalogApi.md#visorListRegions) | **GET** /v1/compute/regions | List the global compute region catalog |
| [**visorListSizes**](CatalogApi.md#visorListSizes) | **GET** /v1/compute/sizes | List the global compute size catalog |


<a id="promptsPromptCatalog"></a>
# **promptsPromptCatalog**
> PromptsPromptCatalog200Response promptsPromptCatalog()

Read-only starter prompt library

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CatalogApi()
try {
    val result : PromptsPromptCatalog200Response = apiInstance.promptsPromptCatalog()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CatalogApi#promptsPromptCatalog")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CatalogApi#promptsPromptCatalog")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PromptsPromptCatalog200Response**](PromptsPromptCatalog200Response.md)

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

<a id="visorListRegions"></a>
# **visorListRegions**
> kotlin.Any visorListRegions()

List the global compute region catalog

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CatalogApi()
try {
    val result : kotlin.Any = apiInstance.visorListRegions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CatalogApi#visorListRegions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CatalogApi#visorListRegions")
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

<a id="visorListSizes"></a>
# **visorListSizes**
> kotlin.Any visorListSizes()

List the global compute size catalog

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CatalogApi()
try {
    val result : kotlin.Any = apiInstance.visorListSizes()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CatalogApi#visorListSizes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CatalogApi#visorListSizes")
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

