# SecretSharingApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsCreateSharedSecret**](SecretSharingApi.md#kmsCreateSharedSecret) | **POST** /v1/kms/secret-sharing/shared | Create a shared secret |
| [**kmsDeleteSharedSecret**](SecretSharingApi.md#kmsDeleteSharedSecret) | **DELETE** /v1/kms/secret-sharing/shared/{sharedSecretId} | Delete a shared secret |
| [**kmsGetSharedSecret**](SecretSharingApi.md#kmsGetSharedSecret) | **GET** /v1/kms/secret-sharing/shared/{sharedSecretId} | Get a shared secret by ID (consumes a view) |
| [**kmsListSharedSecrets**](SecretSharingApi.md#kmsListSharedSecrets) | **GET** /v1/kms/secret-sharing/shared | List shared secrets created by the user |


<a id="kmsCreateSharedSecret"></a>
# **kmsCreateSharedSecret**
> KmsCreateSharedSecret200Response kmsCreateSharedSecret(kmsCreateSharedSecretRequest)

Create a shared secret

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretSharingApi()
val kmsCreateSharedSecretRequest : KmsCreateSharedSecretRequest =  // KmsCreateSharedSecretRequest | 
try {
    val result : KmsCreateSharedSecret200Response = apiInstance.kmsCreateSharedSecret(kmsCreateSharedSecretRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretSharingApi#kmsCreateSharedSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretSharingApi#kmsCreateSharedSecret")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateSharedSecretRequest** | [**KmsCreateSharedSecretRequest**](KmsCreateSharedSecretRequest.md)|  | |

### Return type

[**KmsCreateSharedSecret200Response**](KmsCreateSharedSecret200Response.md)

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

<a id="kmsDeleteSharedSecret"></a>
# **kmsDeleteSharedSecret**
> kotlin.Any kmsDeleteSharedSecret(sharedSecretId)

Delete a shared secret

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretSharingApi()
val sharedSecretId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kmsDeleteSharedSecret(sharedSecretId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretSharingApi#kmsDeleteSharedSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretSharingApi#kmsDeleteSharedSecret")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sharedSecretId** | **java.util.UUID**|  | |

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

<a id="kmsGetSharedSecret"></a>
# **kmsGetSharedSecret**
> KmsGetSharedSecret200Response kmsGetSharedSecret(sharedSecretId)

Get a shared secret by ID (consumes a view)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretSharingApi()
val sharedSecretId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsGetSharedSecret200Response = apiInstance.kmsGetSharedSecret(sharedSecretId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretSharingApi#kmsGetSharedSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretSharingApi#kmsGetSharedSecret")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sharedSecretId** | **java.util.UUID**|  | |

### Return type

[**KmsGetSharedSecret200Response**](KmsGetSharedSecret200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="kmsListSharedSecrets"></a>
# **kmsListSharedSecrets**
> KmsListSharedSecrets200Response kmsListSharedSecrets()

List shared secrets created by the user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretSharingApi()
try {
    val result : KmsListSharedSecrets200Response = apiInstance.kmsListSharedSecrets()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretSharingApi#kmsListSharedSecrets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretSharingApi#kmsListSharedSecrets")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**KmsListSharedSecrets200Response**](KmsListSharedSecrets200Response.md)

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

