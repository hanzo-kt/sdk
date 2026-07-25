# SecretSyncsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsCreateSecretSync**](SecretSyncsApi.md#kmsCreateSecretSync) | **POST** /v1/kms/secret-syncs | Create a secret sync |
| [**kmsDeleteSecretSync**](SecretSyncsApi.md#kmsDeleteSecretSync) | **DELETE** /v1/kms/secret-syncs/{syncId} | Delete a secret sync |
| [**kmsGetSecretSync**](SecretSyncsApi.md#kmsGetSecretSync) | **GET** /v1/kms/secret-syncs/{syncId} | Get a secret sync by ID |
| [**kmsListSecretSyncs**](SecretSyncsApi.md#kmsListSecretSyncs) | **GET** /v1/kms/secret-syncs | List secret syncs |
| [**kmsTriggerSecretSync**](SecretSyncsApi.md#kmsTriggerSecretSync) | **POST** /v1/kms/secret-syncs/{syncId}/trigger | Manually trigger a secret sync |
| [**kmsUpdateSecretSync**](SecretSyncsApi.md#kmsUpdateSecretSync) | **PATCH** /v1/kms/secret-syncs/{syncId} | Update a secret sync |


<a id="kmsCreateSecretSync"></a>
# **kmsCreateSecretSync**
> KmsCreateSecretSync200Response kmsCreateSecretSync(kmsCreateSecretSyncRequest)

Create a secret sync

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretSyncsApi()
val kmsCreateSecretSyncRequest : KmsCreateSecretSyncRequest =  // KmsCreateSecretSyncRequest | 
try {
    val result : KmsCreateSecretSync200Response = apiInstance.kmsCreateSecretSync(kmsCreateSecretSyncRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretSyncsApi#kmsCreateSecretSync")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretSyncsApi#kmsCreateSecretSync")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateSecretSyncRequest** | [**KmsCreateSecretSyncRequest**](KmsCreateSecretSyncRequest.md)|  | |

### Return type

[**KmsCreateSecretSync200Response**](KmsCreateSecretSync200Response.md)

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

<a id="kmsDeleteSecretSync"></a>
# **kmsDeleteSecretSync**
> kotlin.Any kmsDeleteSecretSync(syncId)

Delete a secret sync

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretSyncsApi()
val syncId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kmsDeleteSecretSync(syncId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretSyncsApi#kmsDeleteSecretSync")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretSyncsApi#kmsDeleteSecretSync")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **syncId** | **java.util.UUID**|  | |

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

<a id="kmsGetSecretSync"></a>
# **kmsGetSecretSync**
> KmsCreateSecretSync200Response kmsGetSecretSync(syncId)

Get a secret sync by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretSyncsApi()
val syncId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsCreateSecretSync200Response = apiInstance.kmsGetSecretSync(syncId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretSyncsApi#kmsGetSecretSync")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretSyncsApi#kmsGetSecretSync")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **syncId** | **java.util.UUID**|  | |

### Return type

[**KmsCreateSecretSync200Response**](KmsCreateSecretSync200Response.md)

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

<a id="kmsListSecretSyncs"></a>
# **kmsListSecretSyncs**
> KmsListSecretSyncs200Response kmsListSecretSyncs(projectId)

List secret syncs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretSyncsApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsListSecretSyncs200Response = apiInstance.kmsListSecretSyncs(projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretSyncsApi#kmsListSecretSyncs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretSyncsApi#kmsListSecretSyncs")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **java.util.UUID**|  | |

### Return type

[**KmsListSecretSyncs200Response**](KmsListSecretSyncs200Response.md)

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

<a id="kmsTriggerSecretSync"></a>
# **kmsTriggerSecretSync**
> kotlin.Any kmsTriggerSecretSync(syncId)

Manually trigger a secret sync

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretSyncsApi()
val syncId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kmsTriggerSecretSync(syncId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretSyncsApi#kmsTriggerSecretSync")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretSyncsApi#kmsTriggerSecretSync")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **syncId** | **java.util.UUID**|  | |

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

<a id="kmsUpdateSecretSync"></a>
# **kmsUpdateSecretSync**
> KmsCreateSecretSync200Response kmsUpdateSecretSync(syncId, kmsUpdateSecretSyncRequest)

Update a secret sync

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretSyncsApi()
val syncId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsUpdateSecretSyncRequest : KmsUpdateSecretSyncRequest =  // KmsUpdateSecretSyncRequest | 
try {
    val result : KmsCreateSecretSync200Response = apiInstance.kmsUpdateSecretSync(syncId, kmsUpdateSecretSyncRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretSyncsApi#kmsUpdateSecretSync")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretSyncsApi#kmsUpdateSecretSync")
    e.printStackTrace()
}
```

### Parameters
| **syncId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUpdateSecretSyncRequest** | [**KmsUpdateSecretSyncRequest**](KmsUpdateSecretSyncRequest.md)|  | |

### Return type

[**KmsCreateSecretSync200Response**](KmsCreateSecretSync200Response.md)

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

