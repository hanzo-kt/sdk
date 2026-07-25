# ModulesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**frameworkGetModule**](ModulesApi.md#frameworkGetModule) | **GET** /v1/framework/modules/{module} | Inspect a module and its install state in this org |
| [**frameworkInstallModule**](ModulesApi.md#frameworkInstallModule) | **POST** /v1/framework/modules/{module}/install | Install a module&#39;s DocType fixtures into this org (idempotent) |
| [**frameworkListModules**](ModulesApi.md#frameworkListModules) | **GET** /v1/framework/modules | List registered app-lane modules |


<a id="frameworkGetModule"></a>
# **frameworkGetModule**
> FrameworkGetModule200Response frameworkGetModule(module)

Inspect a module and its install state in this org

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModulesApi()
val module : kotlin.String = module_example // kotlin.String | 
try {
    val result : FrameworkGetModule200Response = apiInstance.frameworkGetModule(module)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModulesApi#frameworkGetModule")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModulesApi#frameworkGetModule")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **module** | **kotlin.String**|  | |

### Return type

[**FrameworkGetModule200Response**](FrameworkGetModule200Response.md)

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

<a id="frameworkInstallModule"></a>
# **frameworkInstallModule**
> FrameworkInstallModule200Response frameworkInstallModule(module)

Install a module&#39;s DocType fixtures into this org (idempotent)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModulesApi()
val module : kotlin.String = module_example // kotlin.String | 
try {
    val result : FrameworkInstallModule200Response = apiInstance.frameworkInstallModule(module)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModulesApi#frameworkInstallModule")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModulesApi#frameworkInstallModule")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **module** | **kotlin.String**|  | |

### Return type

[**FrameworkInstallModule200Response**](FrameworkInstallModule200Response.md)

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

<a id="frameworkListModules"></a>
# **frameworkListModules**
> FrameworkListModules200Response frameworkListModules()

List registered app-lane modules

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModulesApi()
try {
    val result : FrameworkListModules200Response = apiInstance.frameworkListModules()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModulesApi#frameworkListModules")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModulesApi#frameworkListModules")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**FrameworkListModules200Response**](FrameworkListModules200Response.md)

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

