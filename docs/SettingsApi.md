# SettingsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatGetUserSettingsFavorites**](SettingsApi.md#chatGetUserSettingsFavorites) | **GET** /v1/chat/user/settings/favorites | Get user favorites |
| [**chatPostUserSettingsFavorites**](SettingsApi.md#chatPostUserSettingsFavorites) | **POST** /v1/chat/user/settings/favorites | Update user favorites |
| [**observeGetSettings**](SettingsApi.md#observeGetSettings) | **GET** /v1/settings/{product} | Read per-(org,product) settings |
| [**observePutSettings**](SettingsApi.md#observePutSettings) | **PUT** /v1/settings/{product} | Write per-(org,product) settings |
| [**platformHealth**](SettingsApi.md#platformHealth) | **GET** /v1/platform/health | Platform health (REST) |
| [**platformHealthcheck**](SettingsApi.md#platformHealthcheck) | **GET** /v1/platform/healthcheck | Platform healthcheck (REST) |
| [**platformSettingsCleanAll**](SettingsApi.md#platformSettingsCleanAll) | **POST** /v1/platform/settings/cleanAll | Full Docker cleanup (admin) |
| [**platformSettingsGetHanzoVersion**](SettingsApi.md#platformSettingsGetHanzoVersion) | **GET** /v1/platform/settings/getHanzoVersion | Get platform version |
| [**platformSettingsHealth**](SettingsApi.md#platformSettingsHealth) | **GET** /v1/platform/settings/health | Platform health check (tRPC) |
| [**platformSettingsIsCloud**](SettingsApi.md#platformSettingsIsCloud) | **GET** /v1/platform/settings/isCloud | Check if running in cloud mode |
| [**platformSettingsReloadTraefik**](SettingsApi.md#platformSettingsReloadTraefik) | **POST** /v1/platform/settings/reloadTraefik | Reload Traefik configuration (admin) |
| [**searchGetSettings**](SettingsApi.md#searchGetSettings) | **GET** /v1/search/indexes/{indexUid}/settings | Get all index settings |
| [**searchResetSettings**](SettingsApi.md#searchResetSettings) | **DELETE** /v1/search/indexes/{indexUid}/settings | Reset all settings to defaults |
| [**searchUpdateSettings**](SettingsApi.md#searchUpdateSettings) | **PATCH** /v1/search/indexes/{indexUid}/settings | Update index settings |


<a id="chatGetUserSettingsFavorites"></a>
# **chatGetUserSettingsFavorites**
> kotlin.Any chatGetUserSettingsFavorites()

Get user favorites

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SettingsApi()
try {
    val result : kotlin.Any = apiInstance.chatGetUserSettingsFavorites()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#chatGetUserSettingsFavorites")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#chatGetUserSettingsFavorites")
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

<a id="chatPostUserSettingsFavorites"></a>
# **chatPostUserSettingsFavorites**
> kotlin.Any chatPostUserSettingsFavorites(body)

Update user favorites

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SettingsApi()
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPostUserSettingsFavorites(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#chatPostUserSettingsFavorites")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#chatPostUserSettingsFavorites")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="observeGetSettings"></a>
# **observeGetSettings**
> ObserveSettingsView observeGetSettings(product)

Read per-(org,product) settings

Returns the org&#39;s persisted config document for a product, plus the NAMES of set secret fields (values are never returned). When the org has never written config for the product, an honest empty config (&#x60;{}&#x60;) is returned with 200 — not a 404. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SettingsApi()
val product : kotlin.String = product_example // kotlin.String | Console product slug. Must match `^[a-z0-9][a-z0-9._-]{0,62}$`.
try {
    val result : ObserveSettingsView = apiInstance.observeGetSettings(product)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#observeGetSettings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#observeGetSettings")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **product** | **kotlin.String**| Console product slug. Must match &#x60;^[a-z0-9][a-z0-9._-]{0,62}$&#x60;. | |

### Return type

[**ObserveSettingsView**](ObserveSettingsView.md)

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

<a id="observePutSettings"></a>
# **observePutSettings**
> ObserveSettingsView observePutSettings(product, observeSettingsRequest)

Write per-(org,product) settings

Upserts the org&#39;s non-secret config document for a product. Secret fields are routed to KMS and NEVER stored in SQLite; a secret whose value is empty or the mask sentinel (&#x60;••••••••&#x60;) is treated as unchanged. If KMS is unavailable, a request carrying secrets fails closed (503) rather than persisting plaintext. Returns the updated settings view. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SettingsApi()
val product : kotlin.String = product_example // kotlin.String | Console product slug. Must match `^[a-z0-9][a-z0-9._-]{0,62}$`.
val observeSettingsRequest : ObserveSettingsRequest =  // ObserveSettingsRequest | 
try {
    val result : ObserveSettingsView = apiInstance.observePutSettings(product, observeSettingsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#observePutSettings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#observePutSettings")
    e.printStackTrace()
}
```

### Parameters
| **product** | **kotlin.String**| Console product slug. Must match &#x60;^[a-z0-9][a-z0-9._-]{0,62}$&#x60;. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **observeSettingsRequest** | [**ObserveSettingsRequest**](ObserveSettingsRequest.md)|  | |

### Return type

[**ObserveSettingsView**](ObserveSettingsView.md)

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

<a id="platformHealth"></a>
# **platformHealth**
> platformHealth()

Platform health (REST)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SettingsApi()
try {
    apiInstance.platformHealth()
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#platformHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#platformHealth")
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

<a id="platformHealthcheck"></a>
# **platformHealthcheck**
> platformHealthcheck()

Platform healthcheck (REST)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SettingsApi()
try {
    apiInstance.platformHealthcheck()
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#platformHealthcheck")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#platformHealthcheck")
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

<a id="platformSettingsCleanAll"></a>
# **platformSettingsCleanAll**
> PlatformTRPCResult platformSettingsCleanAll()

Full Docker cleanup (admin)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SettingsApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformSettingsCleanAll()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#platformSettingsCleanAll")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#platformSettingsCleanAll")
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

<a id="platformSettingsGetHanzoVersion"></a>
# **platformSettingsGetHanzoVersion**
> PlatformTRPCResult platformSettingsGetHanzoVersion()

Get platform version

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SettingsApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformSettingsGetHanzoVersion()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#platformSettingsGetHanzoVersion")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#platformSettingsGetHanzoVersion")
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

<a id="platformSettingsHealth"></a>
# **platformSettingsHealth**
> PlatformTRPCResult platformSettingsHealth()

Platform health check (tRPC)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SettingsApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformSettingsHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#platformSettingsHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#platformSettingsHealth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="platformSettingsIsCloud"></a>
# **platformSettingsIsCloud**
> PlatformTRPCResult platformSettingsIsCloud()

Check if running in cloud mode

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SettingsApi()
try {
    val result : PlatformTRPCResult = apiInstance.platformSettingsIsCloud()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#platformSettingsIsCloud")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#platformSettingsIsCloud")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PlatformTRPCResult**](PlatformTRPCResult.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="platformSettingsReloadTraefik"></a>
# **platformSettingsReloadTraefik**
> PlatformTRPCResult platformSettingsReloadTraefik(platformSettingsReloadTraefikRequest)

Reload Traefik configuration (admin)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SettingsApi()
val platformSettingsReloadTraefikRequest : PlatformSettingsReloadTraefikRequest =  // PlatformSettingsReloadTraefikRequest | 
try {
    val result : PlatformTRPCResult = apiInstance.platformSettingsReloadTraefik(platformSettingsReloadTraefikRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#platformSettingsReloadTraefik")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#platformSettingsReloadTraefik")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platformSettingsReloadTraefikRequest** | [**PlatformSettingsReloadTraefikRequest**](PlatformSettingsReloadTraefikRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="searchGetSettings"></a>
# **searchGetSettings**
> SearchSettings searchGetSettings(indexUid)

Get all index settings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SettingsApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
try {
    val result : SearchSettings = apiInstance.searchGetSettings(indexUid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#searchGetSettings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#searchGetSettings")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **indexUid** | **kotlin.String**| Unique index identifier | |

### Return type

[**SearchSettings**](SearchSettings.md)

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

<a id="searchResetSettings"></a>
# **searchResetSettings**
> SearchSummarizedTaskView searchResetSettings(indexUid)

Reset all settings to defaults

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SettingsApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
try {
    val result : SearchSummarizedTaskView = apiInstance.searchResetSettings(indexUid)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#searchResetSettings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#searchResetSettings")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **indexUid** | **kotlin.String**| Unique index identifier | |

### Return type

[**SearchSummarizedTaskView**](SearchSummarizedTaskView.md)

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

<a id="searchUpdateSettings"></a>
# **searchUpdateSettings**
> SearchSummarizedTaskView searchUpdateSettings(indexUid, searchSettings)

Update index settings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SettingsApi()
val indexUid : kotlin.String = indexUid_example // kotlin.String | Unique index identifier
val searchSettings : SearchSettings =  // SearchSettings | 
try {
    val result : SearchSummarizedTaskView = apiInstance.searchUpdateSettings(indexUid, searchSettings)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SettingsApi#searchUpdateSettings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SettingsApi#searchUpdateSettings")
    e.printStackTrace()
}
```

### Parameters
| **indexUid** | **kotlin.String**| Unique index identifier | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **searchSettings** | [**SearchSettings**](SearchSettings.md)|  | |

### Return type

[**SearchSummarizedTaskView**](SearchSummarizedTaskView.md)

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

