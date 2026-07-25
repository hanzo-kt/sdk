# TemplateAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddTemplate**](TemplateAPIApi.md#cloudApiControllerAddTemplate) | **POST** /v1/cloud/add-template | Api Controller Add Template |
| [**cloudApiControllerDeleteTemplate**](TemplateAPIApi.md#cloudApiControllerDeleteTemplate) | **POST** /v1/cloud/delete-template | Api Controller Delete Template |
| [**cloudApiControllerGetTemplate**](TemplateAPIApi.md#cloudApiControllerGetTemplate) | **GET** /v1/cloud/get-template | Api Controller Get Template |
| [**cloudApiControllerGetTemplates**](TemplateAPIApi.md#cloudApiControllerGetTemplates) | **GET** /v1/cloud/get-templates | Api Controller Get Templates |
| [**cloudApiControllerUpdateTemplate**](TemplateAPIApi.md#cloudApiControllerUpdateTemplate) | **POST** /v1/cloud/update-template | Api Controller Update Template |
| [**nexusAddTemplate**](TemplateAPIApi.md#nexusAddTemplate) | **POST** /v1/nexus/add-template | add Template |
| [**nexusDeleteTemplate**](TemplateAPIApi.md#nexusDeleteTemplate) | **POST** /v1/nexus/delete-template | delete Template |
| [**nexusGetTemplate**](TemplateAPIApi.md#nexusGetTemplate) | **GET** /v1/nexus/get-template | get Template |
| [**nexusGetTemplates**](TemplateAPIApi.md#nexusGetTemplates) | **GET** /v1/nexus/get-templates | get Templates |
| [**nexusUpdateTemplate**](TemplateAPIApi.md#nexusUpdateTemplate) | **POST** /v1/nexus/update-template | update Template |


<a id="cloudApiControllerAddTemplate"></a>
# **cloudApiControllerAddTemplate**
> CloudControllersResponse cloudApiControllerAddTemplate(cloudObjectTemplate)

Api Controller Add Template

add template

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplateAPIApi()
val cloudObjectTemplate : CloudObjectTemplate =  // CloudObjectTemplate | The details of the template
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddTemplate(cloudObjectTemplate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplateAPIApi#cloudApiControllerAddTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplateAPIApi#cloudApiControllerAddTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectTemplate** | [**CloudObjectTemplate**](CloudObjectTemplate.md)| The details of the template | |

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

<a id="cloudApiControllerDeleteTemplate"></a>
# **cloudApiControllerDeleteTemplate**
> CloudControllersResponse cloudApiControllerDeleteTemplate(cloudObjectTemplate)

Api Controller Delete Template

delete template

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplateAPIApi()
val cloudObjectTemplate : CloudObjectTemplate =  // CloudObjectTemplate | The details of the template
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteTemplate(cloudObjectTemplate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplateAPIApi#cloudApiControllerDeleteTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplateAPIApi#cloudApiControllerDeleteTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectTemplate** | [**CloudObjectTemplate**](CloudObjectTemplate.md)| The details of the template | |

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

<a id="cloudApiControllerGetTemplate"></a>
# **cloudApiControllerGetTemplate**
> CloudObjectTemplate cloudApiControllerGetTemplate(id)

Api Controller Get Template

get template

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplateAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of template
try {
    val result : CloudObjectTemplate = apiInstance.cloudApiControllerGetTemplate(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplateAPIApi#cloudApiControllerGetTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplateAPIApi#cloudApiControllerGetTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of template | |

### Return type

[**CloudObjectTemplate**](CloudObjectTemplate.md)

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

<a id="cloudApiControllerGetTemplates"></a>
# **cloudApiControllerGetTemplates**
> kotlin.collections.List&lt;CloudObjectTemplate&gt; cloudApiControllerGetTemplates(owner)

Api Controller Get Templates

get templates

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplateAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of templates
try {
    val result : kotlin.collections.List<CloudObjectTemplate> = apiInstance.cloudApiControllerGetTemplates(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplateAPIApi#cloudApiControllerGetTemplates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplateAPIApi#cloudApiControllerGetTemplates")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of templates | |

### Return type

[**kotlin.collections.List&lt;CloudObjectTemplate&gt;**](CloudObjectTemplate.md)

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

<a id="cloudApiControllerUpdateTemplate"></a>
# **cloudApiControllerUpdateTemplate**
> CloudControllersResponse cloudApiControllerUpdateTemplate(id, cloudObjectTemplate)

Api Controller Update Template

update template

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplateAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the template
val cloudObjectTemplate : CloudObjectTemplate =  // CloudObjectTemplate | The details of the template
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateTemplate(id, cloudObjectTemplate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplateAPIApi#cloudApiControllerUpdateTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplateAPIApi#cloudApiControllerUpdateTemplate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the template | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectTemplate** | [**CloudObjectTemplate**](CloudObjectTemplate.md)| The details of the template | |

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

<a id="nexusAddTemplate"></a>
# **nexusAddTemplate**
> NexusResponse nexusAddTemplate(cloudObjectTemplate)

add Template

Add a template

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplateAPIApi()
val cloudObjectTemplate : CloudObjectTemplate =  // CloudObjectTemplate | The details of the template
try {
    val result : NexusResponse = apiInstance.nexusAddTemplate(cloudObjectTemplate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplateAPIApi#nexusAddTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplateAPIApi#nexusAddTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectTemplate** | [**CloudObjectTemplate**](CloudObjectTemplate.md)| The details of the template | |

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

<a id="nexusDeleteTemplate"></a>
# **nexusDeleteTemplate**
> NexusResponse nexusDeleteTemplate(cloudObjectTemplate)

delete Template

Delete a template

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplateAPIApi()
val cloudObjectTemplate : CloudObjectTemplate =  // CloudObjectTemplate | The details of the template
try {
    val result : NexusResponse = apiInstance.nexusDeleteTemplate(cloudObjectTemplate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplateAPIApi#nexusDeleteTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplateAPIApi#nexusDeleteTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectTemplate** | [**CloudObjectTemplate**](CloudObjectTemplate.md)| The details of the template | |

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

<a id="nexusGetTemplate"></a>
# **nexusGetTemplate**
> CloudObjectTemplate nexusGetTemplate(id)

get Template

Get a template

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplateAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id of the template
try {
    val result : CloudObjectTemplate = apiInstance.nexusGetTemplate(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplateAPIApi#nexusGetTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplateAPIApi#nexusGetTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id of the template | |

### Return type

[**CloudObjectTemplate**](CloudObjectTemplate.md)

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

<a id="nexusGetTemplates"></a>
# **nexusGetTemplates**
> kotlin.collections.List&lt;CloudObjectTemplate&gt; nexusGetTemplates(owner)

get Templates

Get templates

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplateAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of the templates
try {
    val result : kotlin.collections.List<CloudObjectTemplate> = apiInstance.nexusGetTemplates(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplateAPIApi#nexusGetTemplates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplateAPIApi#nexusGetTemplates")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of the templates | |

### Return type

[**kotlin.collections.List&lt;CloudObjectTemplate&gt;**](CloudObjectTemplate.md)

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

<a id="nexusUpdateTemplate"></a>
# **nexusUpdateTemplate**
> NexusResponse nexusUpdateTemplate(id, cloudObjectTemplate)

update Template

Update a template

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = TemplateAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the template
val cloudObjectTemplate : CloudObjectTemplate =  // CloudObjectTemplate | The details of the template
try {
    val result : NexusResponse = apiInstance.nexusUpdateTemplate(id, cloudObjectTemplate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TemplateAPIApi#nexusUpdateTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TemplateAPIApi#nexusUpdateTemplate")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the template | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectTemplate** | [**CloudObjectTemplate**](CloudObjectTemplate.md)| The details of the template | |

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

