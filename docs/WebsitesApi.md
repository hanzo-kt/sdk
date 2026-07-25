# WebsitesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**analyticsCreateWebsite**](WebsitesApi.md#analyticsCreateWebsite) | **POST** /v1/analytics/websites | Create a new website |
| [**analyticsDeleteWebsite**](WebsitesApi.md#analyticsDeleteWebsite) | **DELETE** /v1/analytics/websites/{websiteId} | Delete website |
| [**analyticsGetActiveVisitors**](WebsitesApi.md#analyticsGetActiveVisitors) | **GET** /v1/analytics/websites/{websiteId}/active | Get count of active visitors |
| [**analyticsGetWebsite**](WebsitesApi.md#analyticsGetWebsite) | **GET** /v1/analytics/websites/{websiteId} | Get website by ID |
| [**analyticsGetWebsiteDateRange**](WebsitesApi.md#analyticsGetWebsiteDateRange) | **GET** /v1/analytics/websites/{websiteId}/daterange | Get the date range of data available for a website |
| [**analyticsGetWebsiteValues**](WebsitesApi.md#analyticsGetWebsiteValues) | **GET** /v1/analytics/websites/{websiteId}/values | Get distinct values for a given column type |
| [**analyticsListWebsites**](WebsitesApi.md#analyticsListWebsites) | **GET** /v1/analytics/websites | List websites owned by current user |
| [**analyticsResetWebsite**](WebsitesApi.md#analyticsResetWebsite) | **POST** /v1/analytics/websites/{websiteId}/reset | Reset all data for a website |
| [**analyticsTransferWebsite**](WebsitesApi.md#analyticsTransferWebsite) | **POST** /v1/analytics/websites/{websiteId}/transfer | Transfer website ownership to another user or team |
| [**analyticsUpdateWebsite**](WebsitesApi.md#analyticsUpdateWebsite) | **POST** /v1/analytics/websites/{websiteId} | Update website |


<a id="analyticsCreateWebsite"></a>
# **analyticsCreateWebsite**
> AnalyticsWebsite analyticsCreateWebsite(analyticsCreateWebsiteRequest)

Create a new website

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebsitesApi()
val analyticsCreateWebsiteRequest : AnalyticsCreateWebsiteRequest =  // AnalyticsCreateWebsiteRequest | 
try {
    val result : AnalyticsWebsite = apiInstance.analyticsCreateWebsite(analyticsCreateWebsiteRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebsitesApi#analyticsCreateWebsite")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebsitesApi#analyticsCreateWebsite")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsCreateWebsiteRequest** | [**AnalyticsCreateWebsiteRequest**](AnalyticsCreateWebsiteRequest.md)|  | |

### Return type

[**AnalyticsWebsite**](AnalyticsWebsite.md)

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

<a id="analyticsDeleteWebsite"></a>
# **analyticsDeleteWebsite**
> kotlin.Any analyticsDeleteWebsite(websiteId)

Delete website

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebsitesApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.analyticsDeleteWebsite(websiteId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebsitesApi#analyticsDeleteWebsite")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebsitesApi#analyticsDeleteWebsite")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **websiteId** | **java.util.UUID**|  | |

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

<a id="analyticsGetActiveVisitors"></a>
# **analyticsGetActiveVisitors**
> AnalyticsGetActiveVisitors200Response analyticsGetActiveVisitors(websiteId)

Get count of active visitors

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebsitesApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : AnalyticsGetActiveVisitors200Response = apiInstance.analyticsGetActiveVisitors(websiteId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebsitesApi#analyticsGetActiveVisitors")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebsitesApi#analyticsGetActiveVisitors")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **websiteId** | **java.util.UUID**|  | |

### Return type

[**AnalyticsGetActiveVisitors200Response**](AnalyticsGetActiveVisitors200Response.md)

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

<a id="analyticsGetWebsite"></a>
# **analyticsGetWebsite**
> AnalyticsWebsite analyticsGetWebsite(websiteId)

Get website by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebsitesApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : AnalyticsWebsite = apiInstance.analyticsGetWebsite(websiteId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebsitesApi#analyticsGetWebsite")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebsitesApi#analyticsGetWebsite")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **websiteId** | **java.util.UUID**|  | |

### Return type

[**AnalyticsWebsite**](AnalyticsWebsite.md)

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

<a id="analyticsGetWebsiteDateRange"></a>
# **analyticsGetWebsiteDateRange**
> AnalyticsGetWebsiteDateRange200Response analyticsGetWebsiteDateRange(websiteId)

Get the date range of data available for a website

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebsitesApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : AnalyticsGetWebsiteDateRange200Response = apiInstance.analyticsGetWebsiteDateRange(websiteId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebsitesApi#analyticsGetWebsiteDateRange")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebsitesApi#analyticsGetWebsiteDateRange")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **websiteId** | **java.util.UUID**|  | |

### Return type

[**AnalyticsGetWebsiteDateRange200Response**](AnalyticsGetWebsiteDateRange200Response.md)

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

<a id="analyticsGetWebsiteValues"></a>
# **analyticsGetWebsiteValues**
> kotlin.collections.List&lt;kotlin.String&gt; analyticsGetWebsiteValues(websiteId, startAt, endAt, type, search)

Get distinct values for a given column type

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebsitesApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startAt : kotlin.Long = 789 // kotlin.Long | Start timestamp in milliseconds
val endAt : kotlin.Long = 789 // kotlin.Long | End timestamp in milliseconds
val type : kotlin.String = type_example // kotlin.String | Column type (e.g. browser, os, device, country, url, referrer, title, event, tag, language, region, city, host)
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<kotlin.String> = apiInstance.analyticsGetWebsiteValues(websiteId, startAt, endAt, type, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebsitesApi#analyticsGetWebsiteValues")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebsitesApi#analyticsGetWebsiteValues")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **startAt** | **kotlin.Long**| Start timestamp in milliseconds | |
| **endAt** | **kotlin.Long**| End timestamp in milliseconds | |
| **type** | **kotlin.String**| Column type (e.g. browser, os, device, country, url, referrer, title, event, tag, language, region, city, host) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **search** | **kotlin.String**|  | [optional] |

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

<a id="analyticsListWebsites"></a>
# **analyticsListWebsites**
> kotlin.collections.List&lt;AnalyticsWebsite&gt; analyticsListWebsites(page, pageSize, orderBy, search)

List websites owned by current user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebsitesApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<AnalyticsWebsite> = apiInstance.analyticsListWebsites(page, pageSize, orderBy, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebsitesApi#analyticsListWebsites")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebsitesApi#analyticsListWebsites")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **orderBy** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;AnalyticsWebsite&gt;**](AnalyticsWebsite.md)

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

<a id="analyticsResetWebsite"></a>
# **analyticsResetWebsite**
> kotlin.Any analyticsResetWebsite(websiteId)

Reset all data for a website

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebsitesApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.analyticsResetWebsite(websiteId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebsitesApi#analyticsResetWebsite")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebsitesApi#analyticsResetWebsite")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **websiteId** | **java.util.UUID**|  | |

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

<a id="analyticsTransferWebsite"></a>
# **analyticsTransferWebsite**
> AnalyticsWebsite analyticsTransferWebsite(websiteId, analyticsTransferWebsiteRequest)

Transfer website ownership to another user or team

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebsitesApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val analyticsTransferWebsiteRequest : AnalyticsTransferWebsiteRequest =  // AnalyticsTransferWebsiteRequest | 
try {
    val result : AnalyticsWebsite = apiInstance.analyticsTransferWebsite(websiteId, analyticsTransferWebsiteRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebsitesApi#analyticsTransferWebsite")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebsitesApi#analyticsTransferWebsite")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsTransferWebsiteRequest** | [**AnalyticsTransferWebsiteRequest**](AnalyticsTransferWebsiteRequest.md)|  | |

### Return type

[**AnalyticsWebsite**](AnalyticsWebsite.md)

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

<a id="analyticsUpdateWebsite"></a>
# **analyticsUpdateWebsite**
> AnalyticsWebsite analyticsUpdateWebsite(websiteId, analyticsUpdateWebsiteRequest)

Update website

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebsitesApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val analyticsUpdateWebsiteRequest : AnalyticsUpdateWebsiteRequest =  // AnalyticsUpdateWebsiteRequest | 
try {
    val result : AnalyticsWebsite = apiInstance.analyticsUpdateWebsite(websiteId, analyticsUpdateWebsiteRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebsitesApi#analyticsUpdateWebsite")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebsitesApi#analyticsUpdateWebsite")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsUpdateWebsiteRequest** | [**AnalyticsUpdateWebsiteRequest**](AnalyticsUpdateWebsiteRequest.md)|  | |

### Return type

[**AnalyticsWebsite**](AnalyticsWebsite.md)

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

