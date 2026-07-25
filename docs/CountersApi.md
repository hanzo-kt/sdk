# CountersApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**commerceGetDailyDashboard**](CountersApi.md#commerceGetDailyDashboard) | **POST** /v1/commerce/counter/dashboard/daily | Get daily dashboard metrics |
| [**commerceGetProductCounters**](CountersApi.md#commerceGetProductCounters) | **GET** /v1/commerce/counter/product/{productid} | Get product counters |
| [**commerceGetToplineMetrics**](CountersApi.md#commerceGetToplineMetrics) | **GET** /v1/commerce/counter/topline | Get topline metrics |
| [**commerceSearchCounters**](CountersApi.md#commerceSearchCounters) | **POST** /v1/commerce/counter | Search counters |


<a id="commerceGetDailyDashboard"></a>
# **commerceGetDailyDashboard**
> kotlin.Any commerceGetDailyDashboard(commerceGetDailyDashboardRequest)

Get daily dashboard metrics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CountersApi()
val commerceGetDailyDashboardRequest : CommerceGetDailyDashboardRequest =  // CommerceGetDailyDashboardRequest | 
try {
    val result : kotlin.Any = apiInstance.commerceGetDailyDashboard(commerceGetDailyDashboardRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CountersApi#commerceGetDailyDashboard")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CountersApi#commerceGetDailyDashboard")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceGetDailyDashboardRequest** | [**CommerceGetDailyDashboardRequest**](CommerceGetDailyDashboardRequest.md)|  | [optional] |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="commerceGetProductCounters"></a>
# **commerceGetProductCounters**
> kotlin.Any commerceGetProductCounters(productid)

Get product counters

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CountersApi()
val productid : kotlin.String = productid_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.commerceGetProductCounters(productid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CountersApi#commerceGetProductCounters")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CountersApi#commerceGetProductCounters")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productid** | **kotlin.String**|  | |

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

<a id="commerceGetToplineMetrics"></a>
# **commerceGetToplineMetrics**
> kotlin.Any commerceGetToplineMetrics()

Get topline metrics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CountersApi()
try {
    val result : kotlin.Any = apiInstance.commerceGetToplineMetrics()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CountersApi#commerceGetToplineMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CountersApi#commerceGetToplineMetrics")
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

<a id="commerceSearchCounters"></a>
# **commerceSearchCounters**
> kotlin.Any commerceSearchCounters(commerceSearchCountersRequest)

Search counters

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CountersApi()
val commerceSearchCountersRequest : CommerceSearchCountersRequest =  // CommerceSearchCountersRequest | 
try {
    val result : kotlin.Any = apiInstance.commerceSearchCounters(commerceSearchCountersRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CountersApi#commerceSearchCounters")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CountersApi#commerceSearchCounters")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **commerceSearchCountersRequest** | [**CommerceSearchCountersRequest**](CommerceSearchCountersRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

