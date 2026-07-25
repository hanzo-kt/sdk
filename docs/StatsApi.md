# StatsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**analyticsGetWebsiteMetrics**](StatsApi.md#analyticsGetWebsiteMetrics) | **GET** /v1/analytics/websites/{websiteId}/metrics | Get breakdown metrics by type (url, referrer, browser, os, device, country, event, channel, etc.) |
| [**analyticsGetWebsiteStats**](StatsApi.md#analyticsGetWebsiteStats) | **GET** /v1/analytics/websites/{websiteId}/stats | Get aggregate statistics for a website |
| [**searchGetIndexStats**](StatsApi.md#searchGetIndexStats) | **GET** /v1/search/indexes/{indexUid}/stats | Get index statistics |
| [**searchGetMetrics**](StatsApi.md#searchGetMetrics) | **GET** /metrics | Get Prometheus metrics |
| [**searchGetStats**](StatsApi.md#searchGetStats) | **GET** /v1/search/stats | Get global statistics |


<a id="analyticsGetWebsiteMetrics"></a>
# **analyticsGetWebsiteMetrics**
> kotlin.collections.List&lt;AnalyticsMetric&gt; analyticsGetWebsiteMetrics(websiteId, startAt, endAt, type, limit, offset, search, url, referrer, title, os, browser, device, country, region, city, tag, host, language, event)

Get breakdown metrics by type (url, referrer, browser, os, device, country, event, channel, etc.)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StatsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
val type : kotlin.String = type_example // kotlin.String | Metric type to break down by
val limit : kotlin.Int = 56 // kotlin.Int | 
val offset : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val url : kotlin.String = url_example // kotlin.String | 
val referrer : kotlin.String = referrer_example // kotlin.String | 
val title : kotlin.String = title_example // kotlin.String | 
val os : kotlin.String = os_example // kotlin.String | 
val browser : kotlin.String = browser_example // kotlin.String | 
val device : kotlin.String = device_example // kotlin.String | 
val country : kotlin.String = country_example // kotlin.String | 
val region : kotlin.String = region_example // kotlin.String | 
val city : kotlin.String = city_example // kotlin.String | 
val tag : kotlin.String = tag_example // kotlin.String | 
val host : kotlin.String = host_example // kotlin.String | 
val language : kotlin.String = language_example // kotlin.String | 
val event : kotlin.String = event_example // kotlin.String | 
try {
    val result : kotlin.collections.List<AnalyticsMetric> = apiInstance.analyticsGetWebsiteMetrics(websiteId, startAt, endAt, type, limit, offset, search, url, referrer, title, os, browser, device, country, region, city, tag, host, language, event)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StatsApi#analyticsGetWebsiteMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StatsApi#analyticsGetWebsiteMetrics")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |
| **type** | **kotlin.String**| Metric type to break down by | [enum: url, referrer, title, browser, os, device, country, region, city, language, event, tag, host, query, channel] |
| **limit** | **kotlin.Int**|  | [optional] |
| **offset** | **kotlin.Int**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **url** | **kotlin.String**|  | [optional] |
| **referrer** | **kotlin.String**|  | [optional] |
| **title** | **kotlin.String**|  | [optional] |
| **os** | **kotlin.String**|  | [optional] |
| **browser** | **kotlin.String**|  | [optional] |
| **device** | **kotlin.String**|  | [optional] |
| **country** | **kotlin.String**|  | [optional] |
| **region** | **kotlin.String**|  | [optional] |
| **city** | **kotlin.String**|  | [optional] |
| **tag** | **kotlin.String**|  | [optional] |
| **host** | **kotlin.String**|  | [optional] |
| **language** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **event** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;AnalyticsMetric&gt;**](AnalyticsMetric.md)

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

<a id="analyticsGetWebsiteStats"></a>
# **analyticsGetWebsiteStats**
> AnalyticsGetWebsiteStats200Response analyticsGetWebsiteStats(websiteId, startAt, endAt, compare, url, referrer, title, os, browser, device, country, region, city, tag, host, language, event)

Get aggregate statistics for a website

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StatsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
val compare : kotlin.String = compare_example // kotlin.String | Compare period (e.g. \"previous_period\")
val url : kotlin.String = url_example // kotlin.String | 
val referrer : kotlin.String = referrer_example // kotlin.String | 
val title : kotlin.String = title_example // kotlin.String | 
val os : kotlin.String = os_example // kotlin.String | 
val browser : kotlin.String = browser_example // kotlin.String | 
val device : kotlin.String = device_example // kotlin.String | 
val country : kotlin.String = country_example // kotlin.String | 
val region : kotlin.String = region_example // kotlin.String | 
val city : kotlin.String = city_example // kotlin.String | 
val tag : kotlin.String = tag_example // kotlin.String | 
val host : kotlin.String = host_example // kotlin.String | 
val language : kotlin.String = language_example // kotlin.String | 
val event : kotlin.String = event_example // kotlin.String | 
try {
    val result : AnalyticsGetWebsiteStats200Response = apiInstance.analyticsGetWebsiteStats(websiteId, startAt, endAt, compare, url, referrer, title, os, browser, device, country, region, city, tag, host, language, event)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StatsApi#analyticsGetWebsiteStats")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StatsApi#analyticsGetWebsiteStats")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |
| **compare** | **kotlin.String**| Compare period (e.g. \&quot;previous_period\&quot;) | [optional] |
| **url** | **kotlin.String**|  | [optional] |
| **referrer** | **kotlin.String**|  | [optional] |
| **title** | **kotlin.String**|  | [optional] |
| **os** | **kotlin.String**|  | [optional] |
| **browser** | **kotlin.String**|  | [optional] |
| **device** | **kotlin.String**|  | [optional] |
| **country** | **kotlin.String**|  | [optional] |
| **region** | **kotlin.String**|  | [optional] |
| **city** | **kotlin.String**|  | [optional] |
| **tag** | **kotlin.String**|  | [optional] |
| **host** | **kotlin.String**|  | [optional] |
| **language** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **event** | **kotlin.String**|  | [optional] |

### Return type

[**AnalyticsGetWebsiteStats200Response**](AnalyticsGetWebsiteStats200Response.md)

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

<a id="searchGetIndexStats"></a>
# **searchGetIndexStats**
> SearchIndexStats searchGetIndexStats(indexUid)

Get index statistics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StatsApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
try {
    val result : SearchIndexStats = apiInstance.searchGetIndexStats(indexUid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StatsApi#searchGetIndexStats")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StatsApi#searchGetIndexStats")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **indexUid** | **kotlin.String**| Unique index identifier | |

### Return type

[**SearchIndexStats**](SearchIndexStats.md)

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

<a id="searchGetMetrics"></a>
# **searchGetMetrics**
> kotlin.String searchGetMetrics()

Get Prometheus metrics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StatsApi()
try {
    val result : kotlin.String = apiInstance.searchGetMetrics()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StatsApi#searchGetMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StatsApi#searchGetMetrics")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**kotlin.String**

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
 - **Accept**: text/plain

<a id="searchGetStats"></a>
# **searchGetStats**
> SearchStats searchGetStats()

Get global statistics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StatsApi()
try {
    val result : SearchStats = apiInstance.searchGetStats()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StatsApi#searchGetStats")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StatsApi#searchGetStats")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**SearchStats**](SearchStats.md)

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

