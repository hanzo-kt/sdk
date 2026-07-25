# PageviewsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**analyticsGetPageviews**](PageviewsApi.md#analyticsGetPageviews) | **GET** /v1/analytics/websites/{websiteId}/pageviews | Get pageview and session time series |


<a id="analyticsGetPageviews"></a>
# **analyticsGetPageviews**
> AnalyticsGetPageviews200Response analyticsGetPageviews(websiteId, startAt, endAt, unit, timezone, compare, url, referrer, title, os, browser, device, country, region, city, tag, host, language, event)

Get pageview and session time series

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PageviewsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
val unit : kotlin.String = unit_example // kotlin.String | 
val timezone : kotlin.String = America/Los_Angeles // kotlin.String | 
val compare : kotlin.String = compare_example // kotlin.String | 
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
    val result : AnalyticsGetPageviews200Response = apiInstance.analyticsGetPageviews(websiteId, startAt, endAt, unit, timezone, compare, url, referrer, title, os, browser, device, country, region, city, tag, host, language, event)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PageviewsApi#analyticsGetPageviews")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PageviewsApi#analyticsGetPageviews")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |
| **unit** | **kotlin.String**|  | [optional] [enum: minute, hour, day, week, month, year] |
| **timezone** | **kotlin.String**|  | [optional] |
| **compare** | **kotlin.String**|  | [optional] |
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

[**AnalyticsGetPageviews200Response**](AnalyticsGetPageviews200Response.md)

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

