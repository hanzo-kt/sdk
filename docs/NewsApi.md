# NewsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**worldWorldArxiv**](NewsApi.md#worldWorldArxiv) | **GET** /v1/world/arxiv | arXiv research feed (backs Robotics/Quantum lenses) |
| [**worldWorldGdeltDoc**](NewsApi.md#worldWorldGdeltDoc) | **GET** /v1/world/gdelt-doc | GDELT article search |
| [**worldWorldGdeltGeo**](NewsApi.md#worldWorldGdeltGeo) | **GET** /v1/world/gdelt-geo | GDELT geo-tagged events |
| [**worldWorldGithubTrending**](NewsApi.md#worldWorldGithubTrending) | **GET** /v1/world/github-trending | GitHub trending repositories |
| [**worldWorldHackernews**](NewsApi.md#worldWorldHackernews) | **GET** /v1/world/hackernews | Hacker News stories |
| [**worldWorldOgStory**](NewsApi.md#worldWorldOgStory) | **GET** /v1/world/og-story | Open-graph story card |
| [**worldWorldRssProxy**](NewsApi.md#worldWorldRssProxy) | **GET** /v1/world/rss-proxy | Allowlisted RSS feed proxy (SSRF-bounded) |
| [**worldWorldStory**](NewsApi.md#worldWorldStory) | **GET** /v1/world/story | Story detail |
| [**worldWorldTechEvents**](NewsApi.md#worldWorldTechEvents) | **GET** /v1/world/tech-events | Curated technology events |


<a id="worldWorldArxiv"></a>
# **worldWorldArxiv**
> kotlin.Any worldWorldArxiv(q, cat)

arXiv research feed (backs Robotics/Quantum lenses)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NewsApi()
val q : kotlin.String = q_example // kotlin.String | 
val cat : kotlin.String = cat_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.worldWorldArxiv(q, cat)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NewsApi#worldWorldArxiv")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NewsApi#worldWorldArxiv")
    e.printStackTrace()
}
```

### Parameters
| **q** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cat** | **kotlin.String**|  | [optional] |

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

<a id="worldWorldGdeltDoc"></a>
# **worldWorldGdeltDoc**
> kotlin.Any worldWorldGdeltDoc(query, maxrecords, timespan)

GDELT article search

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NewsApi()
val query : kotlin.String = query_example // kotlin.String | 
val maxrecords : kotlin.String = maxrecords_example // kotlin.String | 
val timespan : kotlin.String = timespan_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.worldWorldGdeltDoc(query, maxrecords, timespan)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NewsApi#worldWorldGdeltDoc")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NewsApi#worldWorldGdeltDoc")
    e.printStackTrace()
}
```

### Parameters
| **query** | **kotlin.String**|  | |
| **maxrecords** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **timespan** | **kotlin.String**|  | [optional] |

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

<a id="worldWorldGdeltGeo"></a>
# **worldWorldGdeltGeo**
> kotlin.Any worldWorldGdeltGeo(query, format, maxrecords, timespan)

GDELT geo-tagged events

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NewsApi()
val query : kotlin.String = query_example // kotlin.String | 
val format : kotlin.String = format_example // kotlin.String | 
val maxrecords : kotlin.String = maxrecords_example // kotlin.String | 
val timespan : kotlin.String = timespan_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.worldWorldGdeltGeo(query, format, maxrecords, timespan)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NewsApi#worldWorldGdeltGeo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NewsApi#worldWorldGdeltGeo")
    e.printStackTrace()
}
```

### Parameters
| **query** | **kotlin.String**|  | |
| **format** | **kotlin.String**|  | [optional] |
| **maxrecords** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **timespan** | **kotlin.String**|  | [optional] |

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

<a id="worldWorldGithubTrending"></a>
# **worldWorldGithubTrending**
> kotlin.Any worldWorldGithubTrending()

GitHub trending repositories

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NewsApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldGithubTrending()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NewsApi#worldWorldGithubTrending")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NewsApi#worldWorldGithubTrending")
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

<a id="worldWorldHackernews"></a>
# **worldWorldHackernews**
> kotlin.Any worldWorldHackernews(type)

Hacker News stories

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NewsApi()
val type : kotlin.String = type_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.worldWorldHackernews(type)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NewsApi#worldWorldHackernews")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NewsApi#worldWorldHackernews")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **type** | **kotlin.String**|  | [optional] |

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

<a id="worldWorldOgStory"></a>
# **worldWorldOgStory**
> kotlin.Any worldWorldOgStory()

Open-graph story card

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NewsApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldOgStory()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NewsApi#worldWorldOgStory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NewsApi#worldWorldOgStory")
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

<a id="worldWorldRssProxy"></a>
# **worldWorldRssProxy**
> kotlin.Any worldWorldRssProxy(url)

Allowlisted RSS feed proxy (SSRF-bounded)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NewsApi()
val url : kotlin.String = url_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.worldWorldRssProxy(url)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NewsApi#worldWorldRssProxy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NewsApi#worldWorldRssProxy")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **url** | **kotlin.String**|  | |

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

<a id="worldWorldStory"></a>
# **worldWorldStory**
> kotlin.Any worldWorldStory()

Story detail

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NewsApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldStory()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NewsApi#worldWorldStory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NewsApi#worldWorldStory")
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

<a id="worldWorldTechEvents"></a>
# **worldWorldTechEvents**
> kotlin.Any worldWorldTechEvents()

Curated technology events

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NewsApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldTechEvents()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NewsApi#worldWorldTechEvents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NewsApi#worldWorldTechEvents")
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

