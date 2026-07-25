# PointsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**vectorDeletePoints**](PointsApi.md#vectorDeletePoints) | **POST** /v1/vector/collections/{collection_name}/points/delete | Delete points |
| [**vectorGetPoint**](PointsApi.md#vectorGetPoint) | **GET** /v1/vector/collections/{collection_name}/points/{id} | Get point |
| [**vectorUpsertPoints**](PointsApi.md#vectorUpsertPoints) | **PUT** /v1/vector/collections/{collection_name}/points | Upsert points |


<a id="vectorDeletePoints"></a>
# **vectorDeletePoints**
> VectorDeletePoints200Response vectorDeletePoints(collectionName, vectorDeletePointsRequest, wait)

Delete points

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PointsApi()
val collectionName : kotlin.String = collectionName_example // kotlin.String | 
val vectorDeletePointsRequest : VectorDeletePointsRequest =  // VectorDeletePointsRequest | 
val wait : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : VectorDeletePoints200Response = apiInstance.vectorDeletePoints(collectionName, vectorDeletePointsRequest, wait)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PointsApi#vectorDeletePoints")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PointsApi#vectorDeletePoints")
    e.printStackTrace()
}
```

### Parameters
| **collectionName** | **kotlin.String**|  | |
| **vectorDeletePointsRequest** | [**VectorDeletePointsRequest**](VectorDeletePointsRequest.md)|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **wait** | **kotlin.Boolean**|  | [optional] [default to true] |

### Return type

[**VectorDeletePoints200Response**](VectorDeletePoints200Response.md)

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

<a id="vectorGetPoint"></a>
# **vectorGetPoint**
> VectorGetPoint200Response vectorGetPoint(collectionName, id)

Get point

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PointsApi()
val collectionName : kotlin.String = collectionName_example // kotlin.String | 
val id : VectorDeletePointsRequestPointsInner =  // VectorDeletePointsRequestPointsInner | 
try {
    val result : VectorGetPoint200Response = apiInstance.vectorGetPoint(collectionName, id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PointsApi#vectorGetPoint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PointsApi#vectorGetPoint")
    e.printStackTrace()
}
```

### Parameters
| **collectionName** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | [**VectorDeletePointsRequestPointsInner**](.md)|  | |

### Return type

[**VectorGetPoint200Response**](VectorGetPoint200Response.md)

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

<a id="vectorUpsertPoints"></a>
# **vectorUpsertPoints**
> VectorUpsertPoints200Response vectorUpsertPoints(collectionName, vectorUpsertPointsRequest, wait)

Upsert points

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PointsApi()
val collectionName : kotlin.String = collectionName_example // kotlin.String | 
val vectorUpsertPointsRequest : VectorUpsertPointsRequest =  // VectorUpsertPointsRequest | 
val wait : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : VectorUpsertPoints200Response = apiInstance.vectorUpsertPoints(collectionName, vectorUpsertPointsRequest, wait)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PointsApi#vectorUpsertPoints")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PointsApi#vectorUpsertPoints")
    e.printStackTrace()
}
```

### Parameters
| **collectionName** | **kotlin.String**|  | |
| **vectorUpsertPointsRequest** | [**VectorUpsertPointsRequest**](VectorUpsertPointsRequest.md)|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **wait** | **kotlin.Boolean**|  | [optional] [default to true] |

### Return type

[**VectorUpsertPoints200Response**](VectorUpsertPoints200Response.md)

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

