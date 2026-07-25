# MarketingApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**commerceCreateMarketingCampaign**](MarketingApi.md#commerceCreateMarketingCampaign) | **POST** /v1/commerce/marketing | Create marketing campaign |


<a id="commerceCreateMarketingCampaign"></a>
# **commerceCreateMarketingCampaign**
> kotlin.Any commerceCreateMarketingCampaign(body)

Create marketing campaign

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = MarketingApi()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.commerceCreateMarketingCampaign(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketingApi#commerceCreateMarketingCampaign")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketingApi#commerceCreateMarketingCampaign")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

