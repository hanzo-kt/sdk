# SubjectsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**mqGetSubjectInfo**](SubjectsApi.md#mqGetSubjectInfo) | **GET** /v1/mq/subjects/{subject}/info | Get subject info |
| [**mqListSubjects**](SubjectsApi.md#mqListSubjects) | **GET** /v1/mq/subjects | List active subjects |


<a id="mqGetSubjectInfo"></a>
# **mqGetSubjectInfo**
> MqSubjectInfo mqGetSubjectInfo(subject)

Get subject info

Returns detailed information about a specific subject, including subscriber count and message throughput. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SubjectsApi()
val subject : kotlin.String = subject_example // kotlin.String | 
try {
    val result : MqSubjectInfo = apiInstance.mqGetSubjectInfo(subject)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubjectsApi#mqGetSubjectInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubjectsApi#mqGetSubjectInfo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **subject** | **kotlin.String**|  | |

### Return type

[**MqSubjectInfo**](MqSubjectInfo.md)

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

<a id="mqListSubjects"></a>
# **mqListSubjects**
> MqListSubjects200Response mqListSubjects(limit, offset, filter)

List active subjects

Returns all active subjects visible to the authenticated account, with subscriber counts and message rates. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SubjectsApi()
val limit : kotlin.Int = 56 // kotlin.Int | Maximum number of items to return.
val offset : kotlin.Int = 56 // kotlin.Int | Number of items to skip.
val filter : kotlin.String = filter_example // kotlin.String | Subject filter pattern (supports wildcards).
try {
    val result : MqListSubjects200Response = apiInstance.mqListSubjects(limit, offset, filter)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SubjectsApi#mqListSubjects")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SubjectsApi#mqListSubjects")
    e.printStackTrace()
}
```

### Parameters
| **limit** | **kotlin.Int**| Maximum number of items to return. | [optional] [default to 100] |
| **offset** | **kotlin.Int**| Number of items to skip. | [optional] [default to 0] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **filter** | **kotlin.String**| Subject filter pattern (supports wildcards). | [optional] |

### Return type

[**MqListSubjects200Response**](MqListSubjects200Response.md)

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

