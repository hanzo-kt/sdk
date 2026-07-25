# ArticleAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddArticle**](ArticleAPIApi.md#cloudApiControllerAddArticle) | **POST** /v1/cloud/add-article | Api Controller Add Article |
| [**cloudApiControllerDeleteArticle**](ArticleAPIApi.md#cloudApiControllerDeleteArticle) | **POST** /v1/cloud/delete-article | Api Controller Delete Article |
| [**cloudApiControllerGetArticle**](ArticleAPIApi.md#cloudApiControllerGetArticle) | **GET** /v1/cloud/get-article | Api Controller Get Article |
| [**cloudApiControllerGetArticles**](ArticleAPIApi.md#cloudApiControllerGetArticles) | **GET** /v1/cloud/get-articles | Api Controller Get Articles |
| [**cloudApiControllerGetGlobalArticles**](ArticleAPIApi.md#cloudApiControllerGetGlobalArticles) | **GET** /v1/cloud/get-global-articles | Api Controller Get Global Articles |
| [**cloudApiControllerUpdateArticle**](ArticleAPIApi.md#cloudApiControllerUpdateArticle) | **POST** /v1/cloud/update-article | Api Controller Update Article |
| [**nexusAddArticle**](ArticleAPIApi.md#nexusAddArticle) | **POST** /v1/nexus/add-article | add Article |
| [**nexusDeleteArticle**](ArticleAPIApi.md#nexusDeleteArticle) | **POST** /v1/nexus/delete-article | delete Article |
| [**nexusGetArticle**](ArticleAPIApi.md#nexusGetArticle) | **GET** /v1/nexus/get-article | get Article |
| [**nexusGetArticles**](ArticleAPIApi.md#nexusGetArticles) | **GET** /v1/nexus/get-articles | get Articles |
| [**nexusGetGlobalArticles**](ArticleAPIApi.md#nexusGetGlobalArticles) | **GET** /v1/nexus/get-global-articles | get Global Articles |
| [**nexusUpdateArticle**](ArticleAPIApi.md#nexusUpdateArticle) | **POST** /v1/nexus/update-article | update Article |


<a id="cloudApiControllerAddArticle"></a>
# **cloudApiControllerAddArticle**
> CloudControllersResponse cloudApiControllerAddArticle(cloudObjectArticle)

Api Controller Add Article

add article

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArticleAPIApi()
val cloudObjectArticle : CloudObjectArticle =  // CloudObjectArticle | The details of the article
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddArticle(cloudObjectArticle)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArticleAPIApi#cloudApiControllerAddArticle")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArticleAPIApi#cloudApiControllerAddArticle")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectArticle** | [**CloudObjectArticle**](CloudObjectArticle.md)| The details of the article | |

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

<a id="cloudApiControllerDeleteArticle"></a>
# **cloudApiControllerDeleteArticle**
> CloudControllersResponse cloudApiControllerDeleteArticle(cloudObjectArticle)

Api Controller Delete Article

delete article

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArticleAPIApi()
val cloudObjectArticle : CloudObjectArticle =  // CloudObjectArticle | The details of the article
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteArticle(cloudObjectArticle)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArticleAPIApi#cloudApiControllerDeleteArticle")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArticleAPIApi#cloudApiControllerDeleteArticle")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectArticle** | [**CloudObjectArticle**](CloudObjectArticle.md)| The details of the article | |

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

<a id="cloudApiControllerGetArticle"></a>
# **cloudApiControllerGetArticle**
> CloudObjectArticle cloudApiControllerGetArticle(id)

Api Controller Get Article

get article

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArticleAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of article
try {
    val result : CloudObjectArticle = apiInstance.cloudApiControllerGetArticle(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArticleAPIApi#cloudApiControllerGetArticle")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArticleAPIApi#cloudApiControllerGetArticle")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of article | |

### Return type

[**CloudObjectArticle**](CloudObjectArticle.md)

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

<a id="cloudApiControllerGetArticles"></a>
# **cloudApiControllerGetArticles**
> kotlin.collections.List&lt;CloudObjectArticle&gt; cloudApiControllerGetArticles(owner)

Api Controller Get Articles

get articles

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArticleAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of article
try {
    val result : kotlin.collections.List<CloudObjectArticle> = apiInstance.cloudApiControllerGetArticles(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArticleAPIApi#cloudApiControllerGetArticles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArticleAPIApi#cloudApiControllerGetArticles")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of article | |

### Return type

[**kotlin.collections.List&lt;CloudObjectArticle&gt;**](CloudObjectArticle.md)

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

<a id="cloudApiControllerGetGlobalArticles"></a>
# **cloudApiControllerGetGlobalArticles**
> kotlin.collections.List&lt;CloudObjectArticle&gt; cloudApiControllerGetGlobalArticles()

Api Controller Get Global Articles

get global articles

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArticleAPIApi()
try {
    val result : kotlin.collections.List<CloudObjectArticle> = apiInstance.cloudApiControllerGetGlobalArticles()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArticleAPIApi#cloudApiControllerGetGlobalArticles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArticleAPIApi#cloudApiControllerGetGlobalArticles")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;CloudObjectArticle&gt;**](CloudObjectArticle.md)

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

<a id="cloudApiControllerUpdateArticle"></a>
# **cloudApiControllerUpdateArticle**
> CloudControllersResponse cloudApiControllerUpdateArticle(id, cloudObjectArticle)

Api Controller Update Article

update article

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArticleAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the article
val cloudObjectArticle : CloudObjectArticle =  // CloudObjectArticle | The details of the article
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateArticle(id, cloudObjectArticle)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArticleAPIApi#cloudApiControllerUpdateArticle")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArticleAPIApi#cloudApiControllerUpdateArticle")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the article | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectArticle** | [**CloudObjectArticle**](CloudObjectArticle.md)| The details of the article | |

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

<a id="nexusAddArticle"></a>
# **nexusAddArticle**
> NexusResponse nexusAddArticle(nexusArticle)

add Article

Add an article

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArticleAPIApi()
val nexusArticle : NexusArticle =  // NexusArticle | The details of the article
try {
    val result : NexusResponse = apiInstance.nexusAddArticle(nexusArticle)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArticleAPIApi#nexusAddArticle")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArticleAPIApi#nexusAddArticle")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusArticle** | [**NexusArticle**](NexusArticle.md)| The details of the article | |

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

<a id="nexusDeleteArticle"></a>
# **nexusDeleteArticle**
> NexusResponse nexusDeleteArticle(nexusArticle)

delete Article

Delete an article

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArticleAPIApi()
val nexusArticle : NexusArticle =  // NexusArticle | The details of the article
try {
    val result : NexusResponse = apiInstance.nexusDeleteArticle(nexusArticle)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArticleAPIApi#nexusDeleteArticle")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArticleAPIApi#nexusDeleteArticle")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusArticle** | [**NexusArticle**](NexusArticle.md)| The details of the article | |

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

<a id="nexusGetArticle"></a>
# **nexusGetArticle**
> NexusArticle nexusGetArticle(id)

get Article

Get an article

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArticleAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the article
try {
    val result : NexusArticle = apiInstance.nexusGetArticle(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArticleAPIApi#nexusGetArticle")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArticleAPIApi#nexusGetArticle")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the article | |

### Return type

[**NexusArticle**](NexusArticle.md)

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

<a id="nexusGetArticles"></a>
# **nexusGetArticles**
> kotlin.collections.List&lt;NexusArticle&gt; nexusGetArticles(owner)

get Articles

Get articles

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArticleAPIApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of the articles
try {
    val result : kotlin.collections.List<NexusArticle> = apiInstance.nexusGetArticles(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArticleAPIApi#nexusGetArticles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArticleAPIApi#nexusGetArticles")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of the articles | |

### Return type

[**kotlin.collections.List&lt;NexusArticle&gt;**](NexusArticle.md)

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

<a id="nexusGetGlobalArticles"></a>
# **nexusGetGlobalArticles**
> kotlin.collections.List&lt;NexusArticle&gt; nexusGetGlobalArticles()

get Global Articles

Get global articles

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArticleAPIApi()
try {
    val result : kotlin.collections.List<NexusArticle> = apiInstance.nexusGetGlobalArticles()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArticleAPIApi#nexusGetGlobalArticles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArticleAPIApi#nexusGetGlobalArticles")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;NexusArticle&gt;**](NexusArticle.md)

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

<a id="nexusUpdateArticle"></a>
# **nexusUpdateArticle**
> NexusResponse nexusUpdateArticle(id, nexusArticle)

update Article

Update an article

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ArticleAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the article
val nexusArticle : NexusArticle =  // NexusArticle | The details of the article
try {
    val result : NexusResponse = apiInstance.nexusUpdateArticle(id, nexusArticle)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ArticleAPIApi#nexusUpdateArticle")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ArticleAPIApi#nexusUpdateArticle")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the article | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **nexusArticle** | [**NexusArticle**](NexusArticle.md)| The details of the article | |

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

