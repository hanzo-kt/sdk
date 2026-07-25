# SnapshotsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchCreateSnapshot**](SnapshotsApi.md#searchCreateSnapshot) | **POST** /v1/search/snapshots | Create a database snapshot |
| [**vectorCreateSnapshot**](SnapshotsApi.md#vectorCreateSnapshot) | **POST** /v1/vector/collections/{collection_name}/snapshots | Create snapshot |
| [**vectorDeleteSnapshot**](SnapshotsApi.md#vectorDeleteSnapshot) | **DELETE** /v1/vector/collections/{collection_name}/snapshots/{snapshot_name} | Delete snapshot |
| [**vectorDownloadSnapshot**](SnapshotsApi.md#vectorDownloadSnapshot) | **GET** /v1/vector/collections/{collection_name}/snapshots/{snapshot_name} | Download snapshot |
| [**vectorListSnapshots**](SnapshotsApi.md#vectorListSnapshots) | **GET** /v1/vector/collections/{collection_name}/snapshots | List snapshots |


<a id="searchCreateSnapshot"></a>
# **searchCreateSnapshot**
> SearchSummarizedTaskView searchCreateSnapshot()

Create a database snapshot

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SnapshotsApi()
try {
    val result : SearchSummarizedTaskView = apiInstance.searchCreateSnapshot()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SnapshotsApi#searchCreateSnapshot")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SnapshotsApi#searchCreateSnapshot")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**SearchSummarizedTaskView**](SearchSummarizedTaskView.md)

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

<a id="vectorCreateSnapshot"></a>
# **vectorCreateSnapshot**
> VectorCreateSnapshot200Response vectorCreateSnapshot(collectionName)

Create snapshot

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SnapshotsApi()
val collectionName : kotlin.String = collectionName_example // kotlin.String | 
try {
    val result : VectorCreateSnapshot200Response = apiInstance.vectorCreateSnapshot(collectionName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SnapshotsApi#vectorCreateSnapshot")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SnapshotsApi#vectorCreateSnapshot")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **collectionName** | **kotlin.String**|  | |

### Return type

[**VectorCreateSnapshot200Response**](VectorCreateSnapshot200Response.md)

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

<a id="vectorDeleteSnapshot"></a>
# **vectorDeleteSnapshot**
> VectorCreateCollection200Response vectorDeleteSnapshot(collectionName, snapshotName)

Delete snapshot

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SnapshotsApi()
val collectionName : kotlin.String = collectionName_example // kotlin.String | 
val snapshotName : kotlin.String = snapshotName_example // kotlin.String | 
try {
    val result : VectorCreateCollection200Response = apiInstance.vectorDeleteSnapshot(collectionName, snapshotName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SnapshotsApi#vectorDeleteSnapshot")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SnapshotsApi#vectorDeleteSnapshot")
    e.printStackTrace()
}
```

### Parameters
| **collectionName** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **snapshotName** | **kotlin.String**|  | |

### Return type

[**VectorCreateCollection200Response**](VectorCreateCollection200Response.md)

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

<a id="vectorDownloadSnapshot"></a>
# **vectorDownloadSnapshot**
> java.io.File vectorDownloadSnapshot(collectionName, snapshotName)

Download snapshot

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SnapshotsApi()
val collectionName : kotlin.String = collectionName_example // kotlin.String | 
val snapshotName : kotlin.String = snapshotName_example // kotlin.String | 
try {
    val result : java.io.File = apiInstance.vectorDownloadSnapshot(collectionName, snapshotName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SnapshotsApi#vectorDownloadSnapshot")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SnapshotsApi#vectorDownloadSnapshot")
    e.printStackTrace()
}
```

### Parameters
| **collectionName** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **snapshotName** | **kotlin.String**|  | |

### Return type

[**java.io.File**](java.io.File.md)

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
 - **Accept**: application/octet-stream

<a id="vectorListSnapshots"></a>
# **vectorListSnapshots**
> VectorListSnapshots200Response vectorListSnapshots(collectionName)

List snapshots

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SnapshotsApi()
val collectionName : kotlin.String = collectionName_example // kotlin.String | 
try {
    val result : VectorListSnapshots200Response = apiInstance.vectorListSnapshots(collectionName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SnapshotsApi#vectorListSnapshots")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SnapshotsApi#vectorListSnapshots")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **collectionName** | **kotlin.String**|  | |

### Return type

[**VectorListSnapshots200Response**](VectorListSnapshots200Response.md)

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

