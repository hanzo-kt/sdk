# AlertsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**flowCreateAlert**](AlertsApi.md#flowCreateAlert) | **POST** /v1/flow/alerts | Create an alert (EE) |
| [**flowDeleteAlert**](AlertsApi.md#flowDeleteAlert) | **DELETE** /v1/flow/alerts/{id} | Delete an alert (EE) |
| [**flowListAlerts**](AlertsApi.md#flowListAlerts) | **GET** /v1/flow/alerts | List alerts (EE) |


<a id="flowCreateAlert"></a>
# **flowCreateAlert**
> kotlin.Any flowCreateAlert(body)

Create an alert (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AlertsApi()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.flowCreateAlert(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AlertsApi#flowCreateAlert")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AlertsApi#flowCreateAlert")
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

<a id="flowDeleteAlert"></a>
# **flowDeleteAlert**
> flowDeleteAlert(id)

Delete an alert (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AlertsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.flowDeleteAlert(id)
} catch (e: ClientException) {
    println("4xx response calling AlertsApi#flowDeleteAlert")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AlertsApi#flowDeleteAlert")
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

<a id="flowListAlerts"></a>
# **flowListAlerts**
> kotlin.Any flowListAlerts()

List alerts (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AlertsApi()
try {
    val result : kotlin.Any = apiInstance.flowListAlerts()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AlertsApi#flowListAlerts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AlertsApi#flowListAlerts")
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

