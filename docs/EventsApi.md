# EventsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**analyticsGetEventDataEvents**](EventsApi.md#analyticsGetEventDataEvents) | **GET** /v1/analytics/websites/{websiteId}/event-data/events | Get event data grouped by event name |
| [**analyticsGetEventDataFields**](EventsApi.md#analyticsGetEventDataFields) | **GET** /v1/analytics/websites/{websiteId}/event-data/fields | Get event data fields |
| [**analyticsGetEventDataProperties**](EventsApi.md#analyticsGetEventDataProperties) | **GET** /v1/analytics/websites/{websiteId}/event-data/properties | Get event data properties |
| [**analyticsGetEventDataStats**](EventsApi.md#analyticsGetEventDataStats) | **GET** /v1/analytics/websites/{websiteId}/event-data/stats | Get event data aggregate stats |
| [**analyticsGetEventDataValues**](EventsApi.md#analyticsGetEventDataValues) | **GET** /v1/analytics/websites/{websiteId}/event-data/values | Get event data values for a property |
| [**analyticsGetEventSeries**](EventsApi.md#analyticsGetEventSeries) | **GET** /v1/analytics/websites/{websiteId}/events/series | Get event metrics as a time series |
| [**analyticsGetEvents**](EventsApi.md#analyticsGetEvents) | **GET** /v1/analytics/websites/{websiteId}/events | Get paginated list of events |
| [**s3GetBucketNotification**](EventsApi.md#s3GetBucketNotification) | **GET** /v1/s3/{bucket}?notification | Get event notification config |
| [**s3PutBucketNotification**](EventsApi.md#s3PutBucketNotification) | **PUT** /v1/s3/{bucket}?notification | Set event notification config |


<a id="analyticsGetEventDataEvents"></a>
# **analyticsGetEventDataEvents**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsGetEventDataEvents(websiteId, startAt, endAt, event)

Get event data grouped by event name

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EventsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
val event : kotlin.String = event_example // kotlin.String | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsGetEventDataEvents(websiteId, startAt, endAt, event)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EventsApi#analyticsGetEventDataEvents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EventsApi#analyticsGetEventDataEvents")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **event** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="analyticsGetEventDataFields"></a>
# **analyticsGetEventDataFields**
> kotlin.collections.List&lt;AnalyticsGetEventDataFields200ResponseInner&gt; analyticsGetEventDataFields(websiteId, startAt, endAt)

Get event data fields

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EventsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
try {
    val result : kotlin.collections.List<AnalyticsGetEventDataFields200ResponseInner> = apiInstance.analyticsGetEventDataFields(websiteId, startAt, endAt)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EventsApi#analyticsGetEventDataFields")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EventsApi#analyticsGetEventDataFields")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |

### Return type

[**kotlin.collections.List&lt;AnalyticsGetEventDataFields200ResponseInner&gt;**](AnalyticsGetEventDataFields200ResponseInner.md)

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

<a id="analyticsGetEventDataProperties"></a>
# **analyticsGetEventDataProperties**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsGetEventDataProperties(websiteId, startAt, endAt, propertyName)

Get event data properties

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EventsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
val propertyName : kotlin.String = propertyName_example // kotlin.String | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsGetEventDataProperties(websiteId, startAt, endAt, propertyName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EventsApi#analyticsGetEventDataProperties")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EventsApi#analyticsGetEventDataProperties")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **propertyName** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="analyticsGetEventDataStats"></a>
# **analyticsGetEventDataStats**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsGetEventDataStats(websiteId, startAt, endAt, propertyName)

Get event data aggregate stats

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EventsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
val propertyName : kotlin.String = propertyName_example // kotlin.String | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsGetEventDataStats(websiteId, startAt, endAt, propertyName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EventsApi#analyticsGetEventDataStats")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EventsApi#analyticsGetEventDataStats")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **propertyName** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="analyticsGetEventDataValues"></a>
# **analyticsGetEventDataValues**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsGetEventDataValues(websiteId, startAt, endAt, eventName, propertyName)

Get event data values for a property

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EventsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
val eventName : kotlin.String = eventName_example // kotlin.String | 
val propertyName : kotlin.String = propertyName_example // kotlin.String | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsGetEventDataValues(websiteId, startAt, endAt, eventName, propertyName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EventsApi#analyticsGetEventDataValues")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EventsApi#analyticsGetEventDataValues")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |
| **eventName** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **propertyName** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="analyticsGetEventSeries"></a>
# **analyticsGetEventSeries**
> kotlin.collections.List&lt;AnalyticsPageviewSeries&gt; analyticsGetEventSeries(websiteId, startAt, endAt, unit, timezone, url, referrer, title, os, browser, device, country, region, city, tag, host, language, event)

Get event metrics as a time series

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EventsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
val unit : kotlin.String = unit_example // kotlin.String | 
val timezone : kotlin.String = America/Los_Angeles // kotlin.String | 
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
    val result : kotlin.collections.List<AnalyticsPageviewSeries> = apiInstance.analyticsGetEventSeries(websiteId, startAt, endAt, unit, timezone, url, referrer, title, os, browser, device, country, region, city, tag, host, language, event)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EventsApi#analyticsGetEventSeries")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EventsApi#analyticsGetEventSeries")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |
| **unit** | **kotlin.String**|  | [optional] [enum: minute, hour, day, week, month, year] |
| **timezone** | **kotlin.String**|  | [optional] |
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

[**kotlin.collections.List&lt;AnalyticsPageviewSeries&gt;**](AnalyticsPageviewSeries.md)

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

<a id="analyticsGetEvents"></a>
# **analyticsGetEvents**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsGetEvents(websiteId, startAt, endAt, page, pageSize, orderBy, search)

Get paginated list of events

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EventsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsGetEvents(websiteId, startAt, endAt, page, pageSize, orderBy, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EventsApi#analyticsGetEvents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EventsApi#analyticsGetEvents")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **orderBy** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="s3GetBucketNotification"></a>
# **s3GetBucketNotification**
> S3GetBucketNotification200Response s3GetBucketNotification(bucket)

Get event notification config

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EventsApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
try {
    val result : S3GetBucketNotification200Response = apiInstance.s3GetBucketNotification(bucket)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EventsApi#s3GetBucketNotification")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EventsApi#s3GetBucketNotification")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bucket** | **kotlin.String**|  | |

### Return type

[**S3GetBucketNotification200Response**](S3GetBucketNotification200Response.md)

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

<a id="s3PutBucketNotification"></a>
# **s3PutBucketNotification**
> s3PutBucketNotification(bucket, s3GetBucketNotification200Response)

Set event notification config

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = EventsApi()
val bucket : kotlin.String = bucket_example // kotlin.String | 
val s3GetBucketNotification200Response : S3GetBucketNotification200Response =  // S3GetBucketNotification200Response | 
try {
    apiInstance.s3PutBucketNotification(bucket, s3GetBucketNotification200Response)
} catch (e: ClientException) {
    println("4xx response calling EventsApi#s3PutBucketNotification")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EventsApi#s3PutBucketNotification")
    e.printStackTrace()
}
```

### Parameters
| **bucket** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **s3GetBucketNotification200Response** | [**S3GetBucketNotification200Response**](S3GetBucketNotification200Response.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: Not defined

