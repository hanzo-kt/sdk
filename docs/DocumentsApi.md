# DocumentsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**frameworkCancelDocument**](DocumentsApi.md#frameworkCancelDocument) | **POST** /v1/framework/{doctype}/{name}/cancel | Cancel a submitted document (docstatus 1→2) |
| [**frameworkCreateDocument**](DocumentsApi.md#frameworkCreateDocument) | **POST** /v1/framework/{doctype} | Create a document |
| [**frameworkDeleteDocument**](DocumentsApi.md#frameworkDeleteDocument) | **DELETE** /v1/framework/{doctype}/{name} | Delete a document |
| [**frameworkGetDocument**](DocumentsApi.md#frameworkGetDocument) | **GET** /v1/framework/{doctype}/{name} | Get a document |
| [**frameworkListDocuments**](DocumentsApi.md#frameworkListDocuments) | **GET** /v1/framework/{doctype} | List documents of a DocType |
| [**frameworkSubmitDocument**](DocumentsApi.md#frameworkSubmitDocument) | **POST** /v1/framework/{doctype}/{name}/submit | Submit a document (docstatus 0→1) |
| [**frameworkUpdateDocument**](DocumentsApi.md#frameworkUpdateDocument) | **PUT** /v1/framework/{doctype}/{name} | Update a draft document |
| [**searchAddOrReplaceDocuments**](DocumentsApi.md#searchAddOrReplaceDocuments) | **POST** /v1/search/indexes/{indexUid}/documents | Add or replace documents |
| [**searchAddOrUpdateDocuments**](DocumentsApi.md#searchAddOrUpdateDocuments) | **PUT** /v1/search/indexes/{indexUid}/documents | Add or update documents (partial) |
| [**searchDeleteAllDocuments**](DocumentsApi.md#searchDeleteAllDocuments) | **DELETE** /v1/search/indexes/{indexUid}/documents | Delete all documents in the index |
| [**searchDeleteDocument**](DocumentsApi.md#searchDeleteDocument) | **DELETE** /v1/search/indexes/{indexUid}/documents/{documentId} | Delete a single document |
| [**searchDeleteDocumentsBatch**](DocumentsApi.md#searchDeleteDocumentsBatch) | **POST** /v1/search/indexes/{indexUid}/documents/delete-batch | Delete documents by IDs |
| [**searchDeleteDocumentsByFilter**](DocumentsApi.md#searchDeleteDocumentsByFilter) | **POST** /v1/search/indexes/{indexUid}/documents/delete | Delete documents by filter |
| [**searchEditDocumentsByFunction**](DocumentsApi.md#searchEditDocumentsByFunction) | **POST** /v1/search/indexes/{indexUid}/documents/edit | Edit documents using a function |
| [**searchGetDocument**](DocumentsApi.md#searchGetDocument) | **GET** /v1/search/indexes/{indexUid}/documents/{documentId} | Get a single document |
| [**searchGetDocuments**](DocumentsApi.md#searchGetDocuments) | **GET** /v1/search/indexes/{indexUid}/documents | Browse documents |


<a id="frameworkCancelDocument"></a>
# **frameworkCancelDocument**
> FrameworkDocument frameworkCancelDocument(doctype, name)

Cancel a submitted document (docstatus 1→2)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val doctype : kotlin.String = doctype_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : FrameworkDocument = apiInstance.frameworkCancelDocument(doctype, name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#frameworkCancelDocument")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#frameworkCancelDocument")
    e.printStackTrace()
}
```

### Parameters
| **doctype** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**FrameworkDocument**](FrameworkDocument.md)

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

<a id="frameworkCreateDocument"></a>
# **frameworkCreateDocument**
> FrameworkDocument frameworkCreateDocument(doctype, frameworkDocument)

Create a document

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val doctype : kotlin.String = doctype_example // kotlin.String | 
val frameworkDocument : FrameworkDocument =  // FrameworkDocument | 
try {
    val result : FrameworkDocument = apiInstance.frameworkCreateDocument(doctype, frameworkDocument)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#frameworkCreateDocument")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#frameworkCreateDocument")
    e.printStackTrace()
}
```

### Parameters
| **doctype** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **frameworkDocument** | [**FrameworkDocument**](FrameworkDocument.md)|  | |

### Return type

[**FrameworkDocument**](FrameworkDocument.md)

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

<a id="frameworkDeleteDocument"></a>
# **frameworkDeleteDocument**
> frameworkDeleteDocument(doctype, name)

Delete a document

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val doctype : kotlin.String = doctype_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
try {
    apiInstance.frameworkDeleteDocument(doctype, name)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#frameworkDeleteDocument")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#frameworkDeleteDocument")
    e.printStackTrace()
}
```

### Parameters
| **doctype** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

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
 - **Accept**: application/json

<a id="frameworkGetDocument"></a>
# **frameworkGetDocument**
> FrameworkDocument frameworkGetDocument(doctype, name)

Get a document

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val doctype : kotlin.String = doctype_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : FrameworkDocument = apiInstance.frameworkGetDocument(doctype, name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#frameworkGetDocument")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#frameworkGetDocument")
    e.printStackTrace()
}
```

### Parameters
| **doctype** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**FrameworkDocument**](FrameworkDocument.md)

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

<a id="frameworkListDocuments"></a>
# **frameworkListDocuments**
> FrameworkListDocuments200Response frameworkListDocuments(doctype, filters, fields, orderBy, limit)

List documents of a DocType

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val doctype : kotlin.String = doctype_example // kotlin.String | 
val filters : kotlin.String = filters_example // kotlin.String | 'JSON object of field→value filters (declared fields, name, or docstatus)'
val fields : kotlin.String = fields_example // kotlin.String | Comma list or JSON array of field names to project
val orderBy : kotlin.String = orderBy_example // kotlin.String | field [asc|desc]
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : FrameworkListDocuments200Response = apiInstance.frameworkListDocuments(doctype, filters, fields, orderBy, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#frameworkListDocuments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#frameworkListDocuments")
    e.printStackTrace()
}
```

### Parameters
| **doctype** | **kotlin.String**|  | |
| **filters** | **kotlin.String**| &#39;JSON object of field→value filters (declared fields, name, or docstatus)&#39; | [optional] |
| **fields** | **kotlin.String**| Comma list or JSON array of field names to project | [optional] |
| **orderBy** | **kotlin.String**| field [asc|desc] | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 100] |

### Return type

[**FrameworkListDocuments200Response**](FrameworkListDocuments200Response.md)

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

<a id="frameworkSubmitDocument"></a>
# **frameworkSubmitDocument**
> FrameworkDocument frameworkSubmitDocument(doctype, name)

Submit a document (docstatus 0→1)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val doctype : kotlin.String = doctype_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : FrameworkDocument = apiInstance.frameworkSubmitDocument(doctype, name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#frameworkSubmitDocument")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#frameworkSubmitDocument")
    e.printStackTrace()
}
```

### Parameters
| **doctype** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**FrameworkDocument**](FrameworkDocument.md)

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

<a id="frameworkUpdateDocument"></a>
# **frameworkUpdateDocument**
> FrameworkDocument frameworkUpdateDocument(doctype, name, frameworkDocument)

Update a draft document

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val doctype : kotlin.String = doctype_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val frameworkDocument : FrameworkDocument =  // FrameworkDocument | 
try {
    val result : FrameworkDocument = apiInstance.frameworkUpdateDocument(doctype, name, frameworkDocument)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#frameworkUpdateDocument")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#frameworkUpdateDocument")
    e.printStackTrace()
}
```

### Parameters
| **doctype** | **kotlin.String**|  | |
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **frameworkDocument** | [**FrameworkDocument**](FrameworkDocument.md)|  | |

### Return type

[**FrameworkDocument**](FrameworkDocument.md)

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

<a id="searchAddOrReplaceDocuments"></a>
# **searchAddOrReplaceDocuments**
> SearchSummarizedTaskView searchAddOrReplaceDocuments(indexUid, requestBody, primaryKey)

Add or replace documents

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
val requestBody : kotlin.collections.List<kotlin.Any> =  // kotlin.collections.List<kotlin.Any> | 
val primaryKey : kotlin.String = primaryKey_example // kotlin.String | Primary key field name
try {
    val result : SearchSummarizedTaskView = apiInstance.searchAddOrReplaceDocuments(indexUid, requestBody, primaryKey)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#searchAddOrReplaceDocuments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#searchAddOrReplaceDocuments")
    e.printStackTrace()
}
```

### Parameters
| **indexUid** | **kotlin.String**| Unique index identifier | |
| **requestBody** | [**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **primaryKey** | **kotlin.String**| Primary key field name | [optional] |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="searchAddOrUpdateDocuments"></a>
# **searchAddOrUpdateDocuments**
> SearchSummarizedTaskView searchAddOrUpdateDocuments(indexUid, requestBody, primaryKey)

Add or update documents (partial)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
val requestBody : kotlin.collections.List<kotlin.Any> =  // kotlin.collections.List<kotlin.Any> | 
val primaryKey : kotlin.String = primaryKey_example // kotlin.String | 
try {
    val result : SearchSummarizedTaskView = apiInstance.searchAddOrUpdateDocuments(indexUid, requestBody, primaryKey)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#searchAddOrUpdateDocuments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#searchAddOrUpdateDocuments")
    e.printStackTrace()
}
```

### Parameters
| **indexUid** | **kotlin.String**| Unique index identifier | |
| **requestBody** | [**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **primaryKey** | **kotlin.String**|  | [optional] |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="searchDeleteAllDocuments"></a>
# **searchDeleteAllDocuments**
> SearchSummarizedTaskView searchDeleteAllDocuments(indexUid)

Delete all documents in the index

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
try {
    val result : SearchSummarizedTaskView = apiInstance.searchDeleteAllDocuments(indexUid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#searchDeleteAllDocuments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#searchDeleteAllDocuments")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **indexUid** | **kotlin.String**| Unique index identifier | |

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

<a id="searchDeleteDocument"></a>
# **searchDeleteDocument**
> SearchSummarizedTaskView searchDeleteDocument(indexUid, documentId)

Delete a single document

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
val documentId : kotlin.String = documentId_example // kotlin.String | 
try {
    val result : SearchSummarizedTaskView = apiInstance.searchDeleteDocument(indexUid, documentId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#searchDeleteDocument")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#searchDeleteDocument")
    e.printStackTrace()
}
```

### Parameters
| **indexUid** | **kotlin.String**| Unique index identifier | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **documentId** | **kotlin.String**|  | |

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

<a id="searchDeleteDocumentsBatch"></a>
# **searchDeleteDocumentsBatch**
> SearchSummarizedTaskView searchDeleteDocumentsBatch(indexUid, requestBody)

Delete documents by IDs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
val requestBody : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
try {
    val result : SearchSummarizedTaskView = apiInstance.searchDeleteDocumentsBatch(indexUid, requestBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#searchDeleteDocumentsBatch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#searchDeleteDocumentsBatch")
    e.printStackTrace()
}
```

### Parameters
| **indexUid** | **kotlin.String**| Unique index identifier | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **requestBody** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="searchDeleteDocumentsByFilter"></a>
# **searchDeleteDocumentsByFilter**
> SearchSummarizedTaskView searchDeleteDocumentsByFilter(indexUid, searchDeleteDocumentsByFilterRequest)

Delete documents by filter

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
val searchDeleteDocumentsByFilterRequest : SearchDeleteDocumentsByFilterRequest =  // SearchDeleteDocumentsByFilterRequest | 
try {
    val result : SearchSummarizedTaskView = apiInstance.searchDeleteDocumentsByFilter(indexUid, searchDeleteDocumentsByFilterRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#searchDeleteDocumentsByFilter")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#searchDeleteDocumentsByFilter")
    e.printStackTrace()
}
```

### Parameters
| **indexUid** | **kotlin.String**| Unique index identifier | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchDeleteDocumentsByFilterRequest** | [**SearchDeleteDocumentsByFilterRequest**](SearchDeleteDocumentsByFilterRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="searchEditDocumentsByFunction"></a>
# **searchEditDocumentsByFunction**
> SearchSummarizedTaskView searchEditDocumentsByFunction(indexUid, searchEditDocumentsByFunctionRequest)

Edit documents using a function

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
val searchEditDocumentsByFunctionRequest : SearchEditDocumentsByFunctionRequest =  // SearchEditDocumentsByFunctionRequest | 
try {
    val result : SearchSummarizedTaskView = apiInstance.searchEditDocumentsByFunction(indexUid, searchEditDocumentsByFunctionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#searchEditDocumentsByFunction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#searchEditDocumentsByFunction")
    e.printStackTrace()
}
```

### Parameters
| **indexUid** | **kotlin.String**| Unique index identifier | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchEditDocumentsByFunctionRequest** | [**SearchEditDocumentsByFunctionRequest**](SearchEditDocumentsByFunctionRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="searchGetDocument"></a>
# **searchGetDocument**
> kotlin.Any searchGetDocument(indexUid, documentId, fields)

Get a single document

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
val documentId : kotlin.String = documentId_example // kotlin.String | 
val fields : kotlin.String = fields_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.searchGetDocument(indexUid, documentId, fields)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#searchGetDocument")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#searchGetDocument")
    e.printStackTrace()
}
```

### Parameters
| **indexUid** | **kotlin.String**| Unique index identifier | |
| **documentId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **fields** | **kotlin.String**|  | [optional] |

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

<a id="searchGetDocuments"></a>
# **searchGetDocuments**
> SearchPaginatedDocuments searchGetDocuments(indexUid, offset, limit, fields, filter)

Browse documents

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocumentsApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
val offset : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val fields : kotlin.String = fields_example // kotlin.String | Comma-separated fields to return
val filter : kotlin.String = filter_example // kotlin.String | 
try {
    val result : SearchPaginatedDocuments = apiInstance.searchGetDocuments(indexUid, offset, limit, fields, filter)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocumentsApi#searchGetDocuments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocumentsApi#searchGetDocuments")
    e.printStackTrace()
}
```

### Parameters
| **indexUid** | **kotlin.String**| Unique index identifier | |
| **offset** | **kotlin.Int**|  | [optional] [default to 0] |
| **limit** | **kotlin.Int**|  | [optional] [default to 20] |
| **fields** | **kotlin.String**| Comma-separated fields to return | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **filter** | **kotlin.String**|  | [optional] |

### Return type

[**SearchPaginatedDocuments**](SearchPaginatedDocuments.md)

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

