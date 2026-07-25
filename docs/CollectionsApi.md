# CollectionsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**vectorCreateCollection**](CollectionsApi.md#vectorCreateCollection) | **PUT** /v1/vector/collections/{collection_name} | Create collection |
| [**vectorDeleteCollection**](CollectionsApi.md#vectorDeleteCollection) | **DELETE** /v1/vector/collections/{collection_name} | Delete collection |
| [**vectorGetCollection**](CollectionsApi.md#vectorGetCollection) | **GET** /v1/vector/collections/{collection_name} | Get collection info |
| [**vectorListCollections**](CollectionsApi.md#vectorListCollections) | **GET** /v1/vector/collections | List collections |


<a id="vectorCreateCollection"></a>
# **vectorCreateCollection**
> VectorCreateCollection200Response vectorCreateCollection(collectionName, vectorCreateCollectionRequest)

Create collection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CollectionsApi()
val collectionName : kotlin.String = collectionName_example // kotlin.String | 
val vectorCreateCollectionRequest : VectorCreateCollectionRequest =  // VectorCreateCollectionRequest | 
try {
    val result : VectorCreateCollection200Response = apiInstance.vectorCreateCollection(collectionName, vectorCreateCollectionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectionsApi#vectorCreateCollection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectionsApi#vectorCreateCollection")
    e.printStackTrace()
}
```

### Parameters
| **collectionName** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **vectorCreateCollectionRequest** | [**VectorCreateCollectionRequest**](VectorCreateCollectionRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="vectorDeleteCollection"></a>
# **vectorDeleteCollection**
> VectorCreateCollection200Response vectorDeleteCollection(collectionName)

Delete collection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CollectionsApi()
val collectionName : kotlin.String = collectionName_example // kotlin.String | 
try {
    val result : VectorCreateCollection200Response = apiInstance.vectorDeleteCollection(collectionName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectionsApi#vectorDeleteCollection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectionsApi#vectorDeleteCollection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **collectionName** | **kotlin.String**|  | |

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

<a id="vectorGetCollection"></a>
# **vectorGetCollection**
> VectorGetCollection200Response vectorGetCollection(collectionName)

Get collection info

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CollectionsApi()
val collectionName : kotlin.String = collectionName_example // kotlin.String | 
try {
    val result : VectorGetCollection200Response = apiInstance.vectorGetCollection(collectionName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectionsApi#vectorGetCollection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectionsApi#vectorGetCollection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **collectionName** | **kotlin.String**|  | |

### Return type

[**VectorGetCollection200Response**](VectorGetCollection200Response.md)

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

<a id="vectorListCollections"></a>
# **vectorListCollections**
> VectorListCollections200Response vectorListCollections()

List collections

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CollectionsApi()
try {
    val result : VectorListCollections200Response = apiInstance.vectorListCollections()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CollectionsApi#vectorListCollections")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CollectionsApi#vectorListCollections")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**VectorListCollections200Response**](VectorListCollections200Response.md)

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

