# PiecesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoGetPiece**](PiecesApi.md#autoGetPiece) | **GET** /v1/auto/pieces/{name} | Get piece metadata by name |
| [**autoGetPieceOptions**](PiecesApi.md#autoGetPieceOptions) | **POST** /v1/auto/pieces/options | Get dynamic property options for a piece action/trigger |
| [**autoListPieceCategories**](PiecesApi.md#autoListPieceCategories) | **GET** /v1/auto/pieces/categories | List piece categories |
| [**autoListPieceVersions**](PiecesApi.md#autoListPieceVersions) | **GET** /v1/auto/pieces/versions | List available versions of a piece |
| [**autoListPieces**](PiecesApi.md#autoListPieces) | **GET** /v1/auto/pieces | List available pieces |
| [**automationsListPieces**](PiecesApi.md#automationsListPieces) | **GET** /v1/automations/pieces | List the connector/piece catalogue |
| [**flowGetPiece**](PiecesApi.md#flowGetPiece) | **GET** /v1/flow/pieces/{name} | Get piece metadata by name |
| [**flowGetPieceOptions**](PiecesApi.md#flowGetPieceOptions) | **POST** /v1/flow/pieces/options | Get dynamic property options for a piece action/trigger |
| [**flowGetPieceRegistry**](PiecesApi.md#flowGetPieceRegistry) | **GET** /v1/flow/pieces/registry | Get piece registry metadata |
| [**flowGetScopedPiece**](PiecesApi.md#flowGetScopedPiece) | **GET** /v1/flow/pieces/{scope}/{name} | Get scoped piece metadata |
| [**flowListPieceCategories**](PiecesApi.md#flowListPieceCategories) | **GET** /v1/flow/pieces/categories | List piece categories |
| [**flowListPieceVersions**](PiecesApi.md#flowListPieceVersions) | **GET** /v1/flow/pieces/versions | List available versions of a piece |
| [**flowListPieces**](PiecesApi.md#flowListPieces) | **GET** /v1/flow/pieces | List available pieces |
| [**flowSyncPieces**](PiecesApi.md#flowSyncPieces) | **POST** /v1/flow/pieces/sync | Sync piece metadata from registry |


<a id="autoGetPiece"></a>
# **autoGetPiece**
> AutoPiece autoGetPiece(name, version)

Get piece metadata by name

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PiecesApi()
val name : kotlin.String = name_example // kotlin.String | 
val version : kotlin.String = version_example // kotlin.String | 
try {
    val result : AutoPiece = apiInstance.autoGetPiece(name, version)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PiecesApi#autoGetPiece")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PiecesApi#autoGetPiece")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **version** | **kotlin.String**|  | [optional] |

### Return type

[**AutoPiece**](AutoPiece.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="autoGetPieceOptions"></a>
# **autoGetPieceOptions**
> kotlin.Any autoGetPieceOptions(autoGetPieceOptionsRequest)

Get dynamic property options for a piece action/trigger

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PiecesApi()
val autoGetPieceOptionsRequest : AutoGetPieceOptionsRequest =  // AutoGetPieceOptionsRequest | 
try {
    val result : kotlin.Any = apiInstance.autoGetPieceOptions(autoGetPieceOptionsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PiecesApi#autoGetPieceOptions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PiecesApi#autoGetPieceOptions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoGetPieceOptionsRequest** | [**AutoGetPieceOptionsRequest**](AutoGetPieceOptionsRequest.md)|  | |

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

<a id="autoListPieceCategories"></a>
# **autoListPieceCategories**
> kotlin.Any autoListPieceCategories()

List piece categories

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PiecesApi()
try {
    val result : kotlin.Any = apiInstance.autoListPieceCategories()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PiecesApi#autoListPieceCategories")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PiecesApi#autoListPieceCategories")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="autoListPieceVersions"></a>
# **autoListPieceVersions**
> kotlin.Any autoListPieceVersions(name)

List available versions of a piece

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PiecesApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoListPieceVersions(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PiecesApi#autoListPieceVersions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PiecesApi#autoListPieceVersions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="autoListPieces"></a>
# **autoListPieces**
> kotlin.collections.List&lt;AutoPiece&gt; autoListPieces(searchQuery, categories)

List available pieces

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PiecesApi()
val searchQuery : kotlin.String = searchQuery_example // kotlin.String | 
val categories : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
try {
    val result : kotlin.collections.List<AutoPiece> = apiInstance.autoListPieces(searchQuery, categories)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PiecesApi#autoListPieces")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PiecesApi#autoListPieces")
    e.printStackTrace()
}
```

### Parameters
| **searchQuery** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **categories** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] |

### Return type

[**kotlin.collections.List&lt;AutoPiece&gt;**](AutoPiece.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="automationsListPieces"></a>
# **automationsListPieces**
> AutomationsCatalog automationsListPieces()

List the connector/piece catalogue

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PiecesApi()
try {
    val result : AutomationsCatalog = apiInstance.automationsListPieces()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PiecesApi#automationsListPieces")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PiecesApi#automationsListPieces")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AutomationsCatalog**](AutomationsCatalog.md)

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

<a id="flowGetPiece"></a>
# **flowGetPiece**
> FlowPiece flowGetPiece(name, version)

Get piece metadata by name

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PiecesApi()
val name : kotlin.String = name_example // kotlin.String | 
val version : kotlin.String = version_example // kotlin.String | 
try {
    val result : FlowPiece = apiInstance.flowGetPiece(name, version)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PiecesApi#flowGetPiece")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PiecesApi#flowGetPiece")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **version** | **kotlin.String**|  | [optional] |

### Return type

[**FlowPiece**](FlowPiece.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="flowGetPieceOptions"></a>
# **flowGetPieceOptions**
> kotlin.Any flowGetPieceOptions(autoGetPieceOptionsRequest)

Get dynamic property options for a piece action/trigger

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PiecesApi()
val autoGetPieceOptionsRequest : AutoGetPieceOptionsRequest =  // AutoGetPieceOptionsRequest | 
try {
    val result : kotlin.Any = apiInstance.flowGetPieceOptions(autoGetPieceOptionsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PiecesApi#flowGetPieceOptions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PiecesApi#flowGetPieceOptions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoGetPieceOptionsRequest** | [**AutoGetPieceOptionsRequest**](AutoGetPieceOptionsRequest.md)|  | |

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

<a id="flowGetPieceRegistry"></a>
# **flowGetPieceRegistry**
> kotlin.Any flowGetPieceRegistry()

Get piece registry metadata

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PiecesApi()
try {
    val result : kotlin.Any = apiInstance.flowGetPieceRegistry()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PiecesApi#flowGetPieceRegistry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PiecesApi#flowGetPieceRegistry")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="flowGetScopedPiece"></a>
# **flowGetScopedPiece**
> FlowPiece flowGetScopedPiece(scope, name, version)

Get scoped piece metadata

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PiecesApi()
val scope : kotlin.String = scope_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val version : kotlin.String = version_example // kotlin.String | 
try {
    val result : FlowPiece = apiInstance.flowGetScopedPiece(scope, name, version)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PiecesApi#flowGetScopedPiece")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PiecesApi#flowGetScopedPiece")
    e.printStackTrace()
}
```

### Parameters
| **scope** | **kotlin.String**|  | |
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **version** | **kotlin.String**|  | [optional] |

### Return type

[**FlowPiece**](FlowPiece.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="flowListPieceCategories"></a>
# **flowListPieceCategories**
> kotlin.collections.List&lt;kotlin.String&gt; flowListPieceCategories()

List piece categories

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PiecesApi()
try {
    val result : kotlin.collections.List<kotlin.String> = apiInstance.flowListPieceCategories()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PiecesApi#flowListPieceCategories")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PiecesApi#flowListPieceCategories")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**kotlin.collections.List&lt;kotlin.String&gt;**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="flowListPieceVersions"></a>
# **flowListPieceVersions**
> kotlin.Any flowListPieceVersions(name)

List available versions of a piece

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PiecesApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowListPieceVersions(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PiecesApi#flowListPieceVersions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PiecesApi#flowListPieceVersions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="flowListPieces"></a>
# **flowListPieces**
> kotlin.collections.List&lt;FlowPiece&gt; flowListPieces(searchQuery, categories, includeHidden, includeTags, sortBy, orderBy)

List available pieces

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PiecesApi()
val searchQuery : kotlin.String = searchQuery_example // kotlin.String | 
val categories : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val includeHidden : kotlin.Boolean = true // kotlin.Boolean | 
val includeTags : kotlin.Boolean = true // kotlin.Boolean | 
val sortBy : kotlin.String = sortBy_example // kotlin.String | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
try {
    val result : kotlin.collections.List<FlowPiece> = apiInstance.flowListPieces(searchQuery, categories, includeHidden, includeTags, sortBy, orderBy)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PiecesApi#flowListPieces")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PiecesApi#flowListPieces")
    e.printStackTrace()
}
```

### Parameters
| **searchQuery** | **kotlin.String**|  | [optional] |
| **categories** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] |
| **includeHidden** | **kotlin.Boolean**|  | [optional] [default to false] |
| **includeTags** | **kotlin.Boolean**|  | [optional] [default to false] |
| **sortBy** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderBy** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;FlowPiece&gt;**](FlowPiece.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="flowSyncPieces"></a>
# **flowSyncPieces**
> kotlin.Any flowSyncPieces()

Sync piece metadata from registry

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PiecesApi()
try {
    val result : kotlin.Any = apiInstance.flowSyncPieces()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PiecesApi#flowSyncPieces")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PiecesApi#flowSyncPieces")
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

