# FacetSearchApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**searchFacetSearch**](FacetSearchApi.md#searchFacetSearch) | **POST** /v1/search/indexes/{indexUid}/facet-search | Search within facet values |


<a id="searchFacetSearch"></a>
# **searchFacetSearch**
> SearchFacetSearch200Response searchFacetSearch(indexUid, searchFacetSearchRequest)

Search within facet values

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FacetSearchApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
val searchFacetSearchRequest : SearchFacetSearchRequest =  // SearchFacetSearchRequest | 
try {
    val result : SearchFacetSearch200Response = apiInstance.searchFacetSearch(indexUid, searchFacetSearchRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FacetSearchApi#searchFacetSearch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FacetSearchApi#searchFacetSearch")
    e.printStackTrace()
}
```

### Parameters
| **indexUid** | **kotlin.String**| Unique index identifier | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchFacetSearchRequest** | [**SearchFacetSearchRequest**](SearchFacetSearchRequest.md)|  | |

### Return type

[**SearchFacetSearch200Response**](SearchFacetSearch200Response.md)

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

