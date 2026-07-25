# IssuesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**trackerCreateIssue**](IssuesApi.md#trackerCreateIssue) | **POST** /v1/tracker/projects/{key}/issues | Create an issue |
| [**trackerDeleteIssue**](IssuesApi.md#trackerDeleteIssue) | **DELETE** /v1/tracker/projects/{key}/issues/{num} | Delete an issue |
| [**trackerGetIssue**](IssuesApi.md#trackerGetIssue) | **GET** /v1/tracker/projects/{key}/issues/{num} | Get an issue |
| [**trackerListIssues**](IssuesApi.md#trackerListIssues) | **GET** /v1/tracker/projects/{key}/issues | List issues (board/list) |
| [**trackerUpdateIssue**](IssuesApi.md#trackerUpdateIssue) | **PATCH** /v1/tracker/projects/{key}/issues/{num} | Update an issue |


<a id="trackerCreateIssue"></a>
# **trackerCreateIssue**
> TrackerIssue trackerCreateIssue(key, trackerCreateIssueRequest)

Create an issue

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IssuesApi()
val key : kotlin.String = key_example // kotlin.String | Project key
val trackerCreateIssueRequest : TrackerCreateIssueRequest =  // TrackerCreateIssueRequest | 
try {
    val result : TrackerIssue = apiInstance.trackerCreateIssue(key, trackerCreateIssueRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IssuesApi#trackerCreateIssue")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IssuesApi#trackerCreateIssue")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**| Project key | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **trackerCreateIssueRequest** | [**TrackerCreateIssueRequest**](TrackerCreateIssueRequest.md)|  | |

### Return type

[**TrackerIssue**](TrackerIssue.md)

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

<a id="trackerDeleteIssue"></a>
# **trackerDeleteIssue**
> trackerDeleteIssue(key, num)

Delete an issue

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IssuesApi()
val key : kotlin.String = key_example // kotlin.String | Project key
val num : kotlin.Int = 56 // kotlin.Int | Per-project issue number
try {
    apiInstance.trackerDeleteIssue(key, num)
} catch (e: ClientException) {
    println("4xx response calling IssuesApi#trackerDeleteIssue")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IssuesApi#trackerDeleteIssue")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**| Project key | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **num** | **kotlin.Int**| Per-project issue number | |

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="trackerGetIssue"></a>
# **trackerGetIssue**
> TrackerIssue trackerGetIssue(key, num)

Get an issue

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IssuesApi()
val key : kotlin.String = key_example // kotlin.String | Project key
val num : kotlin.Int = 56 // kotlin.Int | Per-project issue number
try {
    val result : TrackerIssue = apiInstance.trackerGetIssue(key, num)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IssuesApi#trackerGetIssue")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IssuesApi#trackerGetIssue")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**| Project key | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **num** | **kotlin.Int**| Per-project issue number | |

### Return type

[**TrackerIssue**](TrackerIssue.md)

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

<a id="trackerListIssues"></a>
# **trackerListIssues**
> kotlin.collections.List&lt;TrackerIssue&gt; trackerListIssues(key, status)

List issues (board/list)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IssuesApi()
val key : kotlin.String = key_example // kotlin.String | Project key
val status : TrackerIssueStatus =  // TrackerIssueStatus | Filter to one board column
try {
    val result : kotlin.collections.List<TrackerIssue> = apiInstance.trackerListIssues(key, status)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IssuesApi#trackerListIssues")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IssuesApi#trackerListIssues")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**| Project key | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | [**TrackerIssueStatus**](.md)| Filter to one board column | [optional] [enum: backlog, todo, in_progress, done, canceled] |

### Return type

[**kotlin.collections.List&lt;TrackerIssue&gt;**](TrackerIssue.md)

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

<a id="trackerUpdateIssue"></a>
# **trackerUpdateIssue**
> TrackerIssue trackerUpdateIssue(key, num, trackerUpdateIssueRequest)

Update an issue

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = IssuesApi()
val key : kotlin.String = key_example // kotlin.String | Project key
val num : kotlin.Int = 56 // kotlin.Int | Per-project issue number
val trackerUpdateIssueRequest : TrackerUpdateIssueRequest =  // TrackerUpdateIssueRequest | 
try {
    val result : TrackerIssue = apiInstance.trackerUpdateIssue(key, num, trackerUpdateIssueRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling IssuesApi#trackerUpdateIssue")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling IssuesApi#trackerUpdateIssue")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**| Project key | |
| **num** | **kotlin.Int**| Per-project issue number | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **trackerUpdateIssueRequest** | [**TrackerUpdateIssueRequest**](TrackerUpdateIssueRequest.md)|  | |

### Return type

[**TrackerIssue**](TrackerIssue.md)

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

