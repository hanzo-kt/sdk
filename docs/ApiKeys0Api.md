# ApiKeysApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoCreateApiKey**](ApiKeysApi.md#autoCreateApiKey) | **POST** /v1/auto/api-keys | Create an API key (EE) |
| [**autoDeleteApiKey**](ApiKeysApi.md#autoDeleteApiKey) | **DELETE** /v1/auto/api-keys/{id} | Delete an API key (EE) |
| [**autoListApiKeys**](ApiKeysApi.md#autoListApiKeys) | **GET** /v1/auto/api-keys | List API keys (EE) |
| [**flowCreateApiKey**](ApiKeysApi.md#flowCreateApiKey) | **POST** /v1/flow/api-keys | Create an API key (EE) |
| [**flowDeleteApiKey**](ApiKeysApi.md#flowDeleteApiKey) | **DELETE** /v1/flow/api-keys/{id} | Delete an API key (EE) |
| [**flowListApiKeys**](ApiKeysApi.md#flowListApiKeys) | **GET** /v1/flow/api-keys | List API keys (EE) |


<a id="autoCreateApiKey"></a>
# **autoCreateApiKey**
> kotlin.Any autoCreateApiKey(autoCreateApiKeyRequest)

Create an API key (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApiKeysApi()
val autoCreateApiKeyRequest : AutoCreateApiKeyRequest =  // AutoCreateApiKeyRequest | 
try {
    val result : kotlin.Any = apiInstance.autoCreateApiKey(autoCreateApiKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApiKeysApi#autoCreateApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApiKeysApi#autoCreateApiKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateApiKeyRequest** | [**AutoCreateApiKeyRequest**](AutoCreateApiKeyRequest.md)|  | |

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

<a id="autoDeleteApiKey"></a>
# **autoDeleteApiKey**
> autoDeleteApiKey(id)

Delete an API key (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApiKeysApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.autoDeleteApiKey(id)
} catch (e: ClientException) {
    println("4xx response calling ApiKeysApi#autoDeleteApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApiKeysApi#autoDeleteApiKey")
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

<a id="autoListApiKeys"></a>
# **autoListApiKeys**
> kotlin.Any autoListApiKeys()

List API keys (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApiKeysApi()
try {
    val result : kotlin.Any = apiInstance.autoListApiKeys()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApiKeysApi#autoListApiKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApiKeysApi#autoListApiKeys")
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

<a id="flowCreateApiKey"></a>
# **flowCreateApiKey**
> kotlin.Any flowCreateApiKey(autoCreateApiKeyRequest)

Create an API key (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApiKeysApi()
val autoCreateApiKeyRequest : AutoCreateApiKeyRequest =  // AutoCreateApiKeyRequest | 
try {
    val result : kotlin.Any = apiInstance.flowCreateApiKey(autoCreateApiKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApiKeysApi#flowCreateApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApiKeysApi#flowCreateApiKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateApiKeyRequest** | [**AutoCreateApiKeyRequest**](AutoCreateApiKeyRequest.md)|  | |

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

<a id="flowDeleteApiKey"></a>
# **flowDeleteApiKey**
> flowDeleteApiKey(id)

Delete an API key (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApiKeysApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.flowDeleteApiKey(id)
} catch (e: ClientException) {
    println("4xx response calling ApiKeysApi#flowDeleteApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApiKeysApi#flowDeleteApiKey")
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

<a id="flowListApiKeys"></a>
# **flowListApiKeys**
> kotlin.Any flowListApiKeys()

List API keys (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ApiKeysApi()
try {
    val result : kotlin.Any = apiInstance.flowListApiKeys()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ApiKeysApi#flowListApiKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ApiKeysApi#flowListApiKeys")
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

