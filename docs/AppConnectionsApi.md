# AppConnectionsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoDeleteAppConnection**](AppConnectionsApi.md#autoDeleteAppConnection) | **DELETE** /v1/auto/app-connections/{id} | Delete an app connection |
| [**autoListAppConnections**](AppConnectionsApi.md#autoListAppConnections) | **GET** /v1/auto/app-connections | List app connections |
| [**autoUpdateAppConnection**](AppConnectionsApi.md#autoUpdateAppConnection) | **POST** /v1/auto/app-connections/{id} | Update an app connection |
| [**autoUpsertAppConnection**](AppConnectionsApi.md#autoUpsertAppConnection) | **POST** /v1/auto/app-connections | Upsert an app connection |
| [**flowDeleteAppConnection**](AppConnectionsApi.md#flowDeleteAppConnection) | **DELETE** /v1/flow/app-connections/{id} | Delete an app connection |
| [**flowListAppConnectionOwners**](AppConnectionsApi.md#flowListAppConnectionOwners) | **GET** /v1/flow/app-connections/owners | List app connection owners |
| [**flowListAppConnections**](AppConnectionsApi.md#flowListAppConnections) | **GET** /v1/flow/app-connections | List app connections |
| [**flowReplaceAppConnections**](AppConnectionsApi.md#flowReplaceAppConnections) | **POST** /v1/flow/app-connections/replace | Replace one connection with another across all flows |
| [**flowUpdateAppConnection**](AppConnectionsApi.md#flowUpdateAppConnection) | **POST** /v1/flow/app-connections/{id} | Update an app connection |
| [**flowUpsertAppConnection**](AppConnectionsApi.md#flowUpsertAppConnection) | **POST** /v1/flow/app-connections | Upsert an app connection |
| [**kmsCreateAppConnection**](AppConnectionsApi.md#kmsCreateAppConnection) | **POST** /v1/kms/app-connections | Create an app connection |
| [**kmsDeleteAppConnection**](AppConnectionsApi.md#kmsDeleteAppConnection) | **DELETE** /v1/kms/app-connections/{connectionId} | Delete an app connection |
| [**kmsGetAppConnection**](AppConnectionsApi.md#kmsGetAppConnection) | **GET** /v1/kms/app-connections/{connectionId} | Get an app connection by ID |
| [**kmsListAppConnections**](AppConnectionsApi.md#kmsListAppConnections) | **GET** /v1/kms/app-connections | List app connections |
| [**kmsUpdateAppConnection**](AppConnectionsApi.md#kmsUpdateAppConnection) | **PATCH** /v1/kms/app-connections/{connectionId} | Update an app connection |


<a id="autoDeleteAppConnection"></a>
# **autoDeleteAppConnection**
> autoDeleteAppConnection(id)

Delete an app connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.autoDeleteAppConnection(id)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#autoDeleteAppConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#autoDeleteAppConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

null (empty response body)

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
 - **Accept**: Not defined

<a id="autoListAppConnections"></a>
# **autoListAppConnections**
> AutoListAppConnections200Response autoListAppConnections(pieceName, displayName, status, cursor, limit)

List app connections

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
val pieceName : kotlin.String = pieceName_example // kotlin.String | 
val displayName : kotlin.String = displayName_example // kotlin.String | 
val status : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : AutoListAppConnections200Response = apiInstance.autoListAppConnections(pieceName, displayName, status, cursor, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#autoListAppConnections")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#autoListAppConnections")
    e.printStackTrace()
}
```

### Parameters
| **pieceName** | **kotlin.String**|  | [optional] |
| **displayName** | **kotlin.String**|  | [optional] |
| **status** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] [enum: ACTIVE, ERROR, MISSING_PERMISSIONS] |
| **cursor** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 10] |

### Return type

[**AutoListAppConnections200Response**](AutoListAppConnections200Response.md)

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

<a id="autoUpdateAppConnection"></a>
# **autoUpdateAppConnection**
> kotlin.Any autoUpdateAppConnection(id, autoUpdateAppConnectionRequest)

Update an app connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
val id : kotlin.String = id_example // kotlin.String | 
val autoUpdateAppConnectionRequest : AutoUpdateAppConnectionRequest =  // AutoUpdateAppConnectionRequest | 
try {
    val result : kotlin.Any = apiInstance.autoUpdateAppConnection(id, autoUpdateAppConnectionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#autoUpdateAppConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#autoUpdateAppConnection")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoUpdateAppConnectionRequest** | [**AutoUpdateAppConnectionRequest**](AutoUpdateAppConnectionRequest.md)|  | |

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

<a id="autoUpsertAppConnection"></a>
# **autoUpsertAppConnection**
> AutoAppConnection autoUpsertAppConnection(autoUpsertAppConnectionRequest)

Upsert an app connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
val autoUpsertAppConnectionRequest : AutoUpsertAppConnectionRequest =  // AutoUpsertAppConnectionRequest | 
try {
    val result : AutoAppConnection = apiInstance.autoUpsertAppConnection(autoUpsertAppConnectionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#autoUpsertAppConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#autoUpsertAppConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoUpsertAppConnectionRequest** | [**AutoUpsertAppConnectionRequest**](AutoUpsertAppConnectionRequest.md)|  | |

### Return type

[**AutoAppConnection**](AutoAppConnection.md)

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

<a id="flowDeleteAppConnection"></a>
# **flowDeleteAppConnection**
> flowDeleteAppConnection(id)

Delete an app connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.flowDeleteAppConnection(id)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#flowDeleteAppConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#flowDeleteAppConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

null (empty response body)

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
 - **Accept**: Not defined

<a id="flowListAppConnectionOwners"></a>
# **flowListAppConnectionOwners**
> FlowSeekPage flowListAppConnectionOwners()

List app connection owners

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
try {
    val result : FlowSeekPage = apiInstance.flowListAppConnectionOwners()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#flowListAppConnectionOwners")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#flowListAppConnectionOwners")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**FlowSeekPage**](FlowSeekPage.md)

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

<a id="flowListAppConnections"></a>
# **flowListAppConnections**
> FlowListAppConnections200Response flowListAppConnections(pieceName, displayName, status, cursor, limit)

List app connections

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
val pieceName : kotlin.String = pieceName_example // kotlin.String | 
val displayName : kotlin.String = displayName_example // kotlin.String | 
val status : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | 
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : FlowListAppConnections200Response = apiInstance.flowListAppConnections(pieceName, displayName, status, cursor, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#flowListAppConnections")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#flowListAppConnections")
    e.printStackTrace()
}
```

### Parameters
| **pieceName** | **kotlin.String**|  | [optional] |
| **displayName** | **kotlin.String**|  | [optional] |
| **status** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)|  | [optional] [enum: ACTIVE, ERROR, MISSING_PERMISSIONS] |
| **cursor** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 10] |

### Return type

[**FlowListAppConnections200Response**](FlowListAppConnections200Response.md)

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

<a id="flowReplaceAppConnections"></a>
# **flowReplaceAppConnections**
> kotlin.Any flowReplaceAppConnections(flowReplaceAppConnectionsRequest)

Replace one connection with another across all flows

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
val flowReplaceAppConnectionsRequest : FlowReplaceAppConnectionsRequest =  // FlowReplaceAppConnectionsRequest | 
try {
    val result : kotlin.Any = apiInstance.flowReplaceAppConnections(flowReplaceAppConnectionsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#flowReplaceAppConnections")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#flowReplaceAppConnections")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowReplaceAppConnectionsRequest** | [**FlowReplaceAppConnectionsRequest**](FlowReplaceAppConnectionsRequest.md)|  | |

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

<a id="flowUpdateAppConnection"></a>
# **flowUpdateAppConnection**
> FlowAppConnection flowUpdateAppConnection(id, flowUpdateAppConnectionRequest)

Update an app connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
val id : kotlin.String = id_example // kotlin.String | 
val flowUpdateAppConnectionRequest : FlowUpdateAppConnectionRequest =  // FlowUpdateAppConnectionRequest | 
try {
    val result : FlowAppConnection = apiInstance.flowUpdateAppConnection(id, flowUpdateAppConnectionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#flowUpdateAppConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#flowUpdateAppConnection")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowUpdateAppConnectionRequest** | [**FlowUpdateAppConnectionRequest**](FlowUpdateAppConnectionRequest.md)|  | |

### Return type

[**FlowAppConnection**](FlowAppConnection.md)

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

<a id="flowUpsertAppConnection"></a>
# **flowUpsertAppConnection**
> FlowAppConnection flowUpsertAppConnection(flowUpsertAppConnectionRequest)

Upsert an app connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
val flowUpsertAppConnectionRequest : FlowUpsertAppConnectionRequest =  // FlowUpsertAppConnectionRequest | 
try {
    val result : FlowAppConnection = apiInstance.flowUpsertAppConnection(flowUpsertAppConnectionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#flowUpsertAppConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#flowUpsertAppConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowUpsertAppConnectionRequest** | [**FlowUpsertAppConnectionRequest**](FlowUpsertAppConnectionRequest.md)|  | |

### Return type

[**FlowAppConnection**](FlowAppConnection.md)

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

<a id="kmsCreateAppConnection"></a>
# **kmsCreateAppConnection**
> KmsCreateAppConnection200Response kmsCreateAppConnection(kmsCreateAppConnectionRequest)

Create an app connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
val kmsCreateAppConnectionRequest : KmsCreateAppConnectionRequest =  // KmsCreateAppConnectionRequest | 
try {
    val result : KmsCreateAppConnection200Response = apiInstance.kmsCreateAppConnection(kmsCreateAppConnectionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#kmsCreateAppConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#kmsCreateAppConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateAppConnectionRequest** | [**KmsCreateAppConnectionRequest**](KmsCreateAppConnectionRequest.md)|  | |

### Return type

[**KmsCreateAppConnection200Response**](KmsCreateAppConnection200Response.md)

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

<a id="kmsDeleteAppConnection"></a>
# **kmsDeleteAppConnection**
> kotlin.Any kmsDeleteAppConnection(connectionId)

Delete an app connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
val connectionId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kmsDeleteAppConnection(connectionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#kmsDeleteAppConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#kmsDeleteAppConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **connectionId** | **java.util.UUID**|  | |

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

<a id="kmsGetAppConnection"></a>
# **kmsGetAppConnection**
> KmsCreateAppConnection200Response kmsGetAppConnection(connectionId)

Get an app connection by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
val connectionId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsCreateAppConnection200Response = apiInstance.kmsGetAppConnection(connectionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#kmsGetAppConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#kmsGetAppConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **connectionId** | **java.util.UUID**|  | |

### Return type

[**KmsCreateAppConnection200Response**](KmsCreateAppConnection200Response.md)

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

<a id="kmsListAppConnections"></a>
# **kmsListAppConnections**
> KmsListAppConnections200Response kmsListAppConnections(orgId)

List app connections

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
val orgId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsListAppConnections200Response = apiInstance.kmsListAppConnections(orgId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#kmsListAppConnections")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#kmsListAppConnections")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orgId** | **java.util.UUID**|  | |

### Return type

[**KmsListAppConnections200Response**](KmsListAppConnections200Response.md)

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

<a id="kmsUpdateAppConnection"></a>
# **kmsUpdateAppConnection**
> KmsCreateAppConnection200Response kmsUpdateAppConnection(connectionId, kmsUpdateAppConnectionRequest)

Update an app connection

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = AppConnectionsApi()
val connectionId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsUpdateAppConnectionRequest : KmsUpdateAppConnectionRequest =  // KmsUpdateAppConnectionRequest | 
try {
    val result : KmsCreateAppConnection200Response = apiInstance.kmsUpdateAppConnection(connectionId, kmsUpdateAppConnectionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AppConnectionsApi#kmsUpdateAppConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AppConnectionsApi#kmsUpdateAppConnection")
    e.printStackTrace()
}
```

### Parameters
| **connectionId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUpdateAppConnectionRequest** | [**KmsUpdateAppConnectionRequest**](KmsUpdateAppConnectionRequest.md)|  | |

### Return type

[**KmsCreateAppConnection200Response**](KmsCreateAppConnection200Response.md)

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

