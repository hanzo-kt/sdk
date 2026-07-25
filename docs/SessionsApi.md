# SessionsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**analyticsGetSession**](SessionsApi.md#analyticsGetSession) | **GET** /v1/analytics/websites/{websiteId}/sessions/{sessionId} | Get a single session by ID |
| [**analyticsGetSessionActivity**](SessionsApi.md#analyticsGetSessionActivity) | **GET** /v1/analytics/websites/{websiteId}/sessions/{sessionId}/activity | Get activity log for a session |
| [**analyticsGetSessionDataProperties**](SessionsApi.md#analyticsGetSessionDataProperties) | **GET** /v1/analytics/websites/{websiteId}/session-data/properties | Get distinct session data property names |
| [**analyticsGetSessionDataValues**](SessionsApi.md#analyticsGetSessionDataValues) | **GET** /v1/analytics/websites/{websiteId}/session-data/values | Get session data values for a property |
| [**analyticsGetSessionProperties**](SessionsApi.md#analyticsGetSessionProperties) | **GET** /v1/analytics/websites/{websiteId}/sessions/{sessionId}/properties | Get custom session data properties |
| [**analyticsGetSessionStats**](SessionsApi.md#analyticsGetSessionStats) | **GET** /v1/analytics/websites/{websiteId}/sessions/stats | Get aggregate session statistics |
| [**analyticsGetSessions**](SessionsApi.md#analyticsGetSessions) | **GET** /v1/analytics/websites/{websiteId}/sessions | Get paginated list of sessions |
| [**analyticsGetSessionsWeekly**](SessionsApi.md#analyticsGetSessionsWeekly) | **GET** /v1/analytics/websites/{websiteId}/sessions/weekly | Get weekly session breakdown |
| [**consoleGetSession**](SessionsApi.md#consoleGetSession) | **GET** /v1/console/sessions/{sessionId} | Get a session with its traces |
| [**consoleListSessions**](SessionsApi.md#consoleListSessions) | **GET** /v1/console/sessions | Get sessions |
| [**iamApiControllerAddSession**](SessionsApi.md#iamApiControllerAddSession) | **POST** /v1/iam/sessions | Api Controller Add Session |
| [**iamApiControllerDeleteSession**](SessionsApi.md#iamApiControllerDeleteSession) | **DELETE** /v1/iam/sessions/{id} | Api Controller Delete Session |
| [**iamApiControllerGetSessions**](SessionsApi.md#iamApiControllerGetSessions) | **GET** /v1/iam/sessions | Api Controller Get Sessions |
| [**iamApiControllerGetSingleSession**](SessionsApi.md#iamApiControllerGetSingleSession) | **GET** /v1/iam/sessions/{id} | Api Controller Get Single Session |
| [**iamApiControllerIsSessionDuplicated**](SessionsApi.md#iamApiControllerIsSessionDuplicated) | **GET** /v1/iam/is-session-duplicated | Api Controller Is Session Duplicated |
| [**iamApiControllerUpdateSession**](SessionsApi.md#iamApiControllerUpdateSession) | **PUT** /v1/iam/sessions/{id} | Api Controller Update Session |


<a id="analyticsGetSession"></a>
# **analyticsGetSession**
> AnalyticsSession analyticsGetSession(websiteId, sessionId)

Get a single session by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val sessionId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : AnalyticsSession = apiInstance.analyticsGetSession(websiteId, sessionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#analyticsGetSession")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#analyticsGetSession")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sessionId** | **java.util.UUID**|  | |

### Return type

[**AnalyticsSession**](AnalyticsSession.md)

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

<a id="analyticsGetSessionActivity"></a>
# **analyticsGetSessionActivity**
> kotlin.collections.List&lt;AnalyticsGetSessionActivity200ResponseInner&gt; analyticsGetSessionActivity(websiteId, sessionId, startAt, endAt)

Get activity log for a session

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val sessionId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
try {
    val result : kotlin.collections.List<AnalyticsGetSessionActivity200ResponseInner> = apiInstance.analyticsGetSessionActivity(websiteId, sessionId, startAt, endAt)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#analyticsGetSessionActivity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#analyticsGetSessionActivity")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **sessionId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |

### Return type

[**kotlin.collections.List&lt;AnalyticsGetSessionActivity200ResponseInner&gt;**](AnalyticsGetSessionActivity200ResponseInner.md)

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

<a id="analyticsGetSessionDataProperties"></a>
# **analyticsGetSessionDataProperties**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsGetSessionDataProperties(websiteId, startAt, endAt, propertyName)

Get distinct session data property names

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
val propertyName : kotlin.String = propertyName_example // kotlin.String | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsGetSessionDataProperties(websiteId, startAt, endAt, propertyName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#analyticsGetSessionDataProperties")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#analyticsGetSessionDataProperties")
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

<a id="analyticsGetSessionDataValues"></a>
# **analyticsGetSessionDataValues**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsGetSessionDataValues(websiteId, startAt, endAt, propertyName)

Get session data values for a property

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
val propertyName : kotlin.String = propertyName_example // kotlin.String | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsGetSessionDataValues(websiteId, startAt, endAt, propertyName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#analyticsGetSessionDataValues")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#analyticsGetSessionDataValues")
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

<a id="analyticsGetSessionProperties"></a>
# **analyticsGetSessionProperties**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsGetSessionProperties(websiteId, sessionId)

Get custom session data properties

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val sessionId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsGetSessionProperties(websiteId, sessionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#analyticsGetSessionProperties")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#analyticsGetSessionProperties")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sessionId** | **java.util.UUID**|  | |

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

<a id="analyticsGetSessionStats"></a>
# **analyticsGetSessionStats**
> kotlin.collections.Map&lt;kotlin.String, AnalyticsGetSessionStats200ResponseValue&gt; analyticsGetSessionStats(websiteId, startAt, endAt, url, referrer, title, os, browser, device, country, region, city, tag, host, language, event)

Get aggregate session statistics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
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
    val result : kotlin.collections.Map<kotlin.String, AnalyticsGetSessionStats200ResponseValue> = apiInstance.analyticsGetSessionStats(websiteId, startAt, endAt, url, referrer, title, os, browser, device, country, region, city, tag, host, language, event)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#analyticsGetSessionStats")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#analyticsGetSessionStats")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |
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

[**kotlin.collections.Map&lt;kotlin.String, AnalyticsGetSessionStats200ResponseValue&gt;**](AnalyticsGetSessionStats200ResponseValue.md)

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

<a id="analyticsGetSessions"></a>
# **analyticsGetSessions**
> kotlin.collections.List&lt;AnalyticsSession&gt; analyticsGetSessions(websiteId, startAt, endAt, page, pageSize, orderBy, search)

Get paginated list of sessions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<AnalyticsSession> = apiInstance.analyticsGetSessions(websiteId, startAt, endAt, page, pageSize, orderBy, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#analyticsGetSessions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#analyticsGetSessions")
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

[**kotlin.collections.List&lt;AnalyticsSession&gt;**](AnalyticsSession.md)

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

<a id="analyticsGetSessionsWeekly"></a>
# **analyticsGetSessionsWeekly**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsGetSessionsWeekly(websiteId, startAt, endAt, timezone, page, pageSize, orderBy, search)

Get weekly session breakdown

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
val timezone : kotlin.String = America/Los_Angeles // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsGetSessionsWeekly(websiteId, startAt, endAt, timezone, page, pageSize, orderBy, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#analyticsGetSessionsWeekly")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#analyticsGetSessionsWeekly")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |
| **timezone** | **kotlin.String**|  | [optional] |
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

<a id="consoleGetSession"></a>
# **consoleGetSession**
> ConsoleSessionWithTraces consoleGetSession(sessionId)

Get a session with its traces

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val sessionId : kotlin.String = sessionId_example // kotlin.String | 
try {
    val result : ConsoleSessionWithTraces = apiInstance.consoleGetSession(sessionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#consoleGetSession")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#consoleGetSession")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sessionId** | **kotlin.String**|  | |

### Return type

[**ConsoleSessionWithTraces**](ConsoleSessionWithTraces.md)

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

<a id="consoleListSessions"></a>
# **consoleListSessions**
> ConsoleListSessions200Response consoleListSessions(page, limit, fromTimestamp, toTimestamp, environment)

Get sessions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
val fromTimestamp : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val toTimestamp : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val environment : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
try {
    val result : ConsoleListSessions200Response = apiInstance.consoleListSessions(page, limit, fromTimestamp, toTimestamp, environment)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#consoleListSessions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#consoleListSessions")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| **limit** | **kotlin.Int**|  | [optional] [default to 50] |
| **fromTimestamp** | **java.time.OffsetDateTime**|  | [optional] |
| **toTimestamp** | **java.time.OffsetDateTime**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **environment** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] |

### Return type

[**ConsoleListSessions200Response**](ConsoleListSessions200Response.md)

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

<a id="iamApiControllerAddSession"></a>
# **iamApiControllerAddSession**
> IamControllersResponse iamApiControllerAddSession(iamObjectSession)

Api Controller Add Session

Add session for one user in one application. If there are other existing sessions, join the session into the list.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val iamObjectSession : IamObjectSession =  // IamObjectSession | The session object to add
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddSession(iamObjectSession)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#iamApiControllerAddSession")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#iamApiControllerAddSession")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectSession** | [**IamObjectSession**](IamObjectSession.md)| The session object to add | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerDeleteSession"></a>
# **iamApiControllerDeleteSession**
> IamControllersResponse iamApiControllerDeleteSession(id, iamObjectSession)

Api Controller Delete Session

Delete session for one user in one application.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectSession : IamObjectSession =  // IamObjectSession | The session object to delete
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteSession(id, iamObjectSession)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#iamApiControllerDeleteSession")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#iamApiControllerDeleteSession")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectSession** | [**IamObjectSession**](IamObjectSession.md)| The session object to delete | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerGetSessions"></a>
# **iamApiControllerGetSessions**
> kotlin.collections.List&lt;kotlin.String&gt; iamApiControllerGetSessions(owner)

Api Controller Get Sessions

Get organization user sessions.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val owner : kotlin.String = owner_example // kotlin.String | The organization name
try {
    val result : kotlin.collections.List<kotlin.String> = apiInstance.iamApiControllerGetSessions(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#iamApiControllerGetSessions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#iamApiControllerGetSessions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The organization name | |

### Return type

**kotlin.collections.List&lt;kotlin.String&gt;**

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

<a id="iamApiControllerGetSingleSession"></a>
# **iamApiControllerGetSingleSession**
> kotlin.collections.List&lt;kotlin.String&gt; iamApiControllerGetSingleSession(id, sessionPkId)

Api Controller Get Single Session

Get session for one user in one application.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val sessionPkId : kotlin.String = sessionPkId_example // kotlin.String | The session ID in format: organization/user/application (e.g., built-in/admin/app-built-in)
try {
    val result : kotlin.collections.List<kotlin.String> = apiInstance.iamApiControllerGetSingleSession(id, sessionPkId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#iamApiControllerGetSingleSession")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#iamApiControllerGetSingleSession")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sessionPkId** | **kotlin.String**| The session ID in format: organization/user/application (e.g., built-in/admin/app-built-in) | |

### Return type

**kotlin.collections.List&lt;kotlin.String&gt;**

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

<a id="iamApiControllerIsSessionDuplicated"></a>
# **iamApiControllerIsSessionDuplicated**
> kotlin.collections.List&lt;kotlin.String&gt; iamApiControllerIsSessionDuplicated(sessionPkId, sessionId)

Api Controller Is Session Duplicated

Check if there are other different sessions for one user in one application.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val sessionPkId : kotlin.String = sessionPkId_example // kotlin.String | The session ID in format: organization/user/application (e.g., built-in/admin/app-built-in)
val sessionId : kotlin.String = sessionId_example // kotlin.String | The specific session ID to check
try {
    val result : kotlin.collections.List<kotlin.String> = apiInstance.iamApiControllerIsSessionDuplicated(sessionPkId, sessionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#iamApiControllerIsSessionDuplicated")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#iamApiControllerIsSessionDuplicated")
    e.printStackTrace()
}
```

### Parameters
| **sessionPkId** | **kotlin.String**| The session ID in format: organization/user/application (e.g., built-in/admin/app-built-in) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sessionId** | **kotlin.String**| The specific session ID to check | |

### Return type

**kotlin.collections.List&lt;kotlin.String&gt;**

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

<a id="iamApiControllerUpdateSession"></a>
# **iamApiControllerUpdateSession**
> IamControllersResponse iamApiControllerUpdateSession(id, iamObjectSession)

Api Controller Update Session

Update session for one user in one application.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SessionsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectSession : IamObjectSession =  // IamObjectSession | The session object to update
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateSession(id, iamObjectSession)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SessionsApi#iamApiControllerUpdateSession")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SessionsApi#iamApiControllerUpdateSession")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectSession** | [**IamObjectSession**](IamObjectSession.md)| The session object to update | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

