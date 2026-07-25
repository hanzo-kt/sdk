# IdentityAuthApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsAttachUniversalAuth**](IdentityAuthApi.md#kmsAttachUniversalAuth) | **POST** /v1/kms/auth/universal-auth/identities/{identityId} | Attach Universal Auth to an identity |
| [**kmsCreateIdentityToken**](IdentityAuthApi.md#kmsCreateIdentityToken) | **POST** /v1/kms/auth/token-auth/identities/{identityId}/tokens | Create an identity token |
| [**kmsCreateUniversalAuthClientSecret**](IdentityAuthApi.md#kmsCreateUniversalAuthClientSecret) | **POST** /v1/kms/auth/universal-auth/identities/{identityId}/client-secrets | Create a client secret for Universal Auth |
| [**kmsGetUniversalAuth**](IdentityAuthApi.md#kmsGetUniversalAuth) | **GET** /v1/kms/auth/universal-auth/identities/{identityId} | Get Universal Auth configuration for an identity |
| [**kmsUniversalAuthLogin**](IdentityAuthApi.md#kmsUniversalAuthLogin) | **POST** /v1/kms/auth/universal-auth/login | Login with Universal Auth |


<a id="kmsAttachUniversalAuth"></a>
# **kmsAttachUniversalAuth**
> KmsUniversalAuthConfig kmsAttachUniversalAuth(identityId, kmsAttachUniversalAuthRequest)

Attach Universal Auth to an identity

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentityAuthApi()
val identityId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsAttachUniversalAuthRequest : KmsAttachUniversalAuthRequest =  // KmsAttachUniversalAuthRequest | 
try {
    val result : KmsUniversalAuthConfig = apiInstance.kmsAttachUniversalAuth(identityId, kmsAttachUniversalAuthRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentityAuthApi#kmsAttachUniversalAuth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentityAuthApi#kmsAttachUniversalAuth")
    e.printStackTrace()
}
```

### Parameters
| **identityId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsAttachUniversalAuthRequest** | [**KmsAttachUniversalAuthRequest**](KmsAttachUniversalAuthRequest.md)|  | |

### Return type

[**KmsUniversalAuthConfig**](KmsUniversalAuthConfig.md)

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

<a id="kmsCreateIdentityToken"></a>
# **kmsCreateIdentityToken**
> KmsTokenResponse kmsCreateIdentityToken(identityId)

Create an identity token

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentityAuthApi()
val identityId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsTokenResponse = apiInstance.kmsCreateIdentityToken(identityId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentityAuthApi#kmsCreateIdentityToken")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentityAuthApi#kmsCreateIdentityToken")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **identityId** | **java.util.UUID**|  | |

### Return type

[**KmsTokenResponse**](KmsTokenResponse.md)

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

<a id="kmsCreateUniversalAuthClientSecret"></a>
# **kmsCreateUniversalAuthClientSecret**
> KmsCreateClientSecretResponse kmsCreateUniversalAuthClientSecret(identityId, kmsCreateUniversalAuthClientSecretRequest)

Create a client secret for Universal Auth

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentityAuthApi()
val identityId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsCreateUniversalAuthClientSecretRequest : KmsCreateUniversalAuthClientSecretRequest =  // KmsCreateUniversalAuthClientSecretRequest | 
try {
    val result : KmsCreateClientSecretResponse = apiInstance.kmsCreateUniversalAuthClientSecret(identityId, kmsCreateUniversalAuthClientSecretRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentityAuthApi#kmsCreateUniversalAuthClientSecret")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentityAuthApi#kmsCreateUniversalAuthClientSecret")
    e.printStackTrace()
}
```

### Parameters
| **identityId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateUniversalAuthClientSecretRequest** | [**KmsCreateUniversalAuthClientSecretRequest**](KmsCreateUniversalAuthClientSecretRequest.md)|  | |

### Return type

[**KmsCreateClientSecretResponse**](KmsCreateClientSecretResponse.md)

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

<a id="kmsGetUniversalAuth"></a>
# **kmsGetUniversalAuth**
> KmsUniversalAuthConfig kmsGetUniversalAuth(identityId)

Get Universal Auth configuration for an identity

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentityAuthApi()
val identityId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsUniversalAuthConfig = apiInstance.kmsGetUniversalAuth(identityId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentityAuthApi#kmsGetUniversalAuth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentityAuthApi#kmsGetUniversalAuth")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **identityId** | **java.util.UUID**|  | |

### Return type

[**KmsUniversalAuthConfig**](KmsUniversalAuthConfig.md)

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

<a id="kmsUniversalAuthLogin"></a>
# **kmsUniversalAuthLogin**
> KmsTokenResponse kmsUniversalAuthLogin(kmsUniversalAuthLoginRequest)

Login with Universal Auth

Exchange clientId and clientSecret for an access token.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IdentityAuthApi()
val kmsUniversalAuthLoginRequest : KmsUniversalAuthLoginRequest =  // KmsUniversalAuthLoginRequest | 
try {
    val result : KmsTokenResponse = apiInstance.kmsUniversalAuthLogin(kmsUniversalAuthLoginRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IdentityAuthApi#kmsUniversalAuthLogin")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IdentityAuthApi#kmsUniversalAuthLogin")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUniversalAuthLoginRequest** | [**KmsUniversalAuthLoginRequest**](KmsUniversalAuthLoginRequest.md)|  | |

### Return type

[**KmsTokenResponse**](KmsTokenResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

