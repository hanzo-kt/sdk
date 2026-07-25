# NotificationApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**platformNotificationAll**](NotificationApi.md#platformNotificationAll) | **GET** /v1/platform/notification/all | List notification channels (admin) |


<a id="platformNotificationAll"></a>
# **platformNotificationAll**
> PlatformTRPCResult platformNotificationAll()

List notification channels (admin)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = NotificationApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformNotificationAll()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NotificationApi#platformNotificationAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NotificationApi#platformNotificationAll")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

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

