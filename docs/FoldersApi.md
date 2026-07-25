# FoldersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoCreateFolder**](FoldersApi.md#autoCreateFolder) | **POST** /v1/auto/folders | Create a folder |
| [**autoDeleteFolder**](FoldersApi.md#autoDeleteFolder) | **DELETE** /v1/auto/folders/{id} | Delete a folder |
| [**autoGetFolder**](FoldersApi.md#autoGetFolder) | **GET** /v1/auto/folders/{id} | Get a folder by id |
| [**autoListFolders**](FoldersApi.md#autoListFolders) | **GET** /v1/auto/folders | List folders |
| [**autoUpdateFolder**](FoldersApi.md#autoUpdateFolder) | **POST** /v1/auto/folders/{id} | Update a folder |
| [**flowCreateFolder**](FoldersApi.md#flowCreateFolder) | **POST** /v1/flow/folders | Create a folder |
| [**flowDeleteFolder**](FoldersApi.md#flowDeleteFolder) | **DELETE** /v1/flow/folders/{id} | Delete a folder |
| [**flowGetFolder**](FoldersApi.md#flowGetFolder) | **GET** /v1/flow/folders/{id} | Get a folder by id |
| [**flowListFolders**](FoldersApi.md#flowListFolders) | **GET** /v1/flow/folders | List folders |
| [**flowUpdateFolder**](FoldersApi.md#flowUpdateFolder) | **POST** /v1/flow/folders/{id} | Update a folder |


<a id="autoCreateFolder"></a>
# **autoCreateFolder**
> kotlin.Any autoCreateFolder(autoCreateApiKeyRequest)

Create a folder

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FoldersApi()
val autoCreateApiKeyRequest : AutoCreateApiKeyRequest =  // AutoCreateApiKeyRequest | 
try {
    val result : kotlin.Any = apiInstance.autoCreateFolder(autoCreateApiKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#autoCreateFolder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#autoCreateFolder")
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

<a id="autoDeleteFolder"></a>
# **autoDeleteFolder**
> autoDeleteFolder(id)

Delete a folder

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.autoDeleteFolder(id)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#autoDeleteFolder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#autoDeleteFolder")
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

<a id="autoGetFolder"></a>
# **autoGetFolder**
> kotlin.Any autoGetFolder(id)

Get a folder by id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoGetFolder(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#autoGetFolder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#autoGetFolder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="autoListFolders"></a>
# **autoListFolders**
> kotlin.Any autoListFolders()

List folders

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FoldersApi()
try {
    val result : kotlin.Any = apiInstance.autoListFolders()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#autoListFolders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#autoListFolders")
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

<a id="autoUpdateFolder"></a>
# **autoUpdateFolder**
> kotlin.Any autoUpdateFolder(id, autoUpdateAppConnectionRequest)

Update a folder

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | 
val autoUpdateAppConnectionRequest : AutoUpdateAppConnectionRequest =  // AutoUpdateAppConnectionRequest | 
try {
    val result : kotlin.Any = apiInstance.autoUpdateFolder(id, autoUpdateAppConnectionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#autoUpdateFolder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#autoUpdateFolder")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoUpdateAppConnectionRequest** | [**AutoUpdateAppConnectionRequest**](AutoUpdateAppConnectionRequest.md)|  | |

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

<a id="flowCreateFolder"></a>
# **flowCreateFolder**
> FlowFolder flowCreateFolder(autoCreateApiKeyRequest)

Create a folder

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FoldersApi()
val autoCreateApiKeyRequest : AutoCreateApiKeyRequest =  // AutoCreateApiKeyRequest | 
try {
    val result : FlowFolder = apiInstance.flowCreateFolder(autoCreateApiKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#flowCreateFolder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#flowCreateFolder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateApiKeyRequest** | [**AutoCreateApiKeyRequest**](AutoCreateApiKeyRequest.md)|  | |

### Return type

[**FlowFolder**](FlowFolder.md)

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

<a id="flowDeleteFolder"></a>
# **flowDeleteFolder**
> flowDeleteFolder(id)

Delete a folder

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.flowDeleteFolder(id)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#flowDeleteFolder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#flowDeleteFolder")
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

<a id="flowGetFolder"></a>
# **flowGetFolder**
> kotlin.Any flowGetFolder(id)

Get a folder by id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowGetFolder(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#flowGetFolder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#flowGetFolder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="flowListFolders"></a>
# **flowListFolders**
> kotlin.collections.List&lt;FlowFolder&gt; flowListFolders()

List folders

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FoldersApi()
try {
    val result : kotlin.collections.List<FlowFolder> = apiInstance.flowListFolders()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#flowListFolders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#flowListFolders")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;FlowFolder&gt;**](FlowFolder.md)

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

<a id="flowUpdateFolder"></a>
# **flowUpdateFolder**
> kotlin.Any flowUpdateFolder(id, autoUpdateAppConnectionRequest)

Update a folder

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FoldersApi()
val id : kotlin.String = id_example // kotlin.String | 
val autoUpdateAppConnectionRequest : AutoUpdateAppConnectionRequest =  // AutoUpdateAppConnectionRequest | 
try {
    val result : kotlin.Any = apiInstance.flowUpdateFolder(id, autoUpdateAppConnectionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FoldersApi#flowUpdateFolder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FoldersApi#flowUpdateFolder")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoUpdateAppConnectionRequest** | [**AutoUpdateAppConnectionRequest**](AutoUpdateAppConnectionRequest.md)|  | |

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

