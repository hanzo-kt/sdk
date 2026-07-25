# ActivityAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerGetActivities**](ActivityAPIApi.md#cloudApiControllerGetActivities) | **GET** /v1/cloud/get-activities | Api Controller Get Activities |
| [**nexusGetActivities**](ActivityAPIApi.md#nexusGetActivities) | **GET** /v1/nexus/get-activities | get Activities |


<a id="cloudApiControllerGetActivities"></a>
# **cloudApiControllerGetActivities**
> kotlin.collections.List&lt;CloudObjectActivity&gt; cloudApiControllerGetActivities(days)

Api Controller Get Activities

get activities

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ActivityAPIApi()
val days : kotlin.String = days_example // kotlin.String | days count
try {
    val result : kotlin.collections.List<CloudObjectActivity> = apiInstance.cloudApiControllerGetActivities(days)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityAPIApi#cloudApiControllerGetActivities")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityAPIApi#cloudApiControllerGetActivities")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **days** | **kotlin.String**| days count | |

### Return type

[**kotlin.collections.List&lt;CloudObjectActivity&gt;**](CloudObjectActivity.md)

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

<a id="nexusGetActivities"></a>
# **nexusGetActivities**
> kotlin.collections.List&lt;NexusActivity&gt; nexusGetActivities(days)

get Activities

Get activities

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ActivityAPIApi()
val days : kotlin.String = days_example // kotlin.String | Number of days
try {
    val result : kotlin.collections.List<NexusActivity> = apiInstance.nexusGetActivities(days)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityAPIApi#nexusGetActivities")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityAPIApi#nexusGetActivities")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **days** | **kotlin.String**| Number of days | |

### Return type

[**kotlin.collections.List&lt;NexusActivity&gt;**](NexusActivity.md)

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

