# SigningKeysApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**flowCreateSigningKey**](SigningKeysApi.md#flowCreateSigningKey) | **POST** /v1/flow/signing-keys | Create a signing key (EE) |
| [**flowListSigningKeys**](SigningKeysApi.md#flowListSigningKeys) | **GET** /v1/flow/signing-keys | List signing keys (EE) |


<a id="flowCreateSigningKey"></a>
# **flowCreateSigningKey**
> kotlin.Any flowCreateSigningKey(autoCreateApiKeyRequest)

Create a signing key (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SigningKeysApi()
val autoCreateApiKeyRequest : AutoCreateApiKeyRequest =  // AutoCreateApiKeyRequest | 
try {
    val result : kotlin.Any = apiInstance.flowCreateSigningKey(autoCreateApiKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SigningKeysApi#flowCreateSigningKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SigningKeysApi#flowCreateSigningKey")
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

<a id="flowListSigningKeys"></a>
# **flowListSigningKeys**
> kotlin.Any flowListSigningKeys()

List signing keys (EE)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SigningKeysApi()
try {
    val result : kotlin.Any = apiInstance.flowListSigningKeys()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SigningKeysApi#flowListSigningKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SigningKeysApi#flowListSigningKeys")
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

