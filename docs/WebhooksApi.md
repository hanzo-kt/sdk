# WebhooksApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoHandleWebhook**](WebhooksApi.md#autoHandleWebhook) | **POST** /v1/auto/webhooks/{flowId} | Receive incoming webhook for a flow trigger |
| [**autoHandleWebhookSync**](WebhooksApi.md#autoHandleWebhookSync) | **POST** /v1/auto/webhooks/{flowId}/sync | Receive webhook and wait for flow run result |
| [**flowHandleWebhook**](WebhooksApi.md#flowHandleWebhook) | **POST** /v1/flow/webhooks/{flowId} | Receive incoming webhook for a flow trigger |
| [**flowHandleWebhookSync**](WebhooksApi.md#flowHandleWebhookSync) | **POST** /v1/flow/webhooks/{flowId}/sync | Receive webhook and wait for flow run result |
| [**flowSimulateWebhook**](WebhooksApi.md#flowSimulateWebhook) | **GET** /v1/flow/webhooks/{flowId}/simulate | Simulate a webhook to capture sample data |
| [**iamApiControllerAddWebhook**](WebhooksApi.md#iamApiControllerAddWebhook) | **POST** /v1/iam/webhooks | Api Controller Add Webhook |
| [**iamApiControllerDeleteWebhook**](WebhooksApi.md#iamApiControllerDeleteWebhook) | **DELETE** /v1/iam/webhooks/{id} | Api Controller Delete Webhook |
| [**iamApiControllerGetWebhook**](WebhooksApi.md#iamApiControllerGetWebhook) | **GET** /v1/iam/webhooks/{id} | Api Controller Get Webhook |
| [**iamApiControllerGetWebhooks**](WebhooksApi.md#iamApiControllerGetWebhooks) | **GET** /v1/iam/webhooks | Api Controller Get Webhooks |
| [**iamApiControllerUpdateWebhook**](WebhooksApi.md#iamApiControllerUpdateWebhook) | **PUT** /v1/iam/webhooks/{id} | Api Controller Update Webhook |
| [**kmsCreateWebhook**](WebhooksApi.md#kmsCreateWebhook) | **POST** /v1/kms/webhooks | Create a webhook |
| [**kmsDeleteWebhook**](WebhooksApi.md#kmsDeleteWebhook) | **DELETE** /v1/kms/webhooks/{webhookId} | Delete a webhook |
| [**kmsListWebhooks**](WebhooksApi.md#kmsListWebhooks) | **GET** /v1/kms/webhooks | List webhooks for a project |
| [**kmsTestWebhook**](WebhooksApi.md#kmsTestWebhook) | **POST** /v1/kms/webhooks/{webhookId}/test | Test a webhook |
| [**kmsUpdateWebhook**](WebhooksApi.md#kmsUpdateWebhook) | **PATCH** /v1/kms/webhooks/{webhookId} | Update a webhook |
| [**registryCreateWebhook**](WebhooksApi.md#registryCreateWebhook) | **POST** /v1/registry/webhooks | Create webhook |
| [**registryDeleteWebhook**](WebhooksApi.md#registryDeleteWebhook) | **DELETE** /v1/registry/webhooks/{id} | Delete webhook |
| [**registryGetWebhook**](WebhooksApi.md#registryGetWebhook) | **GET** /v1/registry/webhooks/{id} | Get webhook |
| [**registryListWebhooks**](WebhooksApi.md#registryListWebhooks) | **GET** /v1/registry/webhooks | List webhooks |
| [**registryUpdateWebhook**](WebhooksApi.md#registryUpdateWebhook) | **PUT** /v1/registry/webhooks/{id} | Update webhook |
| [**searchDeleteWebhooks**](WebhooksApi.md#searchDeleteWebhooks) | **DELETE** /v1/search/webhooks | Delete all webhooks |
| [**searchGetWebhooks**](WebhooksApi.md#searchGetWebhooks) | **GET** /v1/search/webhooks | Get webhook configuration |
| [**searchUpdateWebhooks**](WebhooksApi.md#searchUpdateWebhooks) | **PATCH** /v1/search/webhooks | Update webhook configuration |


<a id="autoHandleWebhook"></a>
# **autoHandleWebhook**
> kotlin.Any autoHandleWebhook(flowId, body)

Receive incoming webhook for a flow trigger

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.autoHandleWebhook(flowId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#autoHandleWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#autoHandleWebhook")
    e.printStackTrace()
}
```

### Parameters
| **flowId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | [optional] |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="autoHandleWebhookSync"></a>
# **autoHandleWebhookSync**
> kotlin.Any autoHandleWebhookSync(flowId)

Receive webhook and wait for flow run result

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoHandleWebhookSync(flowId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#autoHandleWebhookSync")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#autoHandleWebhookSync")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowId** | **kotlin.String**|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="flowHandleWebhook"></a>
# **flowHandleWebhook**
> kotlin.Any flowHandleWebhook(flowId, body)

Receive incoming webhook for a flow trigger

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.flowHandleWebhook(flowId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#flowHandleWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#flowHandleWebhook")
    e.printStackTrace()
}
```

### Parameters
| **flowId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | [optional] |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="flowHandleWebhookSync"></a>
# **flowHandleWebhookSync**
> kotlin.Any flowHandleWebhookSync(flowId, body)

Receive webhook and wait for flow run result

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.flowHandleWebhookSync(flowId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#flowHandleWebhookSync")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#flowHandleWebhookSync")
    e.printStackTrace()
}
```

### Parameters
| **flowId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | [optional] |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="flowSimulateWebhook"></a>
# **flowSimulateWebhook**
> kotlin.Any flowSimulateWebhook(flowId)

Simulate a webhook to capture sample data

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowSimulateWebhook(flowId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#flowSimulateWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#flowSimulateWebhook")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **flowId** | **kotlin.String**|  | |

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

<a id="iamApiControllerAddWebhook"></a>
# **iamApiControllerAddWebhook**
> IamControllersResponse iamApiControllerAddWebhook(iamObjectWebhook)

Api Controller Add Webhook

add webhook

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val iamObjectWebhook : IamObjectWebhook =  // IamObjectWebhook | The details of the webhook
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddWebhook(iamObjectWebhook)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#iamApiControllerAddWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#iamApiControllerAddWebhook")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectWebhook** | [**IamObjectWebhook**](IamObjectWebhook.md)| The details of the webhook | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerDeleteWebhook"></a>
# **iamApiControllerDeleteWebhook**
> IamControllersResponse iamApiControllerDeleteWebhook(id, iamObjectWebhook)

Api Controller Delete Webhook

delete webhook

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectWebhook : IamObjectWebhook =  // IamObjectWebhook | The details of the webhook
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteWebhook(id, iamObjectWebhook)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#iamApiControllerDeleteWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#iamApiControllerDeleteWebhook")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectWebhook** | [**IamObjectWebhook**](IamObjectWebhook.md)| The details of the webhook | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="iamApiControllerGetWebhook"></a>
# **iamApiControllerGetWebhook**
> IamObjectWebhook iamApiControllerGetWebhook(id)

Api Controller Get Webhook

get webhook

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the webhook
try {
    val result : IamObjectWebhook = apiInstance.iamApiControllerGetWebhook(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#iamApiControllerGetWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#iamApiControllerGetWebhook")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the webhook | [default to &quot;built-in/admin&quot;] |

### Return type

[**IamObjectWebhook**](IamObjectWebhook.md)

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

<a id="iamApiControllerGetWebhooks"></a>
# **iamApiControllerGetWebhooks**
> kotlin.collections.List&lt;IamObjectWebhook&gt; iamApiControllerGetWebhooks(owner)

Api Controller Get Webhooks

get webhooks

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of webhooks
try {
    val result : kotlin.collections.List<IamObjectWebhook> = apiInstance.iamApiControllerGetWebhooks(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#iamApiControllerGetWebhooks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#iamApiControllerGetWebhooks")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of webhooks | [default to &quot;built-in/admin&quot;] |

### Return type

[**kotlin.collections.List&lt;IamObjectWebhook&gt;**](IamObjectWebhook.md)

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

<a id="iamApiControllerUpdateWebhook"></a>
# **iamApiControllerUpdateWebhook**
> IamControllersResponse iamApiControllerUpdateWebhook(id, iamObjectWebhook)

Api Controller Update Webhook

update webhook

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the webhook
val iamObjectWebhook : IamObjectWebhook =  // IamObjectWebhook | The details of the webhook
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateWebhook(id, iamObjectWebhook)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#iamApiControllerUpdateWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#iamApiControllerUpdateWebhook")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the webhook | [default to &quot;built-in/admin&quot;] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectWebhook** | [**IamObjectWebhook**](IamObjectWebhook.md)| The details of the webhook | |

### Return type

[**IamControllersResponse**](IamControllersResponse.md)

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

<a id="kmsCreateWebhook"></a>
# **kmsCreateWebhook**
> KmsCreateWebhook200Response kmsCreateWebhook(kmsCreateWebhookRequest)

Create a webhook

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val kmsCreateWebhookRequest : KmsCreateWebhookRequest =  // KmsCreateWebhookRequest | 
try {
    val result : KmsCreateWebhook200Response = apiInstance.kmsCreateWebhook(kmsCreateWebhookRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#kmsCreateWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#kmsCreateWebhook")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateWebhookRequest** | [**KmsCreateWebhookRequest**](KmsCreateWebhookRequest.md)|  | |

### Return type

[**KmsCreateWebhook200Response**](KmsCreateWebhook200Response.md)

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

<a id="kmsDeleteWebhook"></a>
# **kmsDeleteWebhook**
> kotlin.Any kmsDeleteWebhook(webhookId)

Delete a webhook

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val webhookId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kmsDeleteWebhook(webhookId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#kmsDeleteWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#kmsDeleteWebhook")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhookId** | **java.util.UUID**|  | |

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

<a id="kmsListWebhooks"></a>
# **kmsListWebhooks**
> KmsListWebhooks200Response kmsListWebhooks(workspaceId)

List webhooks for a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val workspaceId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsListWebhooks200Response = apiInstance.kmsListWebhooks(workspaceId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#kmsListWebhooks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#kmsListWebhooks")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **workspaceId** | **java.util.UUID**|  | |

### Return type

[**KmsListWebhooks200Response**](KmsListWebhooks200Response.md)

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

<a id="kmsTestWebhook"></a>
# **kmsTestWebhook**
> kotlin.Any kmsTestWebhook(webhookId)

Test a webhook

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val webhookId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kmsTestWebhook(webhookId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#kmsTestWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#kmsTestWebhook")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **webhookId** | **java.util.UUID**|  | |

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

<a id="kmsUpdateWebhook"></a>
# **kmsUpdateWebhook**
> KmsCreateWebhook200Response kmsUpdateWebhook(webhookId, kmsUpdateWebhookRequest)

Update a webhook

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val webhookId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsUpdateWebhookRequest : KmsUpdateWebhookRequest =  // KmsUpdateWebhookRequest | 
try {
    val result : KmsCreateWebhook200Response = apiInstance.kmsUpdateWebhook(webhookId, kmsUpdateWebhookRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#kmsUpdateWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#kmsUpdateWebhook")
    e.printStackTrace()
}
```

### Parameters
| **webhookId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUpdateWebhookRequest** | [**KmsUpdateWebhookRequest**](KmsUpdateWebhookRequest.md)|  | |

### Return type

[**KmsCreateWebhook200Response**](KmsCreateWebhook200Response.md)

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

<a id="registryCreateWebhook"></a>
# **registryCreateWebhook**
> kotlin.Any registryCreateWebhook(registryWebhookCreate)

Create webhook

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val registryWebhookCreate : RegistryWebhookCreate =  // RegistryWebhookCreate | 
try {
    val result : kotlin.Any = apiInstance.registryCreateWebhook(registryWebhookCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#registryCreateWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#registryCreateWebhook")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **registryWebhookCreate** | [**RegistryWebhookCreate**](RegistryWebhookCreate.md)|  | |

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

<a id="registryDeleteWebhook"></a>
# **registryDeleteWebhook**
> kotlin.Any registryDeleteWebhook(id)

Delete webhook

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val id : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.Any = apiInstance.registryDeleteWebhook(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#registryDeleteWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#registryDeleteWebhook")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.Int**|  | |

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

<a id="registryGetWebhook"></a>
# **registryGetWebhook**
> RegistryWebhook registryGetWebhook(id)

Get webhook

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val id : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : RegistryWebhook = apiInstance.registryGetWebhook(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#registryGetWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#registryGetWebhook")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.Int**|  | |

### Return type

[**RegistryWebhook**](RegistryWebhook.md)

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

<a id="registryListWebhooks"></a>
# **registryListWebhooks**
> kotlin.collections.List&lt;RegistryWebhook&gt; registryListWebhooks(projectId, page, pageSize)

List webhooks

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val projectId : kotlin.Int = 56 // kotlin.Int | Filter by project ID
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.collections.List<RegistryWebhook> = apiInstance.registryListWebhooks(projectId, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#registryListWebhooks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#registryListWebhooks")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **kotlin.Int**| Filter by project ID | [optional] |
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 10] |

### Return type

[**kotlin.collections.List&lt;RegistryWebhook&gt;**](RegistryWebhook.md)

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

<a id="registryUpdateWebhook"></a>
# **registryUpdateWebhook**
> kotlin.Any registryUpdateWebhook(id, registryWebhookCreate)

Update webhook

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val id : kotlin.Int = 56 // kotlin.Int | 
val registryWebhookCreate : RegistryWebhookCreate =  // RegistryWebhookCreate | 
try {
    val result : kotlin.Any = apiInstance.registryUpdateWebhook(id, registryWebhookCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#registryUpdateWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#registryUpdateWebhook")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.Int**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **registryWebhookCreate** | [**RegistryWebhookCreate**](RegistryWebhookCreate.md)|  | |

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

<a id="searchDeleteWebhooks"></a>
# **searchDeleteWebhooks**
> kotlin.collections.Map&lt;kotlin.String, SearchWebhookResultsValue&gt; searchDeleteWebhooks()

Delete all webhooks

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
try {
    val result : kotlin.collections.Map<kotlin.String, SearchWebhookResultsValue> = apiInstance.searchDeleteWebhooks()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#searchDeleteWebhooks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#searchDeleteWebhooks")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, SearchWebhookResultsValue&gt;**](SearchWebhookResultsValue.md)

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

<a id="searchGetWebhooks"></a>
# **searchGetWebhooks**
> kotlin.collections.Map&lt;kotlin.String, SearchWebhookResultsValue&gt; searchGetWebhooks()

Get webhook configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
try {
    val result : kotlin.collections.Map<kotlin.String, SearchWebhookResultsValue> = apiInstance.searchGetWebhooks()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#searchGetWebhooks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#searchGetWebhooks")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, SearchWebhookResultsValue&gt;**](SearchWebhookResultsValue.md)

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

<a id="searchUpdateWebhooks"></a>
# **searchUpdateWebhooks**
> kotlin.collections.Map&lt;kotlin.String, SearchWebhookResultsValue&gt; searchUpdateWebhooks(requestBody)

Update webhook configuration

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = WebhooksApi()
val requestBody : kotlin.collections.Map<kotlin.String, SearchWebhookSettingsValue> = Object // kotlin.collections.Map<kotlin.String, SearchWebhookSettingsValue> | 
try {
    val result : kotlin.collections.Map<kotlin.String, SearchWebhookResultsValue> = apiInstance.searchUpdateWebhooks(requestBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#searchUpdateWebhooks")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#searchUpdateWebhooks")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **requestBody** | [**kotlin.collections.Map&lt;kotlin.String, SearchWebhookSettingsValue&gt;**](SearchWebhookSettingsValue.md)|  | |

### Return type

[**kotlin.collections.Map&lt;kotlin.String, SearchWebhookResultsValue&gt;**](SearchWebhookResultsValue.md)

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

