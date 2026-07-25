# SendApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**notifyNotifySend**](SendApi.md#notifyNotifySend) | **POST** /v1/notify/send | Send a notification (generic channel) |
| [**notifyNotifySendEmail**](SendApi.md#notifyNotifySendEmail) | **POST** /v1/notify/send/email | Send an email notification |
| [**notifyNotifySendSms**](SendApi.md#notifyNotifySendSms) | **POST** /v1/notify/send/sms | Send an SMS notification |


<a id="notifyNotifySend"></a>
# **notifyNotifySend**
> NotifyNotifySend200Response notifyNotifySend(sync, notifySendRequest)

Send a notification (generic channel)

Synchronously delivers a notification. The channel is read from the request body (&#x60;channel: \&quot;sms\&quot;|\&quot;email\&quot;&#x60;). Only &#x60;sms&#x60; and &#x60;email&#x60; are supported by the cloud fold.  &#x60;sync&#x3D;true&#x60; is REQUIRED. Without it the request fails closed with &#x60;503&#x60; (async dispatch is not available in the fold).  The org scope is taken from the validated principal&#39;s tenant, never from a client-supplied header. The provider is chosen from configured KMS credentials unless &#x60;provider&#x60; pins one explicitly.  RESPONSE SHAPE — for a single recipient the body is a bare &#x60;SendResponse&#x60;. For multiple recipients the body is &#x60;{\&quot;items\&quot;: [SendResponse, ...]}&#x60;, one entry per recipient. A per-recipient terminal delivery failure is reported as a &#x60;200&#x60; with &#x60;status: \&quot;failed\&quot;&#x60; and an &#x60;error&#x60; message, NOT as an HTTP error. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SendApi()
val sync : kotlin.String = sync_example // kotlin.String | Must be `true`. Async dispatch is not available in the cloud fold; any other value yields `503`. 
val notifySendRequest : NotifySendRequest = {"to":["+15551234567"],"channel":"sms","event":"iam.otp_sent","template_vars":{"otp":"482913","recipient":"+15551234567","app":"Hanzo"}} // NotifySendRequest | 
try {
    val result : NotifyNotifySend200Response = apiInstance.notifyNotifySend(sync, notifySendRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SendApi#notifyNotifySend")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SendApi#notifyNotifySend")
    e.printStackTrace()
}
```

### Parameters
| **sync** | **kotlin.String**| Must be &#x60;true&#x60;. Async dispatch is not available in the cloud fold; any other value yields &#x60;503&#x60;.  | [enum: true] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **notifySendRequest** | [**NotifySendRequest**](NotifySendRequest.md)|  | |

### Return type

[**NotifyNotifySend200Response**](NotifyNotifySend200Response.md)

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

<a id="notifyNotifySendEmail"></a>
# **notifyNotifySendEmail**
> NotifyNotifySend200Response notifyNotifySendEmail(sync, notifySendRequest)

Send an email notification

Convenience route that pins &#x60;channel: email&#x60;. Any &#x60;channel&#x60; in the body is overridden. Otherwise identical to &#x60;POST /v1/notify/send&#x60; — &#x60;sync&#x3D;true&#x60; required, org derived from the validated principal, single vs. list response shape. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SendApi()
val sync : kotlin.String = sync_example // kotlin.String | Must be `true`; otherwise `503`.
val notifySendRequest : NotifySendRequest = {"to":["user@example.com"],"subject":"Welcome","body":"Thanks for signing up."} // NotifySendRequest | 
try {
    val result : NotifyNotifySend200Response = apiInstance.notifyNotifySendEmail(sync, notifySendRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SendApi#notifyNotifySendEmail")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SendApi#notifyNotifySendEmail")
    e.printStackTrace()
}
```

### Parameters
| **sync** | **kotlin.String**| Must be &#x60;true&#x60;; otherwise &#x60;503&#x60;. | [enum: true] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **notifySendRequest** | [**NotifySendRequest**](NotifySendRequest.md)|  | |

### Return type

[**NotifyNotifySend200Response**](NotifyNotifySend200Response.md)

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

<a id="notifyNotifySendSms"></a>
# **notifyNotifySendSms**
> NotifyNotifySend200Response notifyNotifySendSms(sync, notifySendRequest)

Send an SMS notification

Convenience route that pins &#x60;channel: sms&#x60;. Any &#x60;channel&#x60; in the body is overridden. Otherwise identical to &#x60;POST /v1/notify/send&#x60; — &#x60;sync&#x3D;true&#x60; required, org derived from the validated principal, single vs. list response shape. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SendApi()
val sync : kotlin.String = sync_example // kotlin.String | Must be `true`; otherwise `503`.
val notifySendRequest : NotifySendRequest = {"to":["+15551234567"],"event":"iam.otp_sent","template_vars":{"otp":"482913","app":"Hanzo"}} // NotifySendRequest | 
try {
    val result : NotifyNotifySend200Response = apiInstance.notifyNotifySendSms(sync, notifySendRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SendApi#notifyNotifySendSms")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SendApi#notifyNotifySendSms")
    e.printStackTrace()
}
```

### Parameters
| **sync** | **kotlin.String**| Must be &#x60;true&#x60;; otherwise &#x60;503&#x60;. | [enum: true] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **notifySendRequest** | [**NotifySendRequest**](NotifySendRequest.md)|  | |

### Return type

[**NotifyNotifySend200Response**](NotifyNotifySend200Response.md)

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

