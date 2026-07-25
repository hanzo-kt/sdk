# FileAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerActivateFile**](FileAPIApi.md#cloudApiControllerActivateFile) | **POST** /v1/cloud/activate-file | Api Controller Activate File |
| [**cloudApiControllerAddFile**](FileAPIApi.md#cloudApiControllerAddFile) | **POST** /v1/cloud/add-file | Api Controller Add File |
| [**cloudApiControllerDeleteFile**](FileAPIApi.md#cloudApiControllerDeleteFile) | **POST** /v1/cloud/delete-file | Api Controller Delete File |
| [**cloudApiControllerGetActiveFile**](FileAPIApi.md#cloudApiControllerGetActiveFile) | **GET** /v1/cloud/get-active-file | Api Controller Get Active File |
| [**cloudApiControllerUpdateFile**](FileAPIApi.md#cloudApiControllerUpdateFile) | **POST** /v1/cloud/update-file | Api Controller Update File |
| [**cloudApiControllerUploadFile**](FileAPIApi.md#cloudApiControllerUploadFile) | **POST** /v1/cloud/upload-file | Api Controller Upload File |
| [**nexusActivateFile**](FileAPIApi.md#nexusActivateFile) | **POST** /v1/nexus/activate-file | activate File |
| [**nexusAddFile**](FileAPIApi.md#nexusAddFile) | **POST** /v1/nexus/add-file | add File |
| [**nexusDeleteFile**](FileAPIApi.md#nexusDeleteFile) | **POST** /v1/nexus/delete-file | delete File |
| [**nexusGetActiveFile**](FileAPIApi.md#nexusGetActiveFile) | **GET** /v1/nexus/get-active-file | get Active File |
| [**nexusUpdateFile**](FileAPIApi.md#nexusUpdateFile) | **POST** /v1/nexus/update-file | update File |
| [**nexusUploadFile**](FileAPIApi.md#nexusUploadFile) | **POST** /v1/nexus/upload-file | upload File |


<a id="cloudApiControllerActivateFile"></a>
# **cloudApiControllerActivateFile**
> CloudControllersResponse cloudApiControllerActivateFile(key, filename)

Api Controller Activate File

activate file

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FileAPIApi()
val key : kotlin.String = key_example // kotlin.String | The key of the file
val filename : kotlin.String = filename_example // kotlin.String | The name of the file
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerActivateFile(key, filename)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FileAPIApi#cloudApiControllerActivateFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FileAPIApi#cloudApiControllerActivateFile")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**| The key of the file | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **filename** | **kotlin.String**| The name of the file | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerAddFile"></a>
# **cloudApiControllerAddFile**
> CloudControllersResponse cloudApiControllerAddFile(store, key, isLeaf, filename)

Api Controller Add File

add file

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FileAPIApi()
val store : kotlin.String = store_example // kotlin.String | The store of the file
val key : kotlin.String = key_example // kotlin.String | The key of the file
val isLeaf : kotlin.String = isLeaf_example // kotlin.String | if is leaf
val filename : kotlin.String = filename_example // kotlin.String | The name of the file
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddFile(store, key, isLeaf, filename)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FileAPIApi#cloudApiControllerAddFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FileAPIApi#cloudApiControllerAddFile")
    e.printStackTrace()
}
```

### Parameters
| **store** | **kotlin.String**| The store of the file | |
| **key** | **kotlin.String**| The key of the file | |
| **isLeaf** | **kotlin.String**| if is leaf | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **filename** | **kotlin.String**| The name of the file | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerDeleteFile"></a>
# **cloudApiControllerDeleteFile**
> CloudControllersResponse cloudApiControllerDeleteFile(store, key, isLeaf)

Api Controller Delete File

delete file

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FileAPIApi()
val store : kotlin.String = store_example // kotlin.String | The store of the file
val key : kotlin.String = key_example // kotlin.String | The key of the file
val isLeaf : kotlin.String = isLeaf_example // kotlin.String | if is leaf
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteFile(store, key, isLeaf)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FileAPIApi#cloudApiControllerDeleteFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FileAPIApi#cloudApiControllerDeleteFile")
    e.printStackTrace()
}
```

### Parameters
| **store** | **kotlin.String**| The store of the file | |
| **key** | **kotlin.String**| The key of the file | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **isLeaf** | **kotlin.String**| if is leaf | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerGetActiveFile"></a>
# **cloudApiControllerGetActiveFile**
> kotlin.Any cloudApiControllerGetActiveFile(prefix)

Api Controller Get Active File

get active file

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FileAPIApi()
val prefix : kotlin.String = prefix_example // kotlin.String | The prefix of the file
try {
    val result : kotlin.Any = apiInstance.cloudApiControllerGetActiveFile(prefix)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FileAPIApi#cloudApiControllerGetActiveFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FileAPIApi#cloudApiControllerGetActiveFile")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **prefix** | **kotlin.String**| The prefix of the file | |

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

<a id="cloudApiControllerUpdateFile"></a>
# **cloudApiControllerUpdateFile**
> CloudControllersResponse cloudApiControllerUpdateFile(storeId, key, cloudObjectFile)

Api Controller Update File

update file

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FileAPIApi()
val storeId : kotlin.String = storeId_example // kotlin.String | The store id of the file
val key : kotlin.String = key_example // kotlin.String | The key of the file
val cloudObjectFile : CloudObjectFile =  // CloudObjectFile | The details of the File
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateFile(storeId, key, cloudObjectFile)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FileAPIApi#cloudApiControllerUpdateFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FileAPIApi#cloudApiControllerUpdateFile")
    e.printStackTrace()
}
```

### Parameters
| **storeId** | **kotlin.String**| The store id of the file | |
| **key** | **kotlin.String**| The key of the file | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectFile** | [**CloudObjectFile**](CloudObjectFile.md)| The details of the File | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerUploadFile"></a>
# **cloudApiControllerUploadFile**
> CloudControllersResponse cloudApiControllerUploadFile(file, type, name)

Api Controller Upload File

upload file to IAM storage

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FileAPIApi()
val file : kotlin.String = file_example // kotlin.String | The base64 encoded file data
val type : kotlin.String = type_example // kotlin.String | The file type/extension
val name : kotlin.String = name_example // kotlin.String | The file name
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUploadFile(file, type, name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FileAPIApi#cloudApiControllerUploadFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FileAPIApi#cloudApiControllerUploadFile")
    e.printStackTrace()
}
```

### Parameters
| **file** | **kotlin.String**| The base64 encoded file data | |
| **type** | **kotlin.String**| The file type/extension | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| The file name | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

<a id="nexusActivateFile"></a>
# **nexusActivateFile**
> NexusResponse nexusActivateFile(key, filename)

activate File

Activate a file for processing

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FileAPIApi()
val key : kotlin.String = key_example // kotlin.String | The key of the file
val filename : kotlin.String = filename_example // kotlin.String | The name of the file
try {
    val result : NexusResponse = apiInstance.nexusActivateFile(key, filename)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FileAPIApi#nexusActivateFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FileAPIApi#nexusActivateFile")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**| The key of the file | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **filename** | **kotlin.String**| The name of the file | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusAddFile"></a>
# **nexusAddFile**
> NexusResponse nexusAddFile(store, key, isLeaf, filename)

add File

Add a file to a knowledge store

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FileAPIApi()
val store : kotlin.String = store_example // kotlin.String | The store of the file
val key : kotlin.String = key_example // kotlin.String | The key of the file
val isLeaf : kotlin.String = isLeaf_example // kotlin.String | Whether the file is a leaf node
val filename : kotlin.String = filename_example // kotlin.String | The name of the file
try {
    val result : NexusResponse = apiInstance.nexusAddFile(store, key, isLeaf, filename)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FileAPIApi#nexusAddFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FileAPIApi#nexusAddFile")
    e.printStackTrace()
}
```

### Parameters
| **store** | **kotlin.String**| The store of the file | |
| **key** | **kotlin.String**| The key of the file | |
| **isLeaf** | **kotlin.String**| Whether the file is a leaf node | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **filename** | **kotlin.String**| The name of the file | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusDeleteFile"></a>
# **nexusDeleteFile**
> NexusResponse nexusDeleteFile(store, key, isLeaf)

delete File

Delete a file

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FileAPIApi()
val store : kotlin.String = store_example // kotlin.String | The store of the file
val key : kotlin.String = key_example // kotlin.String | The key of the file
val isLeaf : kotlin.String = isLeaf_example // kotlin.String | Whether the file is a leaf node
try {
    val result : NexusResponse = apiInstance.nexusDeleteFile(store, key, isLeaf)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FileAPIApi#nexusDeleteFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FileAPIApi#nexusDeleteFile")
    e.printStackTrace()
}
```

### Parameters
| **store** | **kotlin.String**| The store of the file | |
| **key** | **kotlin.String**| The key of the file | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **isLeaf** | **kotlin.String**| Whether the file is a leaf node | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusGetActiveFile"></a>
# **nexusGetActiveFile**
> kotlin.String nexusGetActiveFile(prefix)

get Active File

Get the active file

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FileAPIApi()
val prefix : kotlin.String = prefix_example // kotlin.String | The prefix of the file
try {
    val result : kotlin.String = apiInstance.nexusGetActiveFile(prefix)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FileAPIApi#nexusGetActiveFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FileAPIApi#nexusGetActiveFile")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **prefix** | **kotlin.String**| The prefix of the file | |

### Return type

**kotlin.String**

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

<a id="nexusUpdateFile"></a>
# **nexusUpdateFile**
> NexusResponse nexusUpdateFile(storeId, key, nexusFile)

update File

Update a file

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FileAPIApi()
val storeId : kotlin.String = storeId_example // kotlin.String | The store id of the file
val key : kotlin.String = key_example // kotlin.String | The key of the file
val nexusFile : NexusFile =  // NexusFile | The details of the file
try {
    val result : NexusResponse = apiInstance.nexusUpdateFile(storeId, key, nexusFile)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FileAPIApi#nexusUpdateFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FileAPIApi#nexusUpdateFile")
    e.printStackTrace()
}
```

### Parameters
| **storeId** | **kotlin.String**| The store id of the file | |
| **key** | **kotlin.String**| The key of the file | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusFile** | [**NexusFile**](NexusFile.md)| The details of the file | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusUploadFile"></a>
# **nexusUploadFile**
> NexusResponse nexusUploadFile(file, type, name)

upload File

Upload a file to storage

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FileAPIApi()
val file : kotlin.String = file_example // kotlin.String | The base64 encoded file data
val type : kotlin.String = type_example // kotlin.String | The file type/extension
val name : kotlin.String = name_example // kotlin.String | The file name
try {
    val result : NexusResponse = apiInstance.nexusUploadFile(file, type, name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FileAPIApi#nexusUploadFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FileAPIApi#nexusUploadFile")
    e.printStackTrace()
}
```

### Parameters
| **file** | **kotlin.String**| The base64 encoded file data | |
| **type** | **kotlin.String**| The file type/extension | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| The file name | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

