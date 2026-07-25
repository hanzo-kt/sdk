# ConsumerGroupsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**streamCommitOffsets**](ConsumerGroupsApi.md#streamCommitOffsets) | **PUT** /v1/stream/groups/{group_id}/offsets | Commit offsets |
| [**streamDeleteConsumerGroup**](ConsumerGroupsApi.md#streamDeleteConsumerGroup) | **DELETE** /v1/stream/groups/{group_id} | Delete a consumer group |
| [**streamGetConsumerGroup**](ConsumerGroupsApi.md#streamGetConsumerGroup) | **GET** /v1/stream/groups/{group_id} | Get consumer group details |
| [**streamGetGroupOffsets**](ConsumerGroupsApi.md#streamGetGroupOffsets) | **GET** /v1/stream/groups/{group_id}/offsets | Get committed offsets |
| [**streamListConsumerGroups**](ConsumerGroupsApi.md#streamListConsumerGroups) | **GET** /v1/stream/groups | List consumer groups |


<a id="streamCommitOffsets"></a>
# **streamCommitOffsets**
> streamCommitOffsets(groupId, streamGetGroupOffsets200Response)

Commit offsets

Manually commit offsets for a consumer group.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumerGroupsApi()
val groupId : kotlin.String = groupId_example // kotlin.String | 
val streamGetGroupOffsets200Response : StreamGetGroupOffsets200Response =  // StreamGetGroupOffsets200Response | 
try {
    apiInstance.streamCommitOffsets(groupId, streamGetGroupOffsets200Response)
} catch (e: ClientException) {
    println("4xx response calling ConsumerGroupsApi#streamCommitOffsets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumerGroupsApi#streamCommitOffsets")
    e.printStackTrace()
}
```

### Parameters
| **groupId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **streamGetGroupOffsets200Response** | [**StreamGetGroupOffsets200Response**](StreamGetGroupOffsets200Response.md)|  | |

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

<a id="streamDeleteConsumerGroup"></a>
# **streamDeleteConsumerGroup**
> streamDeleteConsumerGroup(groupId)

Delete a consumer group

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumerGroupsApi()
val groupId : kotlin.String = groupId_example // kotlin.String | 
try {
    apiInstance.streamDeleteConsumerGroup(groupId)
} catch (e: ClientException) {
    println("4xx response calling ConsumerGroupsApi#streamDeleteConsumerGroup")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumerGroupsApi#streamDeleteConsumerGroup")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **groupId** | **kotlin.String**|  | |

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
 - **Accept**: Not defined

<a id="streamGetConsumerGroup"></a>
# **streamGetConsumerGroup**
> StreamConsumerGroup streamGetConsumerGroup(groupId)

Get consumer group details

Returns consumer group state, members, and committed offsets with lag.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumerGroupsApi()
val groupId : kotlin.String = groupId_example // kotlin.String | 
try {
    val result : StreamConsumerGroup = apiInstance.streamGetConsumerGroup(groupId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConsumerGroupsApi#streamGetConsumerGroup")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumerGroupsApi#streamGetConsumerGroup")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **groupId** | **kotlin.String**|  | |

### Return type

[**StreamConsumerGroup**](StreamConsumerGroup.md)

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

<a id="streamGetGroupOffsets"></a>
# **streamGetGroupOffsets**
> StreamGetGroupOffsets200Response streamGetGroupOffsets(groupId, topic)

Get committed offsets

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumerGroupsApi()
val groupId : kotlin.String = groupId_example // kotlin.String | 
val topic : kotlin.String = topic_example // kotlin.String | Filter by topic
try {
    val result : StreamGetGroupOffsets200Response = apiInstance.streamGetGroupOffsets(groupId, topic)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConsumerGroupsApi#streamGetGroupOffsets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumerGroupsApi#streamGetGroupOffsets")
    e.printStackTrace()
}
```

### Parameters
| **groupId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **topic** | **kotlin.String**| Filter by topic | [optional] |

### Return type

[**StreamGetGroupOffsets200Response**](StreamGetGroupOffsets200Response.md)

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

<a id="streamListConsumerGroups"></a>
# **streamListConsumerGroups**
> StreamListConsumerGroups200Response streamListConsumerGroups()

List consumer groups

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConsumerGroupsApi()
try {
    val result : StreamListConsumerGroups200Response = apiInstance.streamListConsumerGroups()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConsumerGroupsApi#streamListConsumerGroups")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConsumerGroupsApi#streamListConsumerGroups")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**StreamListConsumerGroups200Response**](StreamListConsumerGroups200Response.md)

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

