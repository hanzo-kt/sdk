# ConnectorsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kbConnectCallback**](ConnectorsApi.md#kbConnectCallback) | **GET** /v1/kb/connectors/{provider}/callback | OAuth callback (provider redirect — org recovered from signed state) |
| [**kbConnectStart**](ConnectorsApi.md#kbConnectStart) | **GET** /v1/kb/connectors/{provider}/connect | Begin an OAuth connection (returns the provider authorize URL) |
| [**kbDisconnectConnector**](ConnectorsApi.md#kbDisconnectConnector) | **DELETE** /v1/kb/connectors/{provider} | Disconnect a connector (tombstone token, purge its vector points) |
| [**kbListCatalog**](ConnectorsApi.md#kbListCatalog) | **GET** /v1/kb/connectors/catalog | List every connectable source (native + long-tail pieces) |
| [**kbListConnectors**](ConnectorsApi.md#kbListConnectors) | **GET** /v1/kb/connectors | List this org&#39;s connectors and connection state |
| [**kbSyncConnector**](ConnectorsApi.md#kbSyncConnector) | **POST** /v1/kb/connectors/{provider}/sync | Sync the provider&#39;s documents into this org&#39;s knowledge store |


<a id="kbConnectCallback"></a>
# **kbConnectCallback**
> KbConnectCallback200Response kbConnectCallback(provider, code, state, error)

OAuth callback (provider redirect — org recovered from signed state)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectorsApi()
val provider : kotlin.String = provider_example // kotlin.String | 
val code : kotlin.String = code_example // kotlin.String | 
val state : kotlin.String = state_example // kotlin.String | 
val error : kotlin.String = error_example // kotlin.String | 
try {
    val result : KbConnectCallback200Response = apiInstance.kbConnectCallback(provider, code, state, error)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectorsApi#kbConnectCallback")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectorsApi#kbConnectCallback")
    e.printStackTrace()
}
```

### Parameters
| **provider** | **kotlin.String**|  | [enum: github, slack, google, notion] |
| **code** | **kotlin.String**|  | [optional] |
| **state** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **error** | **kotlin.String**|  | [optional] |

### Return type

[**KbConnectCallback200Response**](KbConnectCallback200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="kbConnectStart"></a>
# **kbConnectStart**
> KbConnectStart200Response kbConnectStart(provider)

Begin an OAuth connection (returns the provider authorize URL)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectorsApi()
val provider : kotlin.String = provider_example // kotlin.String | 
try {
    val result : KbConnectStart200Response = apiInstance.kbConnectStart(provider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectorsApi#kbConnectStart")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectorsApi#kbConnectStart")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **provider** | **kotlin.String**|  | [enum: github, slack, google, notion] |

### Return type

[**KbConnectStart200Response**](KbConnectStart200Response.md)

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

<a id="kbDisconnectConnector"></a>
# **kbDisconnectConnector**
> KbDisconnectConnector200Response kbDisconnectConnector(provider)

Disconnect a connector (tombstone token, purge its vector points)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectorsApi()
val provider : kotlin.String = provider_example // kotlin.String | 
try {
    val result : KbDisconnectConnector200Response = apiInstance.kbDisconnectConnector(provider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectorsApi#kbDisconnectConnector")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectorsApi#kbDisconnectConnector")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **provider** | **kotlin.String**|  | [enum: github, slack, google, notion] |

### Return type

[**KbDisconnectConnector200Response**](KbDisconnectConnector200Response.md)

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

<a id="kbListCatalog"></a>
# **kbListCatalog**
> KbListCatalog200Response kbListCatalog()

List every connectable source (native + long-tail pieces)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectorsApi()
try {
    val result : KbListCatalog200Response = apiInstance.kbListCatalog()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectorsApi#kbListCatalog")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectorsApi#kbListCatalog")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**KbListCatalog200Response**](KbListCatalog200Response.md)

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

<a id="kbListConnectors"></a>
# **kbListConnectors**
> KbListConnectors200Response kbListConnectors()

List this org&#39;s connectors and connection state

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectorsApi()
try {
    val result : KbListConnectors200Response = apiInstance.kbListConnectors()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectorsApi#kbListConnectors")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectorsApi#kbListConnectors")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**KbListConnectors200Response**](KbListConnectors200Response.md)

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

<a id="kbSyncConnector"></a>
# **kbSyncConnector**
> KbSyncConnector200Response kbSyncConnector(provider)

Sync the provider&#39;s documents into this org&#39;s knowledge store

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ConnectorsApi()
val provider : kotlin.String = provider_example // kotlin.String | 
try {
    val result : KbSyncConnector200Response = apiInstance.kbSyncConnector(provider)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ConnectorsApi#kbSyncConnector")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ConnectorsApi#kbSyncConnector")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **provider** | **kotlin.String**|  | [enum: github, slack, google, notion] |

### Return type

[**KbSyncConnector200Response**](KbSyncConnector200Response.md)

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

