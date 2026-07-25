# BannerApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatGetBanner**](BannerApi.md#chatGetBanner) | **GET** /v1/chat/banner | Get server announcement banner |


<a id="chatGetBanner"></a>
# **chatGetBanner**
> kotlin.Any chatGetBanner()

Get server announcement banner

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BannerApi()
try {
    val result : kotlin.Any = apiInstance.chatGetBanner()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BannerApi#chatGetBanner")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BannerApi#chatGetBanner")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

