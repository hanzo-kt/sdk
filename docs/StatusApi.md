# StatusApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**observeGetStatus**](StatusApi.md#observeGetStatus) | **GET** /v1/o11y/status | Live health status for a product |


<a id="observeGetStatus"></a>
# **observeGetStatus**
> ObserveStatusResponse observeGetStatus(product)

Live health status for a product

Returns a live health signal for a product: an in-cluster health probe (measured latency, &#x60;/health&#x60; then &#x60;/healthz&#x60;) corroborated by the VictoriaMetrics &#x60;up{service}&#x60; scrape gauge. &#x60;up&#x60; is set by the probe when it succeeds, else by the scrape gauge, else false. Status is infra-level (no per-org data) but still requires a validated principal. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = StatusApi()
val product : kotlin.String = product_example // kotlin.String | Console product slug. Must match `^[a-z0-9][a-z0-9._-]{0,62}$`.
try {
    val result : ObserveStatusResponse = apiInstance.observeGetStatus(product)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StatusApi#observeGetStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StatusApi#observeGetStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **product** | **kotlin.String**| Console product slug. Must match &#x60;^[a-z0-9][a-z0-9._-]{0,62}$&#x60;. | |

### Return type

[**ObserveStatusResponse**](ObserveStatusResponse.md)

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

