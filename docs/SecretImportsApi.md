# SecretImportsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsCreateSecretImport**](SecretImportsApi.md#kmsCreateSecretImport) | **POST** /v1/kms/secret-imports | Create a secret import |
| [**kmsDeleteSecretImport**](SecretImportsApi.md#kmsDeleteSecretImport) | **DELETE** /v1/kms/secret-imports/{importId} | Delete a secret import |
| [**kmsListSecretImports**](SecretImportsApi.md#kmsListSecretImports) | **GET** /v1/kms/secret-imports | List secret imports |
| [**kmsUpdateSecretImport**](SecretImportsApi.md#kmsUpdateSecretImport) | **PATCH** /v1/kms/secret-imports/{importId} | Update a secret import |


<a id="kmsCreateSecretImport"></a>
# **kmsCreateSecretImport**
> KmsCreateSecretImport200Response kmsCreateSecretImport(kmsCreateSecretImportRequest)

Create a secret import

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretImportsApi()
val kmsCreateSecretImportRequest : KmsCreateSecretImportRequest =  // KmsCreateSecretImportRequest | 
try {
    val result : KmsCreateSecretImport200Response = apiInstance.kmsCreateSecretImport(kmsCreateSecretImportRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretImportsApi#kmsCreateSecretImport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretImportsApi#kmsCreateSecretImport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateSecretImportRequest** | [**KmsCreateSecretImportRequest**](KmsCreateSecretImportRequest.md)|  | |

### Return type

[**KmsCreateSecretImport200Response**](KmsCreateSecretImport200Response.md)

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

<a id="kmsDeleteSecretImport"></a>
# **kmsDeleteSecretImport**
> kotlin.Any kmsDeleteSecretImport(importId)

Delete a secret import

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretImportsApi()
val importId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kmsDeleteSecretImport(importId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretImportsApi#kmsDeleteSecretImport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretImportsApi#kmsDeleteSecretImport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **importId** | **java.util.UUID**|  | |

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

<a id="kmsListSecretImports"></a>
# **kmsListSecretImports**
> KmsListSecretImports200Response kmsListSecretImports(workspaceId, environment, directory)

List secret imports

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretImportsApi()
val workspaceId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val environment : kotlin.String = environment_example // kotlin.String | 
val directory : kotlin.String = directory_example // kotlin.String | 
try {
    val result : KmsListSecretImports200Response = apiInstance.kmsListSecretImports(workspaceId, environment, directory)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretImportsApi#kmsListSecretImports")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretImportsApi#kmsListSecretImports")
    e.printStackTrace()
}
```

### Parameters
| **workspaceId** | **java.util.UUID**|  | |
| **environment** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **directory** | **kotlin.String**|  | [optional] [default to &quot;/&quot;] |

### Return type

[**KmsListSecretImports200Response**](KmsListSecretImports200Response.md)

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

<a id="kmsUpdateSecretImport"></a>
# **kmsUpdateSecretImport**
> KmsCreateSecretImport200Response kmsUpdateSecretImport(importId, kmsUpdateSecretImportRequest)

Update a secret import

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretImportsApi()
val importId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsUpdateSecretImportRequest : KmsUpdateSecretImportRequest =  // KmsUpdateSecretImportRequest | 
try {
    val result : KmsCreateSecretImport200Response = apiInstance.kmsUpdateSecretImport(importId, kmsUpdateSecretImportRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretImportsApi#kmsUpdateSecretImport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretImportsApi#kmsUpdateSecretImport")
    e.printStackTrace()
}
```

### Parameters
| **importId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUpdateSecretImportRequest** | [**KmsUpdateSecretImportRequest**](KmsUpdateSecretImportRequest.md)|  | |

### Return type

[**KmsCreateSecretImport200Response**](KmsCreateSecretImport200Response.md)

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

