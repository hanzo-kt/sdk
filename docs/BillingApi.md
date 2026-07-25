# BillingApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**billingBillingBalance**](BillingApi.md#billingBillingBalance) | **GET** /v1/billing/balance | Prepaid credit balance |
| [**billingBillingGpuCharge**](BillingApi.md#billingBillingGpuCharge) | **POST** /v1/billing/gpu-charge | Prepay-only GPU charge |
| [**billingBillingGpuEligibility**](BillingApi.md#billingBillingGpuEligibility) | **GET** /v1/billing/gpu-eligibility | GPU launch eligibility gate |
| [**billingBillingPaymentMethods**](BillingApi.md#billingBillingPaymentMethods) | **GET** /v1/billing/payment-methods | Saved payment methods (masked) |
| [**billingBillingUsage**](BillingApi.md#billingBillingUsage) | **GET** /v1/billing/usage | Per-request usage ledger |
| [**platformBillingGetBalance**](BillingApi.md#platformBillingGetBalance) | **GET** /v1/platform/billing/getBalance | Get account balance |
| [**platformBillingGetPlans**](BillingApi.md#platformBillingGetPlans) | **GET** /v1/platform/billing/getPlans | List subscription plans |


<a id="billingBillingBalance"></a>
# **billingBillingBalance**
> BillingBalance billingBillingBalance(currency)

Prepaid credit balance

The org&#39;s prepaid credit balance in USD cents — the same wallet the gateway debits.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BillingApi()
val currency : kotlin.String = currency_example // kotlin.String | Optional currency filter (default usd)
try {
    val result : BillingBalance = apiInstance.billingBillingBalance(currency)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BillingApi#billingBillingBalance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BillingApi#billingBillingBalance")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **currency** | **kotlin.String**| Optional currency filter (default usd) | [optional] |

### Return type

[**BillingBalance**](BillingBalance.md)

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

<a id="billingBillingGpuCharge"></a>
# **billingBillingGpuCharge**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; billingBillingGpuCharge(billingGpuChargeRequest)

Prepay-only GPU charge

The prepay-only, card-required GPU debit against the caller&#39;s own org wallet. Commerce enforces both gates server-side; the subject is pinned server-side, so only the charge params ride the body. Commerce&#39;s status is forwarded verbatim. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BillingApi()
val billingGpuChargeRequest : BillingGpuChargeRequest =  // BillingGpuChargeRequest | 
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.billingBillingGpuCharge(billingGpuChargeRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BillingApi#billingBillingGpuCharge")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BillingApi#billingBillingGpuCharge")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **billingGpuChargeRequest** | [**BillingGpuChargeRequest**](BillingGpuChargeRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="billingBillingGpuEligibility"></a>
# **billingBillingGpuEligibility**
> BillingGpuEligibility billingBillingGpuEligibility(amountCents, minPrepaidCents, currency)

GPU launch eligibility gate

Read-only launch gate — reports prepaid availability and card-on-file so the launch UI can show the exact remedy.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BillingApi()
val amountCents : kotlin.Long = 789 // kotlin.Long | Immediate charge to test against
val minPrepaidCents : kotlin.Long = 789 // kotlin.Long | 24h-minimum prepaid floor
val currency : kotlin.String = currency_example // kotlin.String | 
try {
    val result : BillingGpuEligibility = apiInstance.billingBillingGpuEligibility(amountCents, minPrepaidCents, currency)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BillingApi#billingBillingGpuEligibility")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BillingApi#billingBillingGpuEligibility")
    e.printStackTrace()
}
```

### Parameters
| **amountCents** | **kotlin.Long**| Immediate charge to test against | [optional] |
| **minPrepaidCents** | **kotlin.Long**| 24h-minimum prepaid floor | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **currency** | **kotlin.String**|  | [optional] |

### Return type

[**BillingGpuEligibility**](BillingGpuEligibility.md)

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

<a id="billingBillingPaymentMethods"></a>
# **billingBillingPaymentMethods**
> BillingPaymentMethods billingBillingPaymentMethods()

Saved payment methods (masked)

The org&#39;s saved cards as commerce&#39;s masked descriptor (brand + last4 + expiry) — never a PAN/CVV/token.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BillingApi()
try {
    val result : BillingPaymentMethods = apiInstance.billingBillingPaymentMethods()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BillingApi#billingBillingPaymentMethods")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BillingApi#billingBillingPaymentMethods")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**BillingPaymentMethods**](BillingPaymentMethods.md)

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

<a id="billingBillingUsage"></a>
# **billingBillingUsage**
> BillingUsageLedger billingBillingUsage(start, end)

Per-request usage ledger

The raw per-request billing ledger (one row per billed call) for the caller&#39;s own org.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BillingApi()
val start : kotlin.String = start_example // kotlin.String | Optional server-side window start
val end : kotlin.String = end_example // kotlin.String | Optional server-side window end
try {
    val result : BillingUsageLedger = apiInstance.billingBillingUsage(start, end)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BillingApi#billingBillingUsage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BillingApi#billingBillingUsage")
    e.printStackTrace()
}
```

### Parameters
| **start** | **kotlin.String**| Optional server-side window start | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **end** | **kotlin.String**| Optional server-side window end | [optional] |

### Return type

[**BillingUsageLedger**](BillingUsageLedger.md)

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

<a id="platformBillingGetBalance"></a>
# **platformBillingGetBalance**
> PlatformTRPCResult platformBillingGetBalance()

Get account balance

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BillingApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformBillingGetBalance()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BillingApi#platformBillingGetBalance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BillingApi#platformBillingGetBalance")
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

<a id="platformBillingGetPlans"></a>
# **platformBillingGetPlans**
> PlatformTRPCResult platformBillingGetPlans()

List subscription plans

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = BillingApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformBillingGetPlans()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BillingApi#platformBillingGetPlans")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BillingApi#platformBillingGetPlans")
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

