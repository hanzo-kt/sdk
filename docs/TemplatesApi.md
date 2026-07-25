# TemplatesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoListTemplates**](TemplatesApi.md#autoListTemplates) | **GET** /v1/auto/templates | List flow templates |
| [**flowGetTemplate**](TemplatesApi.md#flowGetTemplate) | **GET** /v1/flow/templates/{id} | Get a template by id |
| [**flowListTemplates**](TemplatesApi.md#flowListTemplates) | **GET** /v1/flow/templates | List flow templates |
| [**templatesGetTemplate**](TemplatesApi.md#templatesGetTemplate) | **GET** /v1/templates/{slug} | One template by slug |
| [**templatesListTemplates**](TemplatesApi.md#templatesListTemplates) | **GET** /v1/templates | List the starter-kit catalog |


<a id="autoListTemplates"></a>
# **autoListTemplates**
> kotlin.Any autoListTemplates()

List flow templates

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplatesApi()
try {
    val result : kotlin.Any = apiInstance.autoListTemplates()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplatesApi#autoListTemplates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplatesApi#autoListTemplates")
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

<a id="flowGetTemplate"></a>
# **flowGetTemplate**
> FlowTemplate flowGetTemplate(id)

Get a template by id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplatesApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : FlowTemplate = apiInstance.flowGetTemplate(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplatesApi#flowGetTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplatesApi#flowGetTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**FlowTemplate**](FlowTemplate.md)

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

<a id="flowListTemplates"></a>
# **flowListTemplates**
> kotlin.Any flowListTemplates(pieces, tags)

List flow templates

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplatesApi()
val pieces : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val tags : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
try {
    val result : kotlin.Any = apiInstance.flowListTemplates(pieces, tags)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplatesApi#flowListTemplates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplatesApi#flowListTemplates")
    e.printStackTrace()
}
```

### Parameters
| **pieces** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **tags** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] |

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

<a id="templatesGetTemplate"></a>
# **templatesGetTemplate**
> TemplatesTemplate templatesGetTemplate(slug)

One template by slug

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplatesApi()
val slug : kotlin.String = slug_example // kotlin.String | 
try {
    val result : TemplatesTemplate = apiInstance.templatesGetTemplate(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplatesApi#templatesGetTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplatesApi#templatesGetTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**|  | |

### Return type

[**TemplatesTemplate**](TemplatesTemplate.md)

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

<a id="templatesListTemplates"></a>
# **templatesListTemplates**
> TemplatesListTemplates200Response templatesListTemplates()

List the starter-kit catalog

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplatesApi()
try {
    val result : TemplatesListTemplates200Response = apiInstance.templatesListTemplates()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplatesApi#templatesListTemplates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplatesApi#templatesListTemplates")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**TemplatesListTemplates200Response**](TemplatesListTemplates200Response.md)

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

