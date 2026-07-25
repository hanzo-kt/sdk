# CloudApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**pricingGetCloud**](CloudApi.md#pricingGetCloud) | **GET** /v1/pricing/cloud | Cloud VM plans, regions, and storage |
| [**pricingGetFullPricing**](CloudApi.md#pricingGetFullPricing) | **GET** /v1/pricing | Full pricing data |
| [**pricingGetStoragePricing**](CloudApi.md#pricingGetStoragePricing) | **GET** /v1/pricing/cloud/storage | Block storage pricing |
| [**pricingListCloudPlans**](CloudApi.md#pricingListCloudPlans) | **GET** /v1/pricing/cloud/plans | Cloud VM plans |
| [**pricingListCloudRegions**](CloudApi.md#pricingListCloudRegions) | **GET** /v1/pricing/cloud/regions | Available cloud regions |
| [**worldWorldCloudAnalytics**](CloudApi.md#worldWorldCloudAnalytics) | **GET** /v1/world/cloud/analytics | ADMIN. Web analytics aggregate — top pages/referrers/countries, live visitors (analytics.hanzo.ai). Requires an admin-org IAM bearer. |
| [**worldWorldCloudByoGpu**](CloudApi.md#worldWorldCloudByoGpu) | **GET** /v1/world/cloud/byo-gpu | Public BYO-GPU map data — connected GPU workers by region (real counts when a service token is wired server-side, else demo-flagged). No auth. |
| [**worldWorldCloudChainNodes**](CloudApi.md#worldWorldCloudChainNodes) | **GET** /v1/world/cloud/chain-nodes | Public blockchain-network map data — per-network block height, peer count, live flag, and modeled node positions (positionsModeled:true; counts are real, geo is illustrative). No auth. |
| [**worldWorldCloudFleet**](CloudApi.md#worldWorldCloudFleet) | **GET** /v1/world/cloud/fleet | ADMIN. Machines + GPUs grouped by provider/region (visor). Requires an admin-org IAM bearer; 401 without a token, 403 for non-admin. |
| [**worldWorldCloudLlm**](CloudApi.md#worldWorldCloudLlm) | **GET** /v1/world/cloud/llm | ADMIN. Platform LLM observability — per-model/per-org usage, tokens, cost, errors, trace latency (cloud /v1/admin/o11y). Requires an admin-org IAM bearer. |
| [**worldWorldCloudModels**](CloudApi.md#worldWorldCloudModels) | **GET** /v1/world/cloud/models | Public served-model catalog + scale (from the gateway /v1/models). No auth. |
| [**worldWorldCloudPulse**](CloudApi.md#worldWorldCloudPulse) | **GET** /v1/world/cloud-pulse | Public platform aggregate (SaaS variant). Anonymized counts; demo-flagged unless a service token is wired server-side. |
| [**worldWorldCloudServices**](CloudApi.md#worldWorldCloudServices) | **GET** /v1/world/cloud/services | ADMIN. Per-subsystem health + RED metrics (o11y). Requires an admin-org IAM bearer. |
| [**worldWorldCloudTraffic**](CloudApi.md#worldWorldCloudTraffic) | **GET** /v1/world/cloud/traffic | Public request-traffic arcs — country-level origin → nearest region, weight-normalized (real analytics when a service token is wired server-side, else demo-flagged). No auth. |


<a id="pricingGetCloud"></a>
# **pricingGetCloud**
> PricingCloudResponse pricingGetCloud()

Cloud VM plans, regions, and storage

Returns all cloud infrastructure pricing: VM plans, available deployment regions, and block storage rates. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CloudApi()
try {
    val result : PricingCloudResponse = apiInstance.pricingGetCloud()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CloudApi#pricingGetCloud")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CloudApi#pricingGetCloud")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingCloudResponse**](PricingCloudResponse.md)

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

val apiInstance = CloudApi()
try {
    val result : PricingFullPricingResponse = apiInstance.pricingGetFullPricing()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CloudApi#pricingGetFullPricing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CloudApi#pricingGetFullPricing")
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

<a id="pricingGetStoragePricing"></a>
# **pricingGetStoragePricing**
> PricingBlockStoragePricing pricingGetStoragePricing()

Block storage pricing

Returns per-GB/month pricing for block storage volumes.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CloudApi()
try {
    val result : PricingBlockStoragePricing = apiInstance.pricingGetStoragePricing()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CloudApi#pricingGetStoragePricing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CloudApi#pricingGetStoragePricing")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingBlockStoragePricing**](PricingBlockStoragePricing.md)

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

<a id="pricingListCloudPlans"></a>
# **pricingListCloudPlans**
> PricingCloudPlansResponse pricingListCloudPlans()

Cloud VM plans

Returns available cloud VM plans with specs and pricing. Plans range from $5/mo (Starter) to $3,999/mo (Ultra). All prices include zero egress fees. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CloudApi()
try {
    val result : PricingCloudPlansResponse = apiInstance.pricingListCloudPlans()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CloudApi#pricingListCloudPlans")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CloudApi#pricingListCloudPlans")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingCloudPlansResponse**](PricingCloudPlansResponse.md)

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

<a id="pricingListCloudRegions"></a>
# **pricingListCloudRegions**
> PricingCloudRegionsResponse pricingListCloudRegions()

Available cloud regions

Returns deployment regions with availability status.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CloudApi()
try {
    val result : PricingCloudRegionsResponse = apiInstance.pricingListCloudRegions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CloudApi#pricingListCloudRegions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CloudApi#pricingListCloudRegions")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingCloudRegionsResponse**](PricingCloudRegionsResponse.md)

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

<a id="worldWorldCloudAnalytics"></a>
# **worldWorldCloudAnalytics**
> kotlin.Any worldWorldCloudAnalytics()

ADMIN. Web analytics aggregate — top pages/referrers/countries, live visitors (analytics.hanzo.ai). Requires an admin-org IAM bearer.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CloudApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldCloudAnalytics()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CloudApi#worldWorldCloudAnalytics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CloudApi#worldWorldCloudAnalytics")
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

<a id="worldWorldCloudByoGpu"></a>
# **worldWorldCloudByoGpu**
> kotlin.Any worldWorldCloudByoGpu()

Public BYO-GPU map data — connected GPU workers by region (real counts when a service token is wired server-side, else demo-flagged). No auth.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CloudApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldCloudByoGpu()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CloudApi#worldWorldCloudByoGpu")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CloudApi#worldWorldCloudByoGpu")
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

<a id="worldWorldCloudChainNodes"></a>
# **worldWorldCloudChainNodes**
> kotlin.Any worldWorldCloudChainNodes()

Public blockchain-network map data — per-network block height, peer count, live flag, and modeled node positions (positionsModeled:true; counts are real, geo is illustrative). No auth.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CloudApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldCloudChainNodes()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CloudApi#worldWorldCloudChainNodes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CloudApi#worldWorldCloudChainNodes")
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

<a id="worldWorldCloudFleet"></a>
# **worldWorldCloudFleet**
> kotlin.Any worldWorldCloudFleet()

ADMIN. Machines + GPUs grouped by provider/region (visor). Requires an admin-org IAM bearer; 401 without a token, 403 for non-admin.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CloudApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldCloudFleet()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CloudApi#worldWorldCloudFleet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CloudApi#worldWorldCloudFleet")
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

<a id="worldWorldCloudLlm"></a>
# **worldWorldCloudLlm**
> kotlin.Any worldWorldCloudLlm(range)

ADMIN. Platform LLM observability — per-model/per-org usage, tokens, cost, errors, trace latency (cloud /v1/admin/o11y). Requires an admin-org IAM bearer.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CloudApi()
val range : kotlin.String = range_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.worldWorldCloudLlm(range)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CloudApi#worldWorldCloudLlm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CloudApi#worldWorldCloudLlm")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **range** | **kotlin.String**|  | [optional] [default to Range._24h] [enum: 24h, 7d, 30d] |

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

<a id="worldWorldCloudModels"></a>
# **worldWorldCloudModels**
> kotlin.Any worldWorldCloudModels()

Public served-model catalog + scale (from the gateway /v1/models). No auth.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CloudApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldCloudModels()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CloudApi#worldWorldCloudModels")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CloudApi#worldWorldCloudModels")
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

<a id="worldWorldCloudPulse"></a>
# **worldWorldCloudPulse**
> kotlin.Any worldWorldCloudPulse()

Public platform aggregate (SaaS variant). Anonymized counts; demo-flagged unless a service token is wired server-side.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CloudApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldCloudPulse()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CloudApi#worldWorldCloudPulse")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CloudApi#worldWorldCloudPulse")
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

<a id="worldWorldCloudServices"></a>
# **worldWorldCloudServices**
> kotlin.Any worldWorldCloudServices()

ADMIN. Per-subsystem health + RED metrics (o11y). Requires an admin-org IAM bearer.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CloudApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldCloudServices()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CloudApi#worldWorldCloudServices")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CloudApi#worldWorldCloudServices")
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

<a id="worldWorldCloudTraffic"></a>
# **worldWorldCloudTraffic**
> kotlin.Any worldWorldCloudTraffic()

Public request-traffic arcs — country-level origin → nearest region, weight-normalized (real analytics when a service token is wired server-side, else demo-flagged). No auth.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = CloudApi()
try {
    val result : kotlin.Any = apiInstance.worldWorldCloudTraffic()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CloudApi#worldWorldCloudTraffic")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CloudApi#worldWorldCloudTraffic")
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

