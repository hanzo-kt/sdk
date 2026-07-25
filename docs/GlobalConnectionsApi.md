# GlobalConnectionsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoListGlobalConnections**](GlobalConnectionsApi.md#autoListGlobalConnections) | **GET** /v1/auto/global-connections | List platform-wide connections (EE) |
| [**flowCreateGlobalConnection**](GlobalConnectionsApi.md#flowCreateGlobalConnection) | **POST** /v1/flow/global-connections | Create a global connection (EE) |
| [**flowDeleteGlobalConnection**](GlobalConnectionsApi.md#flowDeleteGlobalConnection) | **DELETE** /v1/flow/global-connections/{id} | Delete a global connection (EE) |
| [**flowListGlobalConnections**](GlobalConnectionsApi.md#flowListGlobalConnections) | **GET** /v1/flow/global-connections | List platform-wide connections (EE) |
| [**flowUpdateGlobalConnection**](GlobalConnectionsApi.md#flowUpdateGlobalConnection) | **POST** /v1/flow/global-connections/{id} | Update a global connection (EE) |


<a id="autoListGlobalConnections"></a>
# **autoListGlobalConnections**
> kotlin.Any autoListGlobalConnections()

List platform-wide connections (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GlobalConnectionsApi()
try {
    val result : kotlin.Any = apiInstance.autoListGlobalConnections()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GlobalConnectionsApi#autoListGlobalConnections")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GlobalConnectionsApi#autoListGlobalConnections")
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

<a id="flowCreateGlobalConnection"></a>
# **flowCreateGlobalConnection**
> kotlin.Any flowCreateGlobalConnection(body)

Create a global connection (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GlobalConnectionsApi()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.flowCreateGlobalConnection(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GlobalConnectionsApi#flowCreateGlobalConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GlobalConnectionsApi#flowCreateGlobalConnection")
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

<a id="flowDeleteGlobalConnection"></a>
# **flowDeleteGlobalConnection**
> flowDeleteGlobalConnection(id)

Delete a global connection (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GlobalConnectionsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.flowDeleteGlobalConnection(id)
} catch (e: ClientException) {
    println("4xx response calling GlobalConnectionsApi#flowDeleteGlobalConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GlobalConnectionsApi#flowDeleteGlobalConnection")
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

<a id="flowListGlobalConnections"></a>
# **flowListGlobalConnections**
> kotlin.Any flowListGlobalConnections()

List platform-wide connections (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GlobalConnectionsApi()
try {
    val result : kotlin.Any = apiInstance.flowListGlobalConnections()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GlobalConnectionsApi#flowListGlobalConnections")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GlobalConnectionsApi#flowListGlobalConnections")
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

<a id="flowUpdateGlobalConnection"></a>
# **flowUpdateGlobalConnection**
> kotlin.Any flowUpdateGlobalConnection(id, body)

Update a global connection (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = GlobalConnectionsApi()
val id : kotlin.String = id_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.flowUpdateGlobalConnection(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GlobalConnectionsApi#flowUpdateGlobalConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GlobalConnectionsApi#flowUpdateGlobalConnection")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
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

