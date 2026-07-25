# HealthApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**authzAuthzHealth**](HealthApi.md#authzAuthzHealth) | **GET** /v1/authz/health | Liveness probe |
| [**authzAuthzReadyz**](HealthApi.md#authzAuthzReadyz) | **GET** /v1/authz/readyz | Readiness probe |
| [**autoGetDocs**](HealthApi.md#autoGetDocs) | **GET** /v1/auto/docs | Get auto-generated OpenAPI documentation |
| [**autoGetHealth**](HealthApi.md#autoGetHealth) | **GET** /v1/auto/health | Health check |
| [**consoleGetHealth**](HealthApi.md#consoleGetHealth) | **GET** /v1/console/health | Check health of API and database |
| [**flowGetDocs**](HealthApi.md#flowGetDocs) | **GET** /v1/flow/docs | Get auto-generated OpenAPI documentation |
| [**flowGetHealth**](HealthApi.md#flowGetHealth) | **GET** /v1/flow/health | Health check |
| [**gatewayLivelinessCheck**](HealthApi.md#gatewayLivelinessCheck) | **GET** /v1/gateway/health/liveliness | Liveliness check |
| [**gatewayReadinessCheck**](HealthApi.md#gatewayReadinessCheck) | **GET** /v1/gateway/health/readiness | Readiness check |
| [**mqHealthCheck**](HealthApi.md#mqHealthCheck) | **GET** /v1/mq/health | Health check |
| [**mqServerInfo**](HealthApi.md#mqServerInfo) | **GET** /v1/mq/info | Server info |
| [**notifyNotifyHealth**](HealthApi.md#notifyNotifyHealth) | **GET** /v1/notify/health | Liveness probe |
| [**pricingTriggerSync**](HealthApi.md#pricingTriggerSync) | **POST** /v1/pricing/sync | Trigger manual sync |
| [**referralsReferralsHealth**](HealthApi.md#referralsReferralsHealth) | **GET** /v1/referrals/health | Liveness probe |
| [**streamHealthCheck**](HealthApi.md#streamHealthCheck) | **GET** /health | Health check |


<a id="authzAuthzHealth"></a>
# **authzAuthzHealth**
> AuthzAuthzHealth200Response authzAuthzHealth()

Liveness probe

Always served, no auth required. Returns a static status object.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    val result : AuthzAuthzHealth200Response = apiInstance.authzAuthzHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#authzAuthzHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#authzAuthzHealth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AuthzAuthzHealth200Response**](AuthzAuthzHealth200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="authzAuthzReadyz"></a>
# **authzAuthzReadyz**
> AuthzAuthzReadyz200Response authzAuthzReadyz()

Readiness probe

Always served, no auth required. Returns a static readiness object.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    val result : AuthzAuthzReadyz200Response = apiInstance.authzAuthzReadyz()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#authzAuthzReadyz")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#authzAuthzReadyz")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AuthzAuthzReadyz200Response**](AuthzAuthzReadyz200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="autoGetDocs"></a>
# **autoGetDocs**
> kotlin.Any autoGetDocs()

Get auto-generated OpenAPI documentation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    val result : kotlin.Any = apiInstance.autoGetDocs()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#autoGetDocs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#autoGetDocs")
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

<a id="autoGetHealth"></a>
# **autoGetHealth**
> kotlin.Any autoGetHealth()

Health check

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    val result : kotlin.Any = apiInstance.autoGetHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#autoGetHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#autoGetHealth")
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

<a id="consoleGetHealth"></a>
# **consoleGetHealth**
> ConsoleHealthResponse consoleGetHealth()

Check health of API and database

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    val result : ConsoleHealthResponse = apiInstance.consoleGetHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#consoleGetHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#consoleGetHealth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ConsoleHealthResponse**](ConsoleHealthResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="flowGetDocs"></a>
# **flowGetDocs**
> kotlin.Any flowGetDocs()

Get auto-generated OpenAPI documentation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    val result : kotlin.Any = apiInstance.flowGetDocs()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#flowGetDocs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#flowGetDocs")
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

<a id="flowGetHealth"></a>
# **flowGetHealth**
> kotlin.Any flowGetHealth()

Health check

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    val result : kotlin.Any = apiInstance.flowGetHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#flowGetHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#flowGetHealth")
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

<a id="gatewayLivelinessCheck"></a>
# **gatewayLivelinessCheck**
> kotlin.String gatewayLivelinessCheck()

Liveliness check

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    val result : kotlin.String = apiInstance.gatewayLivelinessCheck()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#gatewayLivelinessCheck")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#gatewayLivelinessCheck")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**kotlin.String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: text/plain

<a id="gatewayReadinessCheck"></a>
# **gatewayReadinessCheck**
> GatewayReadinessCheck200Response gatewayReadinessCheck()

Readiness check

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    val result : GatewayReadinessCheck200Response = apiInstance.gatewayReadinessCheck()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#gatewayReadinessCheck")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#gatewayReadinessCheck")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**GatewayReadinessCheck200Response**](GatewayReadinessCheck200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="mqHealthCheck"></a>
# **mqHealthCheck**
> MqHealthCheck200Response mqHealthCheck()

Health check

Returns service health status. Does not require authentication.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    val result : MqHealthCheck200Response = apiInstance.mqHealthCheck()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#mqHealthCheck")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#mqHealthCheck")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**MqHealthCheck200Response**](MqHealthCheck200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="mqServerInfo"></a>
# **mqServerInfo**
> MqServerInfo mqServerInfo()

Server info

Returns server information including version, cluster details, and JetStream status. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    val result : MqServerInfo = apiInstance.mqServerInfo()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#mqServerInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#mqServerInfo")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**MqServerInfo**](MqServerInfo.md)

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

<a id="notifyNotifyHealth"></a>
# **notifyNotifyHealth**
> NotifyHealthResponse notifyNotifyHealth()

Liveness probe

Returns a fixed health body. Mirrors notifyd&#39;s &#x60;GET /v1/notify/health&#x60; verbatim so existing probes keep working unchanged. Unauthenticated. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    val result : NotifyHealthResponse = apiInstance.notifyNotifyHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#notifyNotifyHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#notifyNotifyHealth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**NotifyHealthResponse**](NotifyHealthResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="pricingTriggerSync"></a>
# **pricingTriggerSync**
> PricingTriggerSync200Response pricingTriggerSync()

Trigger manual sync

Manually triggers a pricing data sync from upstream providers. Requires API key authentication. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    val result : PricingTriggerSync200Response = apiInstance.pricingTriggerSync()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#pricingTriggerSync")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#pricingTriggerSync")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingTriggerSync200Response**](PricingTriggerSync200Response.md)

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

<a id="referralsReferralsHealth"></a>
# **referralsReferralsHealth**
> referralsReferralsHealth()

Liveness probe

Auto-registered liveness probe (serve.go registers &#x60;GET /v1/referrals/health&#x60; for every mounted subsystem). Response body is not defined by this package. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    apiInstance.referralsReferralsHealth()
} catch (e: ClientException) {
    println("4xx response calling HealthApi#referralsReferralsHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#referralsReferralsHealth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="streamHealthCheck"></a>
# **streamHealthCheck**
> StreamHealthCheck200Response streamHealthCheck()

Health check

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = HealthApi()
try {
    val result : StreamHealthCheck200Response = apiInstance.streamHealthCheck()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling HealthApi#streamHealthCheck")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling HealthApi#streamHealthCheck")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**StreamHealthCheck200Response**](StreamHealthCheck200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

