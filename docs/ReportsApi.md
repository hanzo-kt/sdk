# ReportsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**analyticsCreateReport**](ReportsApi.md#analyticsCreateReport) | **POST** /v1/analytics/reports | Create a new report |
| [**analyticsDeleteReport**](ReportsApi.md#analyticsDeleteReport) | **DELETE** /v1/analytics/reports/{reportId} | Delete a report |
| [**analyticsGetReport**](ReportsApi.md#analyticsGetReport) | **GET** /v1/analytics/reports/{reportId} | Get a report by ID |
| [**analyticsGetRevenueValues**](ReportsApi.md#analyticsGetRevenueValues) | **GET** /v1/analytics/reports/revenue | Get available revenue values for a website |
| [**analyticsGetWebsiteReports**](ReportsApi.md#analyticsGetWebsiteReports) | **GET** /v1/analytics/websites/{websiteId}/reports | List reports for a specific website |
| [**analyticsListReports**](ReportsApi.md#analyticsListReports) | **GET** /v1/analytics/reports | List reports, optionally filtered by website or team |
| [**analyticsRunAttributionReport**](ReportsApi.md#analyticsRunAttributionReport) | **POST** /v1/analytics/reports/attribution | Run an attribution report |
| [**analyticsRunFunnelReport**](ReportsApi.md#analyticsRunFunnelReport) | **POST** /v1/analytics/reports/funnel | Run a funnel report |
| [**analyticsRunGoalsReport**](ReportsApi.md#analyticsRunGoalsReport) | **POST** /v1/analytics/reports/goals | Run a goals report |
| [**analyticsRunInsightsReport**](ReportsApi.md#analyticsRunInsightsReport) | **POST** /v1/analytics/reports/insights | Run an insights report |
| [**analyticsRunJourneyReport**](ReportsApi.md#analyticsRunJourneyReport) | **POST** /v1/analytics/reports/journey | Run a user journey report |
| [**analyticsRunRetentionReport**](ReportsApi.md#analyticsRunRetentionReport) | **POST** /v1/analytics/reports/retention | Run a retention report |
| [**analyticsRunRevenueReport**](ReportsApi.md#analyticsRunRevenueReport) | **POST** /v1/analytics/reports/revenue | Run a revenue report |
| [**analyticsRunUtmReport**](ReportsApi.md#analyticsRunUtmReport) | **POST** /v1/analytics/reports/utm | Run a UTM report |
| [**analyticsUpdateReport**](ReportsApi.md#analyticsUpdateReport) | **POST** /v1/analytics/reports/{reportId} | Update a report |


<a id="analyticsCreateReport"></a>
# **analyticsCreateReport**
> AnalyticsReport analyticsCreateReport(analyticsCreateReportRequest)

Create a new report

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val analyticsCreateReportRequest : AnalyticsCreateReportRequest =  // AnalyticsCreateReportRequest | 
try {
    val result : AnalyticsReport = apiInstance.analyticsCreateReport(analyticsCreateReportRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsCreateReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsCreateReport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsCreateReportRequest** | [**AnalyticsCreateReportRequest**](AnalyticsCreateReportRequest.md)|  | |

### Return type

[**AnalyticsReport**](AnalyticsReport.md)

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

<a id="analyticsDeleteReport"></a>
# **analyticsDeleteReport**
> kotlin.Any analyticsDeleteReport(reportId)

Delete a report

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val reportId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.analyticsDeleteReport(reportId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsDeleteReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsDeleteReport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **reportId** | **java.util.UUID**|  | |

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

<a id="analyticsGetReport"></a>
# **analyticsGetReport**
> AnalyticsReport analyticsGetReport(reportId)

Get a report by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val reportId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : AnalyticsReport = apiInstance.analyticsGetReport(reportId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsGetReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsGetReport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **reportId** | **java.util.UUID**|  | |

### Return type

[**AnalyticsReport**](AnalyticsReport.md)

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

<a id="analyticsGetRevenueValues"></a>
# **analyticsGetRevenueValues**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsGetRevenueValues(websiteId, startDate, endDate)

Get available revenue values for a website

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val startDate : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val endDate : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsGetRevenueValues(websiteId, startDate, endDate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsGetRevenueValues")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsGetRevenueValues")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **startDate** | **java.time.OffsetDateTime**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **endDate** | **java.time.OffsetDateTime**|  | |

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

<a id="analyticsGetWebsiteReports"></a>
# **analyticsGetWebsiteReports**
> kotlin.collections.List&lt;AnalyticsReport&gt; analyticsGetWebsiteReports(websiteId, page, pageSize, orderBy, search)

List reports for a specific website

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<AnalyticsReport> = apiInstance.analyticsGetWebsiteReports(websiteId, page, pageSize, orderBy, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsGetWebsiteReports")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsGetWebsiteReports")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **orderBy** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;AnalyticsReport&gt;**](AnalyticsReport.md)

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

<a id="analyticsListReports"></a>
# **analyticsListReports**
> kotlin.collections.List&lt;AnalyticsReport&gt; analyticsListReports(websiteId, teamId, page, pageSize, orderBy, search)

List reports, optionally filtered by website or team

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val websiteId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val teamId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderBy : kotlin.String = orderBy_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<AnalyticsReport> = apiInstance.analyticsListReports(websiteId, teamId, page, pageSize, orderBy, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsListReports")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsListReports")
    e.printStackTrace()
}
```

### Parameters
| **websiteId** | **java.util.UUID**|  | [optional] |
| **teamId** | **java.util.UUID**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **orderBy** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;AnalyticsReport&gt;**](AnalyticsReport.md)

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

<a id="analyticsRunAttributionReport"></a>
# **analyticsRunAttributionReport**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsRunAttributionReport(analyticsRunAttributionReportRequest)

Run an attribution report

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val analyticsRunAttributionReportRequest : AnalyticsRunAttributionReportRequest =  // AnalyticsRunAttributionReportRequest | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsRunAttributionReport(analyticsRunAttributionReportRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsRunAttributionReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsRunAttributionReport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsRunAttributionReportRequest** | [**AnalyticsRunAttributionReportRequest**](AnalyticsRunAttributionReportRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="analyticsRunFunnelReport"></a>
# **analyticsRunFunnelReport**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsRunFunnelReport(analyticsRunFunnelReportRequest)

Run a funnel report

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val analyticsRunFunnelReportRequest : AnalyticsRunFunnelReportRequest =  // AnalyticsRunFunnelReportRequest | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsRunFunnelReport(analyticsRunFunnelReportRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsRunFunnelReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsRunFunnelReport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsRunFunnelReportRequest** | [**AnalyticsRunFunnelReportRequest**](AnalyticsRunFunnelReportRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="analyticsRunGoalsReport"></a>
# **analyticsRunGoalsReport**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsRunGoalsReport(analyticsRunGoalsReportRequest)

Run a goals report

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val analyticsRunGoalsReportRequest : AnalyticsRunGoalsReportRequest =  // AnalyticsRunGoalsReportRequest | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsRunGoalsReport(analyticsRunGoalsReportRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsRunGoalsReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsRunGoalsReport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsRunGoalsReportRequest** | [**AnalyticsRunGoalsReportRequest**](AnalyticsRunGoalsReportRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="analyticsRunInsightsReport"></a>
# **analyticsRunInsightsReport**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsRunInsightsReport(analyticsRunInsightsReportRequest)

Run an insights report

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val analyticsRunInsightsReportRequest : AnalyticsRunInsightsReportRequest =  // AnalyticsRunInsightsReportRequest | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsRunInsightsReport(analyticsRunInsightsReportRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsRunInsightsReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsRunInsightsReport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsRunInsightsReportRequest** | [**AnalyticsRunInsightsReportRequest**](AnalyticsRunInsightsReportRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="analyticsRunJourneyReport"></a>
# **analyticsRunJourneyReport**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsRunJourneyReport(analyticsRunJourneyReportRequest)

Run a user journey report

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val analyticsRunJourneyReportRequest : AnalyticsRunJourneyReportRequest =  // AnalyticsRunJourneyReportRequest | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsRunJourneyReport(analyticsRunJourneyReportRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsRunJourneyReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsRunJourneyReport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsRunJourneyReportRequest** | [**AnalyticsRunJourneyReportRequest**](AnalyticsRunJourneyReportRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="analyticsRunRetentionReport"></a>
# **analyticsRunRetentionReport**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsRunRetentionReport(analyticsRunRetentionReportRequest)

Run a retention report

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val analyticsRunRetentionReportRequest : AnalyticsRunRetentionReportRequest =  // AnalyticsRunRetentionReportRequest | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsRunRetentionReport(analyticsRunRetentionReportRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsRunRetentionReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsRunRetentionReport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsRunRetentionReportRequest** | [**AnalyticsRunRetentionReportRequest**](AnalyticsRunRetentionReportRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="analyticsRunRevenueReport"></a>
# **analyticsRunRevenueReport**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsRunRevenueReport(analyticsRunRevenueReportRequest)

Run a revenue report

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val analyticsRunRevenueReportRequest : AnalyticsRunRevenueReportRequest =  // AnalyticsRunRevenueReportRequest | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsRunRevenueReport(analyticsRunRevenueReportRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsRunRevenueReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsRunRevenueReport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsRunRevenueReportRequest** | [**AnalyticsRunRevenueReportRequest**](AnalyticsRunRevenueReportRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="analyticsRunUtmReport"></a>
# **analyticsRunUtmReport**
> kotlin.collections.List&lt;kotlin.Any&gt; analyticsRunUtmReport(analyticsRunUtmReportRequest)

Run a UTM report

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val analyticsRunUtmReportRequest : AnalyticsRunUtmReportRequest =  // AnalyticsRunUtmReportRequest | 
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.analyticsRunUtmReport(analyticsRunUtmReportRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsRunUtmReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsRunUtmReport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsRunUtmReportRequest** | [**AnalyticsRunUtmReportRequest**](AnalyticsRunUtmReportRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="analyticsUpdateReport"></a>
# **analyticsUpdateReport**
> AnalyticsReport analyticsUpdateReport(reportId, analyticsCreateReportRequest)

Update a report

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ReportsApi()
val reportId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val analyticsCreateReportRequest : AnalyticsCreateReportRequest =  // AnalyticsCreateReportRequest | 
try {
    val result : AnalyticsReport = apiInstance.analyticsUpdateReport(reportId, analyticsCreateReportRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#analyticsUpdateReport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#analyticsUpdateReport")
    e.printStackTrace()
}
```

### Parameters
| **reportId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **analyticsCreateReportRequest** | [**AnalyticsCreateReportRequest**](AnalyticsCreateReportRequest.md)|  | |

### Return type

[**AnalyticsReport**](AnalyticsReport.md)

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

