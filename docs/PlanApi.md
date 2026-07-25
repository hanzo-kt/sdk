# PlanApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**worldWorldLimits**](PlanApi.md#worldWorldLimits) | **GET** /v1/world/limits | Resolved World plan limits (contract echo) |


<a id="worldWorldLimits"></a>
# **worldWorldLimits**
> WorldWorldLimits200Response worldWorldLimits(plan)

Resolved World plan limits (contract echo)

Returns the Hanzo World enforcement limits for a plan, resolved from the @hanzo/plans catalog (the single source of truth) via the world.* entitlement vocabulary. Agents and the dashboard read this to self-config against the live catalog instead of hardcoding tier numbers. Defaults to world-free; degrades to the fail-closed Free floor on a catalog outage. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PlanApi()
val plan : kotlin.String = plan_example // kotlin.String | Plan id (world-free | world-pro | world-team | world-enterprise). Defaults to world-free.
try {
    val result : WorldWorldLimits200Response = apiInstance.worldWorldLimits(plan)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlanApi#worldWorldLimits")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlanApi#worldWorldLimits")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **plan** | **kotlin.String**| Plan id (world-free | world-pro | world-team | world-enterprise). Defaults to world-free. | [optional] [default to &quot;world-free&quot;] |

### Return type

[**WorldWorldLimits200Response**](WorldWorldLimits200Response.md)

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

