# ExperimentalApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchGetExperimentalFeatures**](ExperimentalApi.md#searchGetExperimentalFeatures) | **GET** /v1/search/experimental-features | Get runtime-togglable experimental features |
| [**searchUpdateExperimentalFeatures**](ExperimentalApi.md#searchUpdateExperimentalFeatures) | **PATCH** /v1/search/experimental-features | Toggle experimental features |


<a id="searchGetExperimentalFeatures"></a>
# **searchGetExperimentalFeatures**
> SearchRuntimeTogglableFeatures searchGetExperimentalFeatures()

Get runtime-togglable experimental features

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ExperimentalApi()
try {
    val result : SearchRuntimeTogglableFeatures = apiInstance.searchGetExperimentalFeatures()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ExperimentalApi#searchGetExperimentalFeatures")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ExperimentalApi#searchGetExperimentalFeatures")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**SearchRuntimeTogglableFeatures**](SearchRuntimeTogglableFeatures.md)

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

<a id="searchUpdateExperimentalFeatures"></a>
# **searchUpdateExperimentalFeatures**
> SearchRuntimeTogglableFeatures searchUpdateExperimentalFeatures(searchRuntimeTogglableFeatures)

Toggle experimental features

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ExperimentalApi()
val searchRuntimeTogglableFeatures : SearchRuntimeTogglableFeatures =  // SearchRuntimeTogglableFeatures | 
try {
    val result : SearchRuntimeTogglableFeatures = apiInstance.searchUpdateExperimentalFeatures(searchRuntimeTogglableFeatures)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ExperimentalApi#searchUpdateExperimentalFeatures")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ExperimentalApi#searchUpdateExperimentalFeatures")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchRuntimeTogglableFeatures** | [**SearchRuntimeTogglableFeatures**](SearchRuntimeTogglableFeatures.md)|  | |

### Return type

[**SearchRuntimeTogglableFeatures**](SearchRuntimeTogglableFeatures.md)

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

