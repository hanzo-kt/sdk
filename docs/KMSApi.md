# KMSApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsCreateKmsKey**](KMSApi.md#kmsCreateKmsKey) | **POST** /v1/kms/kms/keys | Create a KMS encryption key |
| [**kmsDecryptData**](KMSApi.md#kmsDecryptData) | **POST** /v1/kms/kms/keys/{keyId}/decrypt | Decrypt data with a KMS key |
| [**kmsDeleteKmsKey**](KMSApi.md#kmsDeleteKmsKey) | **DELETE** /v1/kms/kms/keys/{keyId} | Delete a KMS key |
| [**kmsEncryptData**](KMSApi.md#kmsEncryptData) | **POST** /v1/kms/kms/keys/{keyId}/encrypt | Encrypt data with a KMS key |
| [**kmsListKmsKeys**](KMSApi.md#kmsListKmsKeys) | **GET** /v1/kms/kms/keys | List KMS encryption keys |
| [**kmsUpdateKmsKey**](KMSApi.md#kmsUpdateKmsKey) | **PATCH** /v1/kms/kms/keys/{keyId} | Update a KMS key |


<a id="kmsCreateKmsKey"></a>
# **kmsCreateKmsKey**
> KmsCreateKmsKey200Response kmsCreateKmsKey(kmsCreateKmsKeyRequest)

Create a KMS encryption key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KMSApi()
val kmsCreateKmsKeyRequest : KmsCreateKmsKeyRequest =  // KmsCreateKmsKeyRequest | 
try {
    val result : KmsCreateKmsKey200Response = apiInstance.kmsCreateKmsKey(kmsCreateKmsKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KMSApi#kmsCreateKmsKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KMSApi#kmsCreateKmsKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateKmsKeyRequest** | [**KmsCreateKmsKeyRequest**](KmsCreateKmsKeyRequest.md)|  | |

### Return type

[**KmsCreateKmsKey200Response**](KmsCreateKmsKey200Response.md)

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

<a id="kmsDecryptData"></a>
# **kmsDecryptData**
> KmsDecryptDataResponse kmsDecryptData(keyId, kmsDecryptDataRequest)

Decrypt data with a KMS key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KMSApi()
val keyId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsDecryptDataRequest : KmsDecryptDataRequest =  // KmsDecryptDataRequest | 
try {
    val result : KmsDecryptDataResponse = apiInstance.kmsDecryptData(keyId, kmsDecryptDataRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KMSApi#kmsDecryptData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KMSApi#kmsDecryptData")
    e.printStackTrace()
}
```

### Parameters
| **keyId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsDecryptDataRequest** | [**KmsDecryptDataRequest**](KmsDecryptDataRequest.md)|  | |

### Return type

[**KmsDecryptDataResponse**](KmsDecryptDataResponse.md)

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

<a id="kmsDeleteKmsKey"></a>
# **kmsDeleteKmsKey**
> kotlin.Any kmsDeleteKmsKey(keyId)

Delete a KMS key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KMSApi()
val keyId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kmsDeleteKmsKey(keyId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KMSApi#kmsDeleteKmsKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KMSApi#kmsDeleteKmsKey")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **keyId** | **java.util.UUID**|  | |

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

<a id="kmsEncryptData"></a>
# **kmsEncryptData**
> KmsEncryptDataResponse kmsEncryptData(keyId, kmsEncryptDataRequest)

Encrypt data with a KMS key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KMSApi()
val keyId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsEncryptDataRequest : KmsEncryptDataRequest =  // KmsEncryptDataRequest | 
try {
    val result : KmsEncryptDataResponse = apiInstance.kmsEncryptData(keyId, kmsEncryptDataRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KMSApi#kmsEncryptData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KMSApi#kmsEncryptData")
    e.printStackTrace()
}
```

### Parameters
| **keyId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsEncryptDataRequest** | [**KmsEncryptDataRequest**](KmsEncryptDataRequest.md)|  | |

### Return type

[**KmsEncryptDataResponse**](KmsEncryptDataResponse.md)

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

<a id="kmsListKmsKeys"></a>
# **kmsListKmsKeys**
> KmsListKmsKeys200Response kmsListKmsKeys(projectId)

List KMS encryption keys

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KMSApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsListKmsKeys200Response = apiInstance.kmsListKmsKeys(projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KMSApi#kmsListKmsKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KMSApi#kmsListKmsKeys")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **java.util.UUID**|  | |

### Return type

[**KmsListKmsKeys200Response**](KmsListKmsKeys200Response.md)

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

<a id="kmsUpdateKmsKey"></a>
# **kmsUpdateKmsKey**
> KmsCreateKmsKey200Response kmsUpdateKmsKey(keyId, kmsUpdateKmsKeyRequest)

Update a KMS key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = KMSApi()
val keyId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsUpdateKmsKeyRequest : KmsUpdateKmsKeyRequest =  // KmsUpdateKmsKeyRequest | 
try {
    val result : KmsCreateKmsKey200Response = apiInstance.kmsUpdateKmsKey(keyId, kmsUpdateKmsKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KMSApi#kmsUpdateKmsKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KMSApi#kmsUpdateKmsKey")
    e.printStackTrace()
}
```

### Parameters
| **keyId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUpdateKmsKeyRequest** | [**KmsUpdateKmsKeyRequest**](KmsUpdateKmsKeyRequest.md)|  | |

### Return type

[**KmsCreateKmsKey200Response**](KmsCreateKmsKey200Response.md)

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

