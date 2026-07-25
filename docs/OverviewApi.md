# OverviewApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**adminAdminOverview**](OverviewApi.md#adminAdminOverview) | **GET** /v1/admin/overview | Fleet overview tiles |
| [**adminAdminProducts**](OverviewApi.md#adminAdminProducts) | **GET** /v1/admin/products | Product / workload registry |
| [**adminAdminSync**](OverviewApi.md#adminAdminSync) | **POST** /v1/admin/sync | Trigger a fleet re-read |
| [**adminAdminUsage**](OverviewApi.md#adminAdminUsage) | **GET** /v1/admin/usage | Fleet usage roll-up |


<a id="adminAdminOverview"></a>
# **adminAdminOverview**
> AdminAdminOverview200Response adminAdminOverview()

Fleet overview tiles

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OverviewApi()
try {
    val result : AdminAdminOverview200Response = apiInstance.adminAdminOverview()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OverviewApi#adminAdminOverview")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OverviewApi#adminAdminOverview")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AdminAdminOverview200Response**](AdminAdminOverview200Response.md)

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

<a id="adminAdminProducts"></a>
# **adminAdminProducts**
> AdminAdminProducts200Response adminAdminProducts()

Product / workload registry

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OverviewApi()
try {
    val result : AdminAdminProducts200Response = apiInstance.adminAdminProducts()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OverviewApi#adminAdminProducts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OverviewApi#adminAdminProducts")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AdminAdminProducts200Response**](AdminAdminProducts200Response.md)

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

<a id="adminAdminSync"></a>
# **adminAdminSync**
> AdminAdminSync200Response adminAdminSync()

Trigger a fleet re-read

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OverviewApi()
try {
    val result : AdminAdminSync200Response = apiInstance.adminAdminSync()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OverviewApi#adminAdminSync")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OverviewApi#adminAdminSync")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AdminAdminSync200Response**](AdminAdminSync200Response.md)

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

<a id="adminAdminUsage"></a>
# **adminAdminUsage**
> AdminAdminUsage200Response adminAdminUsage(org)

Fleet usage roll-up

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OverviewApi()
val org : kotlin.String = org_example // kotlin.String | Scope to one org (default fleet)
try {
    val result : AdminAdminUsage200Response = apiInstance.adminAdminUsage(org)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OverviewApi#adminAdminUsage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OverviewApi#adminAdminUsage")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **org** | **kotlin.String**| Scope to one org (default fleet) | [optional] |

### Return type

[**AdminAdminUsage200Response**](AdminAdminUsage200Response.md)

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

