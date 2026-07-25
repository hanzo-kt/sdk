# ModelsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**aiListModels**](ModelsApi.md#aiListModels) | **GET** /v1/models | List available models |
| [**aiRetrieveModel**](ModelsApi.md#aiRetrieveModel) | **GET** /v1/models/{model} | Retrieve a model |
| [**chatGetModels**](ModelsApi.md#chatGetModels) | **GET** /v1/chat/models | List available models |
| [**consoleCreateModel**](ModelsApi.md#consoleCreateModel) | **POST** /v1/console/models | Create a model definition |
| [**consoleDeleteModel**](ModelsApi.md#consoleDeleteModel) | **DELETE** /v1/console/models/{id} | Delete a model |
| [**consoleGetModel**](ModelsApi.md#consoleGetModel) | **GET** /v1/console/models/{id} | Get a model by ID |
| [**consoleListModels**](ModelsApi.md#consoleListModels) | **GET** /v1/console/models | Get all models |
| [**gatewayGetModel**](ModelsApi.md#gatewayGetModel) | **GET** /v1/gateway/models/{model} | Get model |
| [**gatewayListModels**](ModelsApi.md#gatewayListModels) | **GET** /v1/gateway/models | List models |
| [**mlGetModel**](ModelsApi.md#mlGetModel) | **GET** /v1/ml/models/{model_id} | Get model details |
| [**mlListModels**](ModelsApi.md#mlListModels) | **GET** /v1/ml/models | List models |
| [**mlPromoteModel**](ModelsApi.md#mlPromoteModel) | **POST** /v1/ml/models/{model_id}/promote | Promote a model |
| [**mlRegisterModel**](ModelsApi.md#mlRegisterModel) | **POST** /v1/ml/models | Register a model |
| [**mlRollbackModel**](ModelsApi.md#mlRollbackModel) | **POST** /v1/ml/models/{model_id}/rollback | Rollback a model |
| [**pricingGetFullPricing**](ModelsApi.md#pricingGetFullPricing) | **GET** /v1/pricing | Full pricing data |
| [**pricingGetModel**](ModelsApi.md#pricingGetModel) | **GET** /v1/pricing/model/{name} | Single model lookup |
| [**pricingGetPricingSummary**](ModelsApi.md#pricingGetPricingSummary) | **GET** /v1/pricing/summary | Model counts and provider breakdown |
| [**pricingListFeaturedModels**](ModelsApi.md#pricingListFeaturedModels) | **GET** /v1/pricing/featured | Featured third-party models |
| [**pricingListFreeModels**](ModelsApi.md#pricingListFreeModels) | **GET** /v1/pricing/free | Free models only |
| [**pricingListModels**](ModelsApi.md#pricingListModels) | **GET** /v1/pricing/models | List all AI models (OpenAI-compatible) |
| [**pricingListProviders**](ModelsApi.md#pricingListProviders) | **GET** /v1/pricing/providers | Provider breakdown |


<a id="aiListModels"></a>
# **aiListModels**
> AiModelList aiListModels()

List available models

OpenAI-compatible model list across every routable provider.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
try {
    val result : AiModelList = apiInstance.aiListModels()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#aiListModels")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#aiListModels")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**AiModelList**](AiModelList.md)

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

<a id="aiRetrieveModel"></a>
# **aiRetrieveModel**
> AiModel aiRetrieveModel(model)

Retrieve a model

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
val model : kotlin.String = model_example // kotlin.String | 
try {
    val result : AiModel = apiInstance.aiRetrieveModel(model)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#aiRetrieveModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#aiRetrieveModel")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **model** | **kotlin.String**|  | |

### Return type

[**AiModel**](AiModel.md)

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

<a id="chatGetModels"></a>
# **chatGetModels**
> kotlin.collections.Map&lt;kotlin.String, kotlin.collections.List&lt;kotlin.String&gt;&gt; chatGetModels()

List available models

Returns models grouped by endpoint.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.collections.List<kotlin.String>> = apiInstance.chatGetModels()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#chatGetModels")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#chatGetModels")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**kotlin.collections.Map&lt;kotlin.String, kotlin.collections.List&lt;kotlin.String&gt;&gt;**

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

<a id="consoleCreateModel"></a>
# **consoleCreateModel**
> ConsoleModel consoleCreateModel(consoleCreateModelRequest)

Create a model definition

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
val consoleCreateModelRequest : ConsoleCreateModelRequest =  // ConsoleCreateModelRequest | 
try {
    val result : ConsoleModel = apiInstance.consoleCreateModel(consoleCreateModelRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#consoleCreateModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#consoleCreateModel")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleCreateModelRequest** | [**ConsoleCreateModelRequest**](ConsoleCreateModelRequest.md)|  | |

### Return type

[**ConsoleModel**](ConsoleModel.md)

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

<a id="consoleDeleteModel"></a>
# **consoleDeleteModel**
> kotlin.Any consoleDeleteModel(id)

Delete a model

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.consoleDeleteModel(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#consoleDeleteModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#consoleDeleteModel")
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

<a id="consoleGetModel"></a>
# **consoleGetModel**
> ConsoleModel consoleGetModel(id)

Get a model by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : ConsoleModel = apiInstance.consoleGetModel(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#consoleGetModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#consoleGetModel")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**ConsoleModel**](ConsoleModel.md)

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

<a id="consoleListModels"></a>
# **consoleListModels**
> ConsoleListModels200Response consoleListModels(page, limit)

Get all models

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : ConsoleListModels200Response = apiInstance.consoleListModels(page, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#consoleListModels")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#consoleListModels")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**ConsoleListModels200Response**](ConsoleListModels200Response.md)

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

<a id="gatewayGetModel"></a>
# **gatewayGetModel**
> GatewayModel gatewayGetModel(model)

Get model

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
val model : kotlin.String = model_example // kotlin.String | 
try {
    val result : GatewayModel = apiInstance.gatewayGetModel(model)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#gatewayGetModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#gatewayGetModel")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **model** | **kotlin.String**|  | |

### Return type

[**GatewayModel**](GatewayModel.md)

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

<a id="gatewayListModels"></a>
# **gatewayListModels**
> GatewayListModels200Response gatewayListModels()

List models

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
try {
    val result : GatewayListModels200Response = apiInstance.gatewayListModels()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#gatewayListModels")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#gatewayListModels")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**GatewayListModels200Response**](GatewayListModels200Response.md)

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

<a id="mlGetModel"></a>
# **mlGetModel**
> MlModel mlGetModel(modelId)

Get model details

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
val modelId : kotlin.String = modelId_example // kotlin.String | 
try {
    val result : MlModel = apiInstance.mlGetModel(modelId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#mlGetModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#mlGetModel")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **modelId** | **kotlin.String**|  | |

### Return type

[**MlModel**](MlModel.md)

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

<a id="mlListModels"></a>
# **mlListModels**
> MlListModels200Response mlListModels(stage, search)

List models

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
val stage : kotlin.String = stage_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : MlListModels200Response = apiInstance.mlListModels(stage, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#mlListModels")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#mlListModels")
    e.printStackTrace()
}
```

### Parameters
| **stage** | **kotlin.String**|  | [optional] [enum: dev, staging, canary, production] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**MlListModels200Response**](MlListModels200Response.md)

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

<a id="mlPromoteModel"></a>
# **mlPromoteModel**
> MlModel mlPromoteModel(modelId, mlPromoteModelRequest)

Promote a model

Promote a model to the next deployment stage.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
val modelId : kotlin.String = modelId_example // kotlin.String | 
val mlPromoteModelRequest : MlPromoteModelRequest =  // MlPromoteModelRequest | 
try {
    val result : MlModel = apiInstance.mlPromoteModel(modelId, mlPromoteModelRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#mlPromoteModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#mlPromoteModel")
    e.printStackTrace()
}
```

### Parameters
| **modelId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mlPromoteModelRequest** | [**MlPromoteModelRequest**](MlPromoteModelRequest.md)|  | |

### Return type

[**MlModel**](MlModel.md)

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

<a id="mlRegisterModel"></a>
# **mlRegisterModel**
> MlModel mlRegisterModel(mlRegisterModelRequest)

Register a model

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
val mlRegisterModelRequest : MlRegisterModelRequest =  // MlRegisterModelRequest | 
try {
    val result : MlModel = apiInstance.mlRegisterModel(mlRegisterModelRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#mlRegisterModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#mlRegisterModel")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mlRegisterModelRequest** | [**MlRegisterModelRequest**](MlRegisterModelRequest.md)|  | |

### Return type

[**MlModel**](MlModel.md)

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

<a id="mlRollbackModel"></a>
# **mlRollbackModel**
> mlRollbackModel(modelId, mlRollbackModelRequest)

Rollback a model

Rollback to a previous model version.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
val modelId : kotlin.String = modelId_example // kotlin.String | 
val mlRollbackModelRequest : MlRollbackModelRequest =  // MlRollbackModelRequest | 
try {
    apiInstance.mlRollbackModel(modelId, mlRollbackModelRequest)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#mlRollbackModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#mlRollbackModel")
    e.printStackTrace()
}
```

### Parameters
| **modelId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **mlRollbackModelRequest** | [**MlRollbackModelRequest**](MlRollbackModelRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="pricingGetFullPricing"></a>
# **pricingGetFullPricing**
> PricingFullPricingResponse pricingGetFullPricing()

Full pricing data

Returns the complete pricing dataset including all AI models, tools, infrastructure, and cloud plans. Large response (~500KB). 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
try {
    val result : PricingFullPricingResponse = apiInstance.pricingGetFullPricing()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#pricingGetFullPricing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#pricingGetFullPricing")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingFullPricingResponse**](PricingFullPricingResponse.md)

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

<a id="pricingGetModel"></a>
# **pricingGetModel**
> PricingModel pricingGetModel(name)

Single model lookup

Look up a single model by name or ID. Case-insensitive matching. Returns full model details including pricing, specs, and features. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
val name : kotlin.String = zen4 // kotlin.String | Model name or ID (case-insensitive)
try {
    val result : PricingModel = apiInstance.pricingGetModel(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#pricingGetModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#pricingGetModel")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**| Model name or ID (case-insensitive) | |

### Return type

[**PricingModel**](PricingModel.md)

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

<a id="pricingGetPricingSummary"></a>
# **pricingGetPricingSummary**
> PricingSummaryResponse pricingGetPricingSummary()

Model counts and provider breakdown

Returns aggregate statistics: model counts by category, number of providers, and provider breakdown. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
try {
    val result : PricingSummaryResponse = apiInstance.pricingGetPricingSummary()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#pricingGetPricingSummary")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#pricingGetPricingSummary")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingSummaryResponse**](PricingSummaryResponse.md)

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

<a id="pricingListFeaturedModels"></a>
# **pricingListFeaturedModels**
> PricingPricingModelsResponse pricingListFeaturedModels()

Featured third-party models

Returns curated featured models from third-party providers.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
try {
    val result : PricingPricingModelsResponse = apiInstance.pricingListFeaturedModels()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#pricingListFeaturedModels")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#pricingListFeaturedModels")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingPricingModelsResponse**](PricingPricingModelsResponse.md)

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

<a id="pricingListFreeModels"></a>
# **pricingListFreeModels**
> PricingPricingModelsResponse pricingListFreeModels()

Free models only

Returns models with zero cost (free tier eligible).

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
try {
    val result : PricingPricingModelsResponse = apiInstance.pricingListFreeModels()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#pricingListFreeModels")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#pricingListFreeModels")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingPricingModelsResponse**](PricingPricingModelsResponse.md)

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

<a id="pricingListModels"></a>
# **pricingListModels**
> PricingModelListResponse pricingListModels()

List all AI models (OpenAI-compatible)

Returns all available AI models in an OpenAI-compatible format. Includes 32 Zen (Hanzo first-party) models and 344+ third-party models from providers like OpenAI, Anthropic, Google, Meta, etc. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
try {
    val result : PricingModelListResponse = apiInstance.pricingListModels()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#pricingListModels")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#pricingListModels")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingModelListResponse**](PricingModelListResponse.md)

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

<a id="pricingListProviders"></a>
# **pricingListProviders**
> PricingProvidersResponse pricingListProviders()

Provider breakdown

Returns all model providers with counts.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ModelsApi()
try {
    val result : PricingProvidersResponse = apiInstance.pricingListProviders()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ModelsApi#pricingListProviders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ModelsApi#pricingListProviders")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PricingProvidersResponse**](PricingProvidersResponse.md)

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

