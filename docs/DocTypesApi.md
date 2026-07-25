# DocTypesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**frameworkCreateDocType**](DocTypesApi.md#frameworkCreateDocType) | **POST** /v1/framework/doctypes | Define a DocType |
| [**frameworkDeleteDocType**](DocTypesApi.md#frameworkDeleteDocType) | **DELETE** /v1/framework/doctypes/{name} | Delete a DocType (and its documents) |
| [**frameworkFrameworkSummary**](DocTypesApi.md#frameworkFrameworkSummary) | **GET** /v1/framework/summary | Org summary (doctype + document counts) |
| [**frameworkGetDocType**](DocTypesApi.md#frameworkGetDocType) | **GET** /v1/framework/doctypes/{name} | Get a DocType definition |
| [**frameworkListDocTypes**](DocTypesApi.md#frameworkListDocTypes) | **GET** /v1/framework/doctypes | List DocType definitions |
| [**frameworkReplaceDocType**](DocTypesApi.md#frameworkReplaceDocType) | **PUT** /v1/framework/doctypes/{name} | Replace a DocType definition |


<a id="frameworkCreateDocType"></a>
# **frameworkCreateDocType**
> FrameworkDocType frameworkCreateDocType(frameworkDocType)

Define a DocType

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocTypesApi()
val frameworkDocType : FrameworkDocType =  // FrameworkDocType | 
try {
    val result : FrameworkDocType = apiInstance.frameworkCreateDocType(frameworkDocType)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocTypesApi#frameworkCreateDocType")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocTypesApi#frameworkCreateDocType")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **frameworkDocType** | [**FrameworkDocType**](FrameworkDocType.md)|  | |

### Return type

[**FrameworkDocType**](FrameworkDocType.md)

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

<a id="frameworkDeleteDocType"></a>
# **frameworkDeleteDocType**
> frameworkDeleteDocType(name)

Delete a DocType (and its documents)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocTypesApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    apiInstance.frameworkDeleteDocType(name)
} catch (e: ClientException) {
    println("4xx response calling DocTypesApi#frameworkDeleteDocType")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocTypesApi#frameworkDeleteDocType")
    e.printStackTrace()
}
```

### Parameters
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

<a id="frameworkFrameworkSummary"></a>
# **frameworkFrameworkSummary**
> FrameworkFrameworkSummary200Response frameworkFrameworkSummary()

Org summary (doctype + document counts)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocTypesApi()
try {
    val result : FrameworkFrameworkSummary200Response = apiInstance.frameworkFrameworkSummary()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocTypesApi#frameworkFrameworkSummary")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocTypesApi#frameworkFrameworkSummary")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**FrameworkFrameworkSummary200Response**](FrameworkFrameworkSummary200Response.md)

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

<a id="frameworkGetDocType"></a>
# **frameworkGetDocType**
> FrameworkDocType frameworkGetDocType(name)

Get a DocType definition

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocTypesApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : FrameworkDocType = apiInstance.frameworkGetDocType(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocTypesApi#frameworkGetDocType")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocTypesApi#frameworkGetDocType")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**FrameworkDocType**](FrameworkDocType.md)

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

<a id="frameworkListDocTypes"></a>
# **frameworkListDocTypes**
> FrameworkListDocTypes200Response frameworkListDocTypes()

List DocType definitions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocTypesApi()
try {
    val result : FrameworkListDocTypes200Response = apiInstance.frameworkListDocTypes()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocTypesApi#frameworkListDocTypes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocTypesApi#frameworkListDocTypes")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**FrameworkListDocTypes200Response**](FrameworkListDocTypes200Response.md)

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

<a id="frameworkReplaceDocType"></a>
# **frameworkReplaceDocType**
> FrameworkDocType frameworkReplaceDocType(name, frameworkDocType)

Replace a DocType definition

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DocTypesApi()
val name : kotlin.String = name_example // kotlin.String | 
val frameworkDocType : FrameworkDocType =  // FrameworkDocType | 
try {
    val result : FrameworkDocType = apiInstance.frameworkReplaceDocType(name, frameworkDocType)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DocTypesApi#frameworkReplaceDocType")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DocTypesApi#frameworkReplaceDocType")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **frameworkDocType** | [**FrameworkDocType**](FrameworkDocType.md)|  | |

### Return type

[**FrameworkDocType**](FrameworkDocType.md)

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

