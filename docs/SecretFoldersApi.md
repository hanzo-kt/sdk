# SecretFoldersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kmsCreateSecretFolder**](SecretFoldersApi.md#kmsCreateSecretFolder) | **POST** /v1/kms/folders | Create a secret folder |
| [**kmsDeleteSecretFolder**](SecretFoldersApi.md#kmsDeleteSecretFolder) | **DELETE** /v1/kms/folders/{folderId} | Delete a secret folder |
| [**kmsListSecretFolders**](SecretFoldersApi.md#kmsListSecretFolders) | **GET** /v1/kms/folders | List secret folders |
| [**kmsUpdateSecretFolder**](SecretFoldersApi.md#kmsUpdateSecretFolder) | **PATCH** /v1/kms/folders/{folderId} | Update a secret folder |


<a id="kmsCreateSecretFolder"></a>
# **kmsCreateSecretFolder**
> KmsCreateSecretFolder200Response kmsCreateSecretFolder(kmsCreateSecretFolderRequest)

Create a secret folder

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretFoldersApi()
val kmsCreateSecretFolderRequest : KmsCreateSecretFolderRequest =  // KmsCreateSecretFolderRequest | 
try {
    val result : KmsCreateSecretFolder200Response = apiInstance.kmsCreateSecretFolder(kmsCreateSecretFolderRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretFoldersApi#kmsCreateSecretFolder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretFoldersApi#kmsCreateSecretFolder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateSecretFolderRequest** | [**KmsCreateSecretFolderRequest**](KmsCreateSecretFolderRequest.md)|  | |

### Return type

[**KmsCreateSecretFolder200Response**](KmsCreateSecretFolder200Response.md)

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

<a id="kmsDeleteSecretFolder"></a>
# **kmsDeleteSecretFolder**
> kotlin.Any kmsDeleteSecretFolder(folderId, kmsDeleteSecretFolderRequest)

Delete a secret folder

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretFoldersApi()
val folderId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsDeleteSecretFolderRequest : KmsDeleteSecretFolderRequest =  // KmsDeleteSecretFolderRequest | 
try {
    val result : kotlin.Any = apiInstance.kmsDeleteSecretFolder(folderId, kmsDeleteSecretFolderRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretFoldersApi#kmsDeleteSecretFolder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretFoldersApi#kmsDeleteSecretFolder")
    e.printStackTrace()
}
```

### Parameters
| **folderId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsDeleteSecretFolderRequest** | [**KmsDeleteSecretFolderRequest**](KmsDeleteSecretFolderRequest.md)|  | |

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

<a id="kmsListSecretFolders"></a>
# **kmsListSecretFolders**
> KmsListSecretFolders200Response kmsListSecretFolders(workspaceId, environment, directory)

List secret folders

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretFoldersApi()
val workspaceId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val environment : kotlin.String = environment_example // kotlin.String | 
val directory : kotlin.String = directory_example // kotlin.String | 
try {
    val result : KmsListSecretFolders200Response = apiInstance.kmsListSecretFolders(workspaceId, environment, directory)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretFoldersApi#kmsListSecretFolders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretFoldersApi#kmsListSecretFolders")
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

[**KmsListSecretFolders200Response**](KmsListSecretFolders200Response.md)

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

<a id="kmsUpdateSecretFolder"></a>
# **kmsUpdateSecretFolder**
> KmsCreateSecretFolder200Response kmsUpdateSecretFolder(folderId, kmsUpdateSecretFolderRequest)

Update a secret folder

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SecretFoldersApi()
val folderId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsUpdateSecretFolderRequest : KmsUpdateSecretFolderRequest =  // KmsUpdateSecretFolderRequest | 
try {
    val result : KmsCreateSecretFolder200Response = apiInstance.kmsUpdateSecretFolder(folderId, kmsUpdateSecretFolderRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SecretFoldersApi#kmsUpdateSecretFolder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SecretFoldersApi#kmsUpdateSecretFolder")
    e.printStackTrace()
}
```

### Parameters
| **folderId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUpdateSecretFolderRequest** | [**KmsUpdateSecretFolderRequest**](KmsUpdateSecretFolderRequest.md)|  | |

### Return type

[**KmsCreateSecretFolder200Response**](KmsCreateSecretFolder200Response.md)

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

