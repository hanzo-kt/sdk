# InfrastructureApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**pricingGetComputePresets**](InfrastructureApi.md#pricingGetComputePresets) | **GET** /v1/pricing/compute/presets | Curated compute presets |
| [**pricingGetComputePricing**](InfrastructureApi.md#pricingGetComputePricing) | **GET** /v1/pricing/compute | Compute tiers |
| [**pricingGetFullPricing**](InfrastructureApi.md#pricingGetFullPricing) | **GET** /v1/pricing | Full pricing data |
| [**pricingListGpuTiers**](InfrastructureApi.md#pricingListGpuTiers) | **GET** /v1/pricing/gpu | GPU tier pricing |
| [**pricingListTools**](InfrastructureApi.md#pricingListTools) | **GET** /v1/pricing/tools | Tool pricing |


<a id="pricingGetComputePresets"></a>
# **pricingGetComputePresets**
> PricingGetComputePresets200Response pricingGetComputePresets()

Curated compute presets

Returns curated compute presets for the launch page.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = InfrastructureApi()
try {
    val result : PricingGetComputePresets200Response = apiInstance.pricingGetComputePresets()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InfrastructureApi#pricingGetComputePresets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InfrastructureApi#pricingGetComputePresets")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingGetComputePresets200Response**](PricingGetComputePresets200Response.md)

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

<a id="pricingGetComputePricing"></a>
# **pricingGetComputePricing**
> kotlin.Any pricingGetComputePricing()

Compute tiers

Returns infrastructure compute tier pricing with DO-backed sizes.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = InfrastructureApi()
try {
    val result : kotlin.Any = apiInstance.pricingGetComputePricing()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InfrastructureApi#pricingGetComputePricing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InfrastructureApi#pricingGetComputePricing")
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

<a id="pricingGetFullPricing"></a>
# **pricingGetFullPricing**
> PricingFullPricingResponse pricingGetFullPricing()

Full pricing data

Returns the complete pricing dataset including all AI models, tools, infrastructure, and cloud plans. Large response (~500KB). 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = InfrastructureApi()
try {
    val result : PricingFullPricingResponse = apiInstance.pricingGetFullPricing()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InfrastructureApi#pricingGetFullPricing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InfrastructureApi#pricingGetFullPricing")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingFullPricingResponse**](PricingFullPricingResponse.md)

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

<a id="pricingListGpuTiers"></a>
# **pricingListGpuTiers**
> PricingGpuTiersResponse pricingListGpuTiers()

GPU tier pricing

Returns available GPU tiers with VRAM specs and hourly pricing. Currently offers H100 GPU configurations. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = InfrastructureApi()
try {
    val result : PricingGpuTiersResponse = apiInstance.pricingListGpuTiers()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InfrastructureApi#pricingListGpuTiers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InfrastructureApi#pricingListGpuTiers")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingGpuTiersResponse**](PricingGpuTiersResponse.md)

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

<a id="pricingListTools"></a>
# **pricingListTools**
> PricingToolsResponse pricingListTools()

Tool pricing

Returns pricing for platform tools (Web Search, Code Interpreter, File Analysis, Image Generation, etc.). 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = InfrastructureApi()
try {
    val result : PricingToolsResponse = apiInstance.pricingListTools()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InfrastructureApi#pricingListTools")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InfrastructureApi#pricingListTools")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingToolsResponse**](PricingToolsResponse.md)

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

