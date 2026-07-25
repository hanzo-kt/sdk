# PlansApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**planGetPlanEntitlements**](PlansApi.md#planGetPlanEntitlements) | **GET** /v1/plans/entitlements/{id} | Entitlements for a plan |
| [**planGetPlanPolicy**](PlansApi.md#planGetPlanPolicy) | **GET** /v1/plans/policy | Plan policy |
| [**planGetPlanSchema**](PlansApi.md#planGetPlanSchema) | **GET** /v1/plans/schema | Entitlement schema |
| [**planGetPlanVocab**](PlansApi.md#planGetPlanVocab) | **GET** /v1/plans/vocab | Entitlement vocabulary |
| [**planListBlockchainPlans**](PlansApi.md#planListBlockchainPlans) | **GET** /v1/plans/blockchain | Blockchain plans |
| [**planListCloudPlans**](PlansApi.md#planListCloudPlans) | **GET** /v1/plans/cloud | Cloud plans |
| [**planListDnsPlans**](PlansApi.md#planListDnsPlans) | **GET** /v1/plans/dns | DNS plans |
| [**planListGpuPlans**](PlansApi.md#planListGpuPlans) | **GET** /v1/plans/gpu | GPU plans |
| [**planListPlanRegions**](PlansApi.md#planListPlanRegions) | **GET** /v1/plans/regions | Regions |
| [**planListPlanTools**](PlansApi.md#planListPlanTools) | **GET** /v1/plans/tools | Tools catalog |
| [**planListPlans**](PlansApi.md#planListPlans) | **GET** /v1/plans | The full plan catalog |
| [**planListStoragePlans**](PlansApi.md#planListStoragePlans) | **GET** /v1/plans/storage | Storage plans |
| [**planListSubscriptionPlans**](PlansApi.md#planListSubscriptionPlans) | **GET** /v1/plans/subscriptions | Subscription plans |
| [**planPlansHealth**](PlansApi.md#planPlansHealth) | **GET** /v1/plans/health | Health check |
| [**planResolvePlan**](PlansApi.md#planResolvePlan) | **GET** /v1/plans/resolve/{id} | Resolve a plan by id |


<a id="planGetPlanEntitlements"></a>
# **planGetPlanEntitlements**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; planGetPlanEntitlements(id)

Entitlements for a plan

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
val id : kotlin.String = id_example // kotlin.String | Plan id
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.planGetPlanEntitlements(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planGetPlanEntitlements")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planGetPlanEntitlements")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Plan id | |

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="planGetPlanPolicy"></a>
# **planGetPlanPolicy**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; planGetPlanPolicy()

Plan policy

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.planGetPlanPolicy()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planGetPlanPolicy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planGetPlanPolicy")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="planGetPlanSchema"></a>
# **planGetPlanSchema**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; planGetPlanSchema()

Entitlement schema

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.planGetPlanSchema()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planGetPlanSchema")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planGetPlanSchema")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="planGetPlanVocab"></a>
# **planGetPlanVocab**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; planGetPlanVocab()

Entitlement vocabulary

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.planGetPlanVocab()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planGetPlanVocab")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planGetPlanVocab")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="planListBlockchainPlans"></a>
# **planListBlockchainPlans**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; planListBlockchainPlans()

Blockchain plans

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.planListBlockchainPlans()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planListBlockchainPlans")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planListBlockchainPlans")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="planListCloudPlans"></a>
# **planListCloudPlans**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; planListCloudPlans()

Cloud plans

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.planListCloudPlans()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planListCloudPlans")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planListCloudPlans")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="planListDnsPlans"></a>
# **planListDnsPlans**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; planListDnsPlans()

DNS plans

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.planListDnsPlans()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planListDnsPlans")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planListDnsPlans")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="planListGpuPlans"></a>
# **planListGpuPlans**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; planListGpuPlans()

GPU plans

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.planListGpuPlans()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planListGpuPlans")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planListGpuPlans")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="planListPlanRegions"></a>
# **planListPlanRegions**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; planListPlanRegions()

Regions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.planListPlanRegions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planListPlanRegions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planListPlanRegions")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="planListPlanTools"></a>
# **planListPlanTools**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; planListPlanTools()

Tools catalog

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.planListPlanTools()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planListPlanTools")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planListPlanTools")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="planListPlans"></a>
# **planListPlans**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; planListPlans()

The full plan catalog

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.planListPlans()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planListPlans")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planListPlans")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="planListStoragePlans"></a>
# **planListStoragePlans**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; planListStoragePlans()

Storage plans

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.planListStoragePlans()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planListStoragePlans")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planListStoragePlans")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="planListSubscriptionPlans"></a>
# **planListSubscriptionPlans**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; planListSubscriptionPlans()

Subscription plans

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.planListSubscriptionPlans()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planListSubscriptionPlans")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planListSubscriptionPlans")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="planPlansHealth"></a>
# **planPlansHealth**
> PlanPlansHealth200Response planPlansHealth()

Health check

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
try {
    val result : PlanPlansHealth200Response = apiInstance.planPlansHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planPlansHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planPlansHealth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PlanPlansHealth200Response**](PlanPlansHealth200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="planResolvePlan"></a>
# **planResolvePlan**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; planResolvePlan(id)

Resolve a plan by id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlansApi()
val id : kotlin.String = id_example // kotlin.String | Plan id
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.planResolvePlan(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlansApi#planResolvePlan")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlansApi#planResolvePlan")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Plan id | |

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

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

