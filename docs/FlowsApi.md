# FlowsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoCountFlows**](FlowsApi.md#autoCountFlows) | **GET** /v1/auto/flows/count | Count flows |
| [**autoCreateFlow**](FlowsApi.md#autoCreateFlow) | **POST** /v1/auto/flows | Create a flow |
| [**autoDeleteFlow**](FlowsApi.md#autoDeleteFlow) | **DELETE** /v1/auto/flows/{id} | Delete a flow |
| [**autoGetFlow**](FlowsApi.md#autoGetFlow) | **GET** /v1/auto/flows/{id} | Get a flow by id |
| [**autoGetFlowTemplate**](FlowsApi.md#autoGetFlowTemplate) | **GET** /v1/auto/flows/{id}/template | Export flow as template |
| [**autoListFlows**](FlowsApi.md#autoListFlows) | **GET** /v1/auto/flows | List flows |
| [**autoUpdateFlow**](FlowsApi.md#autoUpdateFlow) | **POST** /v1/auto/flows/{id} | Apply an operation to a flow |
| [**automationsApplyOperation**](FlowsApi.md#automationsApplyOperation) | **POST** /v1/automations/flows/{id}/operations | Apply a flow operation to the latest version |
| [**automationsCreateFlow**](FlowsApi.md#automationsCreateFlow) | **POST** /v1/automations/flows | Create a flow (with an initial draft version) |
| [**automationsCreateVersion**](FlowsApi.md#automationsCreateVersion) | **POST** /v1/automations/flows/{id}/versions | Create a draft version |
| [**automationsDeleteFlow**](FlowsApi.md#automationsDeleteFlow) | **DELETE** /v1/automations/flows/{id} | Delete a flow (with its versions and runs) |
| [**automationsDisableFlow**](FlowsApi.md#automationsDisableFlow) | **POST** /v1/automations/flows/{id}/disable | Disable a flow (removes any POLLING schedule) |
| [**automationsEnableFlow**](FlowsApi.md#automationsEnableFlow) | **POST** /v1/automations/flows/{id}/enable | Enable a flow (POLLING triggers create a schedule) |
| [**automationsGetFlow**](FlowsApi.md#automationsGetFlow) | **GET** /v1/automations/flows/{id} | Get a flow and its latest version |
| [**automationsListFlows**](FlowsApi.md#automationsListFlows) | **GET** /v1/automations/flows | List flows |
| [**automationsListVersions**](FlowsApi.md#automationsListVersions) | **GET** /v1/automations/flows/{id}/versions | List a flow&#39;s versions |
| [**automationsUpdateFlow**](FlowsApi.md#automationsUpdateFlow) | **PATCH** /v1/automations/flows/{id} | Update flow metadata |
| [**flowCountFlows**](FlowsApi.md#flowCountFlows) | **GET** /v1/flow/flows/count | Count flows |
| [**flowCreateFlow**](FlowsApi.md#flowCreateFlow) | **POST** /v1/flow/flows | Create a flow |
| [**flowDeleteFlow**](FlowsApi.md#flowDeleteFlow) | **DELETE** /v1/flow/flows/{id} | Delete a flow |
| [**flowGetFlow**](FlowsApi.md#flowGetFlow) | **GET** /v1/flow/flows/{id} | Get a flow by id |
| [**flowGetFlowTemplate**](FlowsApi.md#flowGetFlowTemplate) | **GET** /v1/flow/flows/{id}/template | Export flow as template |
| [**flowGetHumanInputForm**](FlowsApi.md#flowGetHumanInputForm) | **GET** /v1/flow/human-input/form/{flowId} | Get human input form definition for a flow |
| [**flowGetStepFile**](FlowsApi.md#flowGetStepFile) | **GET** /v1/flow/step-files | Get a file produced by a flow step |
| [**flowListFlows**](FlowsApi.md#flowListFlows) | **GET** /v1/flow/flows | List flows |
| [**flowUpdateFlow**](FlowsApi.md#flowUpdateFlow) | **POST** /v1/flow/flows/{id} | Apply an operation to a flow |


<a id="autoCountFlows"></a>
# **autoCountFlows**
> kotlin.Any autoCountFlows(folderId)

Count flows

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val folderId : kotlin.String = folderId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoCountFlows(folderId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#autoCountFlows")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#autoCountFlows")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **folderId** | **kotlin.String**|  | [optional] |

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

<a id="autoCreateFlow"></a>
# **autoCreateFlow**
> AutoFlow autoCreateFlow(autoCreateFlowRequest)

Create a flow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val autoCreateFlowRequest : AutoCreateFlowRequest =  // AutoCreateFlowRequest | 
try {
    val result : AutoFlow = apiInstance.autoCreateFlow(autoCreateFlowRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#autoCreateFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#autoCreateFlow")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateFlowRequest** | [**AutoCreateFlowRequest**](AutoCreateFlowRequest.md)|  | |

### Return type

[**AutoFlow**](AutoFlow.md)

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

<a id="autoDeleteFlow"></a>
# **autoDeleteFlow**
> autoDeleteFlow(id)

Delete a flow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.autoDeleteFlow(id)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#autoDeleteFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#autoDeleteFlow")
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

<a id="autoGetFlow"></a>
# **autoGetFlow**
> AutoFlow autoGetFlow(id, versionId)

Get a flow by id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
val versionId : kotlin.String = versionId_example // kotlin.String | 
try {
    val result : AutoFlow = apiInstance.autoGetFlow(id, versionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#autoGetFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#autoGetFlow")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **versionId** | **kotlin.String**|  | [optional] |

### Return type

[**AutoFlow**](AutoFlow.md)

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

<a id="autoGetFlowTemplate"></a>
# **autoGetFlowTemplate**
> kotlin.Any autoGetFlowTemplate(id)

Export flow as template

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoGetFlowTemplate(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#autoGetFlowTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#autoGetFlowTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="autoListFlows"></a>
# **autoListFlows**
> AutoListFlows200Response autoListFlows(folderId, status, name, cursor, limit)

List flows

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val folderId : kotlin.String = folderId_example // kotlin.String | 
val status : kotlin.String = status_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : AutoListFlows200Response = apiInstance.autoListFlows(folderId, status, name, cursor, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#autoListFlows")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#autoListFlows")
    e.printStackTrace()
}
```

### Parameters
| **folderId** | **kotlin.String**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] [enum: ENABLED, DISABLED] |
| **name** | **kotlin.String**|  | [optional] |
| **cursor** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 10] |

### Return type

[**AutoListFlows200Response**](AutoListFlows200Response.md)

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

<a id="autoUpdateFlow"></a>
# **autoUpdateFlow**
> AutoFlow autoUpdateFlow(id, autoUpdateFlowRequest)

Apply an operation to a flow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
val autoUpdateFlowRequest : AutoUpdateFlowRequest =  // AutoUpdateFlowRequest | 
try {
    val result : AutoFlow = apiInstance.autoUpdateFlow(id, autoUpdateFlowRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#autoUpdateFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#autoUpdateFlow")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoUpdateFlowRequest** | [**AutoUpdateFlowRequest**](AutoUpdateFlowRequest.md)|  | |

### Return type

[**AutoFlow**](AutoFlow.md)

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

<a id="automationsApplyOperation"></a>
# **automationsApplyOperation**
> AutomationsFlowVersion automationsApplyOperation(id, automationsFlowOperation)

Apply a flow operation to the latest version

A CHANGE_STATUS op enables/disables the flow (returns the Flow); every other op mutates the latest version&#39;s step tree (returns the FlowVersion).

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
val automationsFlowOperation : AutomationsFlowOperation =  // AutomationsFlowOperation | 
try {
    val result : AutomationsFlowVersion = apiInstance.automationsApplyOperation(id, automationsFlowOperation)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#automationsApplyOperation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#automationsApplyOperation")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **automationsFlowOperation** | [**AutomationsFlowOperation**](AutomationsFlowOperation.md)|  | |

### Return type

[**AutomationsFlowVersion**](AutomationsFlowVersion.md)

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

<a id="automationsCreateFlow"></a>
# **automationsCreateFlow**
> AutomationsPopulatedFlow automationsCreateFlow(automationsCreateFlowRequest)

Create a flow (with an initial draft version)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val automationsCreateFlowRequest : AutomationsCreateFlowRequest =  // AutomationsCreateFlowRequest | 
try {
    val result : AutomationsPopulatedFlow = apiInstance.automationsCreateFlow(automationsCreateFlowRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#automationsCreateFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#automationsCreateFlow")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **automationsCreateFlowRequest** | [**AutomationsCreateFlowRequest**](AutomationsCreateFlowRequest.md)|  | |

### Return type

[**AutomationsPopulatedFlow**](AutomationsPopulatedFlow.md)

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

<a id="automationsCreateVersion"></a>
# **automationsCreateVersion**
> AutomationsFlowVersion automationsCreateVersion(id, automationsCreateVersionRequest)

Create a draft version

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
val automationsCreateVersionRequest : AutomationsCreateVersionRequest =  // AutomationsCreateVersionRequest | 
try {
    val result : AutomationsFlowVersion = apiInstance.automationsCreateVersion(id, automationsCreateVersionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#automationsCreateVersion")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#automationsCreateVersion")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **automationsCreateVersionRequest** | [**AutomationsCreateVersionRequest**](AutomationsCreateVersionRequest.md)|  | |

### Return type

[**AutomationsFlowVersion**](AutomationsFlowVersion.md)

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

<a id="automationsDeleteFlow"></a>
# **automationsDeleteFlow**
> automationsDeleteFlow(id)

Delete a flow (with its versions and runs)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.automationsDeleteFlow(id)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#automationsDeleteFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#automationsDeleteFlow")
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
 - **Accept**: application/json

<a id="automationsDisableFlow"></a>
# **automationsDisableFlow**
> AutomationsFlow automationsDisableFlow(id)

Disable a flow (removes any POLLING schedule)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : AutomationsFlow = apiInstance.automationsDisableFlow(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#automationsDisableFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#automationsDisableFlow")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**AutomationsFlow**](AutomationsFlow.md)

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

<a id="automationsEnableFlow"></a>
# **automationsEnableFlow**
> AutomationsFlow automationsEnableFlow(id)

Enable a flow (POLLING triggers create a schedule)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : AutomationsFlow = apiInstance.automationsEnableFlow(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#automationsEnableFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#automationsEnableFlow")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**AutomationsFlow**](AutomationsFlow.md)

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

<a id="automationsGetFlow"></a>
# **automationsGetFlow**
> AutomationsPopulatedFlow automationsGetFlow(id)

Get a flow and its latest version

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : AutomationsPopulatedFlow = apiInstance.automationsGetFlow(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#automationsGetFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#automationsGetFlow")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**AutomationsPopulatedFlow**](AutomationsPopulatedFlow.md)

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

<a id="automationsListFlows"></a>
# **automationsListFlows**
> AutomationsListFlows200Response automationsListFlows(limit)

List flows

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : AutomationsListFlows200Response = apiInstance.automationsListFlows(limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#automationsListFlows")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#automationsListFlows")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 200] |

### Return type

[**AutomationsListFlows200Response**](AutomationsListFlows200Response.md)

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

<a id="automationsListVersions"></a>
# **automationsListVersions**
> AutomationsListVersions200Response automationsListVersions(id, limit)

List a flow&#39;s versions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : AutomationsListVersions200Response = apiInstance.automationsListVersions(id, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#automationsListVersions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#automationsListVersions")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 200] |

### Return type

[**AutomationsListVersions200Response**](AutomationsListVersions200Response.md)

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

<a id="automationsUpdateFlow"></a>
# **automationsUpdateFlow**
> AutomationsFlow automationsUpdateFlow(id, automationsPatchFlowRequest)

Update flow metadata

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
val automationsPatchFlowRequest : AutomationsPatchFlowRequest =  // AutomationsPatchFlowRequest | 
try {
    val result : AutomationsFlow = apiInstance.automationsUpdateFlow(id, automationsPatchFlowRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#automationsUpdateFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#automationsUpdateFlow")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **automationsPatchFlowRequest** | [**AutomationsPatchFlowRequest**](AutomationsPatchFlowRequest.md)|  | |

### Return type

[**AutomationsFlow**](AutomationsFlow.md)

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

<a id="flowCountFlows"></a>
# **flowCountFlows**
> FlowCountFlows200Response flowCountFlows(folderId)

Count flows

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val folderId : kotlin.String = folderId_example // kotlin.String | 
try {
    val result : FlowCountFlows200Response = apiInstance.flowCountFlows(folderId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#flowCountFlows")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#flowCountFlows")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **folderId** | **kotlin.String**|  | [optional] |

### Return type

[**FlowCountFlows200Response**](FlowCountFlows200Response.md)

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

<a id="flowCreateFlow"></a>
# **flowCreateFlow**
> FlowFlow flowCreateFlow(autoCreateFlowRequest)

Create a flow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val autoCreateFlowRequest : AutoCreateFlowRequest =  // AutoCreateFlowRequest | 
try {
    val result : FlowFlow = apiInstance.flowCreateFlow(autoCreateFlowRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#flowCreateFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#flowCreateFlow")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoCreateFlowRequest** | [**AutoCreateFlowRequest**](AutoCreateFlowRequest.md)|  | |

### Return type

[**FlowFlow**](FlowFlow.md)

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

<a id="flowDeleteFlow"></a>
# **flowDeleteFlow**
> flowDeleteFlow(id)

Delete a flow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.flowDeleteFlow(id)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#flowDeleteFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#flowDeleteFlow")
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

<a id="flowGetFlow"></a>
# **flowGetFlow**
> FlowFlow flowGetFlow(id, versionId)

Get a flow by id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
val versionId : kotlin.String = versionId_example // kotlin.String | 
try {
    val result : FlowFlow = apiInstance.flowGetFlow(id, versionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#flowGetFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#flowGetFlow")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **versionId** | **kotlin.String**|  | [optional] |

### Return type

[**FlowFlow**](FlowFlow.md)

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

<a id="flowGetFlowTemplate"></a>
# **flowGetFlowTemplate**
> FlowTemplate flowGetFlowTemplate(id)

Export flow as template

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : FlowTemplate = apiInstance.flowGetFlowTemplate(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#flowGetFlowTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#flowGetFlowTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**FlowTemplate**](FlowTemplate.md)

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

<a id="flowGetHumanInputForm"></a>
# **flowGetHumanInputForm**
> kotlin.Any flowGetHumanInputForm(flowId)

Get human input form definition for a flow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val flowId : kotlin.String = flowId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.flowGetHumanInputForm(flowId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#flowGetHumanInputForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#flowGetHumanInputForm")
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

<a id="flowGetStepFile"></a>
# **flowGetStepFile**
> java.io.File flowGetStepFile(id)

Get a file produced by a flow step

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : java.io.File = apiInstance.flowGetStepFile(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#flowGetStepFile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#flowGetStepFile")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**java.io.File**](java.io.File.md)

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
 - **Accept**: application/octet-stream

<a id="flowListFlows"></a>
# **flowListFlows**
> FlowListFlows200Response flowListFlows(folderId, status, name, cursor, limit)

List flows

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val folderId : kotlin.String = folderId_example // kotlin.String | 
val status : kotlin.String = status_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : FlowListFlows200Response = apiInstance.flowListFlows(folderId, status, name, cursor, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#flowListFlows")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#flowListFlows")
    e.printStackTrace()
}
```

### Parameters
| **folderId** | **kotlin.String**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] [enum: ENABLED, DISABLED] |
| **name** | **kotlin.String**|  | [optional] |
| **cursor** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 10] |

### Return type

[**FlowListFlows200Response**](FlowListFlows200Response.md)

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

<a id="flowUpdateFlow"></a>
# **flowUpdateFlow**
> FlowFlow flowUpdateFlow(id, autoUpdateFlowRequest)

Apply an operation to a flow

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FlowsApi()
val id : kotlin.String = id_example // kotlin.String | 
val autoUpdateFlowRequest : AutoUpdateFlowRequest =  // AutoUpdateFlowRequest | 
try {
    val result : FlowFlow = apiInstance.flowUpdateFlow(id, autoUpdateFlowRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FlowsApi#flowUpdateFlow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FlowsApi#flowUpdateFlow")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoUpdateFlowRequest** | [**AutoUpdateFlowRequest**](AutoUpdateFlowRequest.md)|  | |

### Return type

[**FlowFlow**](FlowFlow.md)

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

