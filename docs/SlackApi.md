# SlackApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**integrationsSlackCommands**](SlackApi.md#integrationsSlackCommands) | **POST** /v1/integrations/slack/commands | Slack slash command webhook |
| [**integrationsSlackEvents**](SlackApi.md#integrationsSlackEvents) | **POST** /v1/integrations/slack/events | Slack Events API webhook |
| [**integrationsSlackLinkCallback**](SlackApi.md#integrationsSlackLinkCallback) | **GET** /v1/integrations/slack/link/callback | hanzo.id OIDC callback — bind Slack↔Hanzo (leg 3) |
| [**integrationsSlackLinkSlack**](SlackApi.md#integrationsSlackLinkSlack) | **GET** /v1/integrations/slack/link/slack | Slack sign-in callback (leg 2) |
| [**integrationsSlackLinkStart**](SlackApi.md#integrationsSlackLinkStart) | **GET** /v1/integrations/slack/link | Begin the per-user account link (leg 1 — Slack sign-in) |


<a id="integrationsSlackCommands"></a>
# **integrationsSlackCommands**
> integrationsSlackCommands(command, text, teamId, userId, channelId, responseUrl)

Slack slash command webhook

Public at the JWT layer; HMAC-verified inside the handler. Accepts the Slack &#x60;application/x-www-form-urlencoded&#x60; slash-command payload.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SlackApi()
val command : kotlin.String = command_example // kotlin.String | 
val text : kotlin.String = text_example // kotlin.String | 
val teamId : kotlin.String = teamId_example // kotlin.String | 
val userId : kotlin.String = userId_example // kotlin.String | 
val channelId : kotlin.String = channelId_example // kotlin.String | 
val responseUrl : kotlin.String = responseUrl_example // kotlin.String | 
try {
    apiInstance.integrationsSlackCommands(command, text, teamId, userId, channelId, responseUrl)
} catch (e: ClientException) {
    println("4xx response calling SlackApi#integrationsSlackCommands")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SlackApi#integrationsSlackCommands")
    e.printStackTrace()
}
```

### Parameters
| **command** | **kotlin.String**|  | [optional] |
| **text** | **kotlin.String**|  | [optional] |
| **teamId** | **kotlin.String**|  | [optional] |
| **userId** | **kotlin.String**|  | [optional] |
| **channelId** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **responseUrl** | **kotlin.String**|  | [optional] |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: Not defined

<a id="integrationsSlackEvents"></a>
# **integrationsSlackEvents**
> integrationsSlackEvents(integrationsSlackEventEnvelope)

Slack Events API webhook

Public at the JWT layer; authenticated inside the handler by HMAC-SHA256 over the raw body with the Slack signing secret. Handles the &#x60;url_verification&#x60; challenge and routes &#x60;app_mention&#x60;/&#x60;message&#x60; events to an on-behalf-of agent run.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SlackApi()
val integrationsSlackEventEnvelope : IntegrationsSlackEventEnvelope =  // IntegrationsSlackEventEnvelope | 
try {
    apiInstance.integrationsSlackEvents(integrationsSlackEventEnvelope)
} catch (e: ClientException) {
    println("4xx response calling SlackApi#integrationsSlackEvents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SlackApi#integrationsSlackEvents")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **integrationsSlackEventEnvelope** | [**IntegrationsSlackEventEnvelope**](IntegrationsSlackEventEnvelope.md)|  | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="integrationsSlackLinkCallback"></a>
# **integrationsSlackLinkCallback**
> kotlin.String integrationsSlackLinkCallback(code, state, error)

hanzo.id OIDC callback — bind Slack↔Hanzo (leg 3)

Reads the Slack-verified (team,user) from the &#x60;__Host-&#x60; link cookie, exchanges the OIDC code, and seals the refresh token into the workspace org&#39;s KMS namespace. Returns an HTML confirmation page.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SlackApi()
val code : kotlin.String = code_example // kotlin.String | 
val state : kotlin.String = state_example // kotlin.String | 
val error : kotlin.String = error_example // kotlin.String | 
try {
    val result : kotlin.String = apiInstance.integrationsSlackLinkCallback(code, state, error)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SlackApi#integrationsSlackLinkCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SlackApi#integrationsSlackLinkCallback")
    e.printStackTrace()
}
```

### Parameters
| **code** | **kotlin.String**|  | [optional] |
| **state** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **error** | **kotlin.String**|  | [optional] |

### Return type

**kotlin.String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="integrationsSlackLinkSlack"></a>
# **integrationsSlackLinkSlack**
> integrationsSlackLinkSlack(code, state, error)

Slack sign-in callback (leg 2)

Requires the leg-1 init cookie to match the sign-in state before exchanging the code; sets the &#x60;__Host-&#x60; link cookie and redirects to hanzo.id OIDC.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SlackApi()
val code : kotlin.String = code_example // kotlin.String | 
val state : kotlin.String = state_example // kotlin.String | 
val error : kotlin.String = error_example // kotlin.String | 
try {
    apiInstance.integrationsSlackLinkSlack(code, state, error)
} catch (e: ClientException) {
    println("4xx response calling SlackApi#integrationsSlackLinkSlack")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SlackApi#integrationsSlackLinkSlack")
    e.printStackTrace()
}
```

### Parameters
| **code** | **kotlin.String**|  | [optional] |
| **state** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **error** | **kotlin.String**|  | [optional] |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

<a id="integrationsSlackLinkStart"></a>
# **integrationsSlackLinkStart**
> integrationsSlackLinkStart(state)

Begin the per-user account link (leg 1 — Slack sign-in)

Sets a &#x60;__Host-&#x60; init cookie and redirects to Slack sign-in. State-authed (no bearer).

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SlackApi()
val state : kotlin.String = state_example // kotlin.String | Signed, single-use link state
try {
    apiInstance.integrationsSlackLinkStart(state)
} catch (e: ClientException) {
    println("4xx response calling SlackApi#integrationsSlackLinkStart")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SlackApi#integrationsSlackLinkStart")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **state** | **kotlin.String**| Signed, single-use link state | |

### Return type

null (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

