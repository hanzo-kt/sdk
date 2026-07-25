# OauthAppsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**flowDeleteOAuthApp**](OauthAppsApi.md#flowDeleteOAuthApp) | **DELETE** /v1/flow/oauth-apps/{id} | Delete an OAuth app (EE) |
| [**flowListOAuthApps**](OauthAppsApi.md#flowListOAuthApps) | **GET** /v1/flow/oauth-apps | List OAuth app configurations (EE) |
| [**flowUpsertOAuthApp**](OauthAppsApi.md#flowUpsertOAuthApp) | **POST** /v1/flow/oauth-apps | Upsert an OAuth app (EE) |


<a id="flowDeleteOAuthApp"></a>
# **flowDeleteOAuthApp**
> flowDeleteOAuthApp(id)

Delete an OAuth app (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OauthAppsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.flowDeleteOAuthApp(id)
} catch (e: ClientException) {
    println("4xx response calling OauthAppsApi#flowDeleteOAuthApp")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OauthAppsApi#flowDeleteOAuthApp")
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

<a id="flowListOAuthApps"></a>
# **flowListOAuthApps**
> kotlin.Any flowListOAuthApps()

List OAuth app configurations (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OauthAppsApi()
try {
    val result : kotlin.Any = apiInstance.flowListOAuthApps()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OauthAppsApi#flowListOAuthApps")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OauthAppsApi#flowListOAuthApps")
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

<a id="flowUpsertOAuthApp"></a>
# **flowUpsertOAuthApp**
> kotlin.Any flowUpsertOAuthApp(flowUpsertOAuthAppRequest)

Upsert an OAuth app (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OauthAppsApi()
val flowUpsertOAuthAppRequest : FlowUpsertOAuthAppRequest =  // FlowUpsertOAuthAppRequest | 
try {
    val result : kotlin.Any = apiInstance.flowUpsertOAuthApp(flowUpsertOAuthAppRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OauthAppsApi#flowUpsertOAuthApp")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OauthAppsApi#flowUpsertOAuthApp")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowUpsertOAuthAppRequest** | [**FlowUpsertOAuthAppRequest**](FlowUpsertOAuthAppRequest.md)|  | |

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

