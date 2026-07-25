# DashboardApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsGetDashboardSecretsOverview**](DashboardApi.md#kmsGetDashboardSecretsOverview) | **GET** /v1/kms/dashboard/{projectId}/secrets-overview | Get secrets overview for the dashboard |


<a id="kmsGetDashboardSecretsOverview"></a>
# **kmsGetDashboardSecretsOverview**
> KmsDashboardSecrets kmsGetDashboardSecretsOverview(projectId, environments, secretPath)

Get secrets overview for the dashboard

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DashboardApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val environments : kotlin.String = environments_example // kotlin.String | 
val secretPath : kotlin.String = secretPath_example // kotlin.String | 
try {
    val result : KmsDashboardSecrets = apiInstance.kmsGetDashboardSecretsOverview(projectId, environments, secretPath)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DashboardApi#kmsGetDashboardSecretsOverview")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DashboardApi#kmsGetDashboardSecretsOverview")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **java.util.UUID**|  | |
| **environments** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **secretPath** | **kotlin.String**|  | [optional] [default to &quot;/&quot;] |

### Return type

[**KmsDashboardSecrets**](KmsDashboardSecrets.md)

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

