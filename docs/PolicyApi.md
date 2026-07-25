# PolicyApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**pricingGetPricingPolicy**](PolicyApi.md#pricingGetPricingPolicy) | **GET** /v1/pricing/policy | Pricing policy and revenue sharing |


<a id="pricingGetPricingPolicy"></a>
# **pricingGetPricingPolicy**
> PricingPricingPolicy pricingGetPricingPolicy()

Pricing policy and revenue sharing

Returns the transparent pricing policy including markup rates, revenue sharing percentages, and free tier details. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PolicyApi()
try {
    val result : PricingPricingPolicy = apiInstance.pricingGetPricingPolicy()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PolicyApi#pricingGetPricingPolicy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PolicyApi#pricingGetPricingPolicy")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingPricingPolicy**](PricingPricingPolicy.md)

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

