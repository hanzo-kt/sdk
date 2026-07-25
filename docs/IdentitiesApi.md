# IdentitiesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsCreateIdentity**](IdentitiesApi.md#kmsCreateIdentity) | **POST** /v1/kms/identities | Create a machine identity |
| [**kmsDeleteIdentity**](IdentitiesApi.md#kmsDeleteIdentity) | **DELETE** /v1/kms/identities/{identityId} | Delete an identity |
| [**kmsGetIdentity**](IdentitiesApi.md#kmsGetIdentity) | **GET** /v1/kms/identities/{identityId} | Get an identity by ID |
| [**kmsUpdateIdentity**](IdentitiesApi.md#kmsUpdateIdentity) | **PATCH** /v1/kms/identities/{identityId} | Update an identity |


<a id="kmsCreateIdentity"></a>
# **kmsCreateIdentity**
> KmsCreateIdentity200Response kmsCreateIdentity(kmsCreateIdentityRequest)

Create a machine identity

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentitiesApi()
val kmsCreateIdentityRequest : KmsCreateIdentityRequest =  // KmsCreateIdentityRequest | 
try {
    val result : KmsCreateIdentity200Response = apiInstance.kmsCreateIdentity(kmsCreateIdentityRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentitiesApi#kmsCreateIdentity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentitiesApi#kmsCreateIdentity")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateIdentityRequest** | [**KmsCreateIdentityRequest**](KmsCreateIdentityRequest.md)|  | |

### Return type

[**KmsCreateIdentity200Response**](KmsCreateIdentity200Response.md)

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

<a id="kmsDeleteIdentity"></a>
# **kmsDeleteIdentity**
> kotlin.Any kmsDeleteIdentity(identityId)

Delete an identity

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentitiesApi()
val identityId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kmsDeleteIdentity(identityId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentitiesApi#kmsDeleteIdentity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentitiesApi#kmsDeleteIdentity")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **identityId** | **java.util.UUID**|  | |

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

<a id="kmsGetIdentity"></a>
# **kmsGetIdentity**
> KmsCreateIdentity200Response kmsGetIdentity(identityId)

Get an identity by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentitiesApi()
val identityId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsCreateIdentity200Response = apiInstance.kmsGetIdentity(identityId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentitiesApi#kmsGetIdentity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentitiesApi#kmsGetIdentity")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **identityId** | **java.util.UUID**|  | |

### Return type

[**KmsCreateIdentity200Response**](KmsCreateIdentity200Response.md)

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

<a id="kmsUpdateIdentity"></a>
# **kmsUpdateIdentity**
> KmsCreateIdentity200Response kmsUpdateIdentity(identityId, kmsUpdateIdentityRequest)

Update an identity

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentitiesApi()
val identityId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsUpdateIdentityRequest : KmsUpdateIdentityRequest =  // KmsUpdateIdentityRequest | 
try {
    val result : KmsCreateIdentity200Response = apiInstance.kmsUpdateIdentity(identityId, kmsUpdateIdentityRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentitiesApi#kmsUpdateIdentity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentitiesApi#kmsUpdateIdentity")
    e.printStackTrace()
}
```

### Parameters
| **identityId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUpdateIdentityRequest** | [**KmsUpdateIdentityRequest**](KmsUpdateIdentityRequest.md)|  | |

### Return type

[**KmsCreateIdentity200Response**](KmsCreateIdentity200Response.md)

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

