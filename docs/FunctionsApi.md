# FunctionsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**edgeCreateFunction**](FunctionsApi.md#edgeCreateFunction) | **POST** /v1/edge/functions | Create function |
| [**edgeDeleteFunction**](FunctionsApi.md#edgeDeleteFunction) | **DELETE** /v1/edge/functions/{slug} | Delete function |
| [**edgeDeployFunction**](FunctionsApi.md#edgeDeployFunction) | **POST** /v1/edge/functions/{slug}/deploy | Deploy function |
| [**edgeGetFunction**](FunctionsApi.md#edgeGetFunction) | **GET** /v1/edge/functions/{slug} | Get function |
| [**edgeGetFunctionMetrics**](FunctionsApi.md#edgeGetFunctionMetrics) | **GET** /v1/edge/functions/{slug}/metrics | Get function metrics |
| [**edgeInvokeFunction**](FunctionsApi.md#edgeInvokeFunction) | **POST** /v1/edge/functions/{slug}/invoke | Invoke function |
| [**edgeListFunctions**](FunctionsApi.md#edgeListFunctions) | **GET** /v1/edge/functions | List functions |
| [**edgeUpdateFunction**](FunctionsApi.md#edgeUpdateFunction) | **PUT** /v1/edge/functions/{slug} | Update function |
| [**functionsCreateFunction**](FunctionsApi.md#functionsCreateFunction) | **POST** /v1/functions | Create a function |
| [**functionsDeleteFunction**](FunctionsApi.md#functionsDeleteFunction) | **DELETE** /v1/functions/{name} | Delete a function |
| [**functionsGetFunction**](FunctionsApi.md#functionsGetFunction) | **GET** /v1/functions/{name} | Get a function (with triggers, recent invocations, secrets) |
| [**functionsGetFunctionLogs**](FunctionsApi.md#functionsGetFunctionLogs) | **GET** /v1/functions/{name}/logs | Get the latest invocation logs |
| [**functionsInvokeFunction**](FunctionsApi.md#functionsInvokeFunction) | **POST** /v1/functions/{name}/invoke | Invoke a function (metered compute) |
| [**functionsListDeployments**](FunctionsApi.md#functionsListDeployments) | **GET** /v1/functions/deployments | List deployed functions |
| [**functionsListFunctionSecrets**](FunctionsApi.md#functionsListFunctionSecrets) | **GET** /v1/functions/secrets | List function secrets (names only) |
| [**functionsListFunctions**](FunctionsApi.md#functionsListFunctions) | **GET** /v1/functions | List functions |
| [**functionsListInvocations**](FunctionsApi.md#functionsListInvocations) | **GET** /v1/functions/{name}/invocations | List a function&#39;s invocations |
| [**functionsListTriggers**](FunctionsApi.md#functionsListTriggers) | **GET** /v1/functions/triggers | List triggers across functions |


<a id="edgeCreateFunction"></a>
# **edgeCreateFunction**
> EdgeFunction edgeCreateFunction(edgeFunctionCreate)

Create function

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
val edgeFunctionCreate : EdgeFunctionCreate =  // EdgeFunctionCreate | 
try {
    val result : EdgeFunction = apiInstance.edgeCreateFunction(edgeFunctionCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#edgeCreateFunction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#edgeCreateFunction")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **edgeFunctionCreate** | [**EdgeFunctionCreate**](EdgeFunctionCreate.md)|  | |

### Return type

[**EdgeFunction**](EdgeFunction.md)

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

<a id="edgeDeleteFunction"></a>
# **edgeDeleteFunction**
> kotlin.Any edgeDeleteFunction(slug)

Delete function

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.edgeDeleteFunction(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#edgeDeleteFunction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#edgeDeleteFunction")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**|  | |

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

<a id="edgeDeployFunction"></a>
# **edgeDeployFunction**
> EdgeFunction edgeDeployFunction(slug, body)

Deploy function

Deploy function source code. Upload a tarball or zip containing the function source. Creates a new version on success. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
val body : java.io.File = BINARY_DATA_HERE // java.io.File | 
try {
    val result : EdgeFunction = apiInstance.edgeDeployFunction(slug, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#edgeDeployFunction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#edgeDeployFunction")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **java.io.File**|  | |

### Return type

[**EdgeFunction**](EdgeFunction.md)

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

 - **Content-Type**: application/octet-stream
 - **Accept**: application/json

<a id="edgeGetFunction"></a>
# **edgeGetFunction**
> EdgeFunction edgeGetFunction(slug)

Get function

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
try {
    val result : EdgeFunction = apiInstance.edgeGetFunction(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#edgeGetFunction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#edgeGetFunction")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**|  | |

### Return type

[**EdgeFunction**](EdgeFunction.md)

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

<a id="edgeGetFunctionMetrics"></a>
# **edgeGetFunctionMetrics**
> kotlin.collections.List&lt;EdgeFunctionMetrics&gt; edgeGetFunctionMetrics(slug, from, to, granularity)

Get function metrics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
val from : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val to : java.time.OffsetDateTime = 2013-10-20T19:20:30+01:00 // java.time.OffsetDateTime | 
val granularity : kotlin.String = granularity_example // kotlin.String | 
try {
    val result : kotlin.collections.List<EdgeFunctionMetrics> = apiInstance.edgeGetFunctionMetrics(slug, from, to, granularity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#edgeGetFunctionMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#edgeGetFunctionMetrics")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**|  | |
| **from** | **java.time.OffsetDateTime**|  | [optional] |
| **to** | **java.time.OffsetDateTime**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **granularity** | **kotlin.String**|  | [optional] [default to Granularity.hour] [enum: minute, hour, day] |

### Return type

[**kotlin.collections.List&lt;EdgeFunctionMetrics&gt;**](EdgeFunctionMetrics.md)

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

<a id="edgeInvokeFunction"></a>
# **edgeInvokeFunction**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; edgeInvokeFunction(slug, requestBody)

Invoke function

Invoke an edge function directly. The request body is passed through to the function handler. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
val requestBody : kotlin.collections.Map<kotlin.String, kotlin.Any> = Object // kotlin.collections.Map<kotlin.String, kotlin.Any> | 
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.edgeInvokeFunction(slug, requestBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#edgeInvokeFunction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#edgeInvokeFunction")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **requestBody** | [**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)|  | [optional] |

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
 - **Accept**: application/json, text/plain

<a id="edgeListFunctions"></a>
# **edgeListFunctions**
> kotlin.collections.List&lt;EdgeFunction&gt; edgeListFunctions(page, pageSize, status)

List functions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val status : kotlin.String = status_example // kotlin.String | 
try {
    val result : kotlin.collections.List<EdgeFunction> = apiInstance.edgeListFunctions(page, pageSize, status)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#edgeListFunctions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#edgeListFunctions")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 20] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | **kotlin.String**|  | [optional] [enum: active, inactive, deploying, failed] |

### Return type

[**kotlin.collections.List&lt;EdgeFunction&gt;**](EdgeFunction.md)

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

<a id="edgeUpdateFunction"></a>
# **edgeUpdateFunction**
> EdgeFunction edgeUpdateFunction(slug, edgeFunctionUpdate)

Update function

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
val slug : kotlin.String = slug_example // kotlin.String | 
val edgeFunctionUpdate : EdgeFunctionUpdate =  // EdgeFunctionUpdate | 
try {
    val result : EdgeFunction = apiInstance.edgeUpdateFunction(slug, edgeFunctionUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#edgeUpdateFunction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#edgeUpdateFunction")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **edgeFunctionUpdate** | [**EdgeFunctionUpdate**](EdgeFunctionUpdate.md)|  | |

### Return type

[**EdgeFunction**](EdgeFunction.md)

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

<a id="functionsCreateFunction"></a>
# **functionsCreateFunction**
> FunctionsFunction functionsCreateFunction(functionsCreateFunctionRequest)

Create a function

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
val functionsCreateFunctionRequest : FunctionsCreateFunctionRequest =  // FunctionsCreateFunctionRequest | 
try {
    val result : FunctionsFunction = apiInstance.functionsCreateFunction(functionsCreateFunctionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#functionsCreateFunction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#functionsCreateFunction")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **functionsCreateFunctionRequest** | [**FunctionsCreateFunctionRequest**](FunctionsCreateFunctionRequest.md)|  | |

### Return type

[**FunctionsFunction**](FunctionsFunction.md)

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

<a id="functionsDeleteFunction"></a>
# **functionsDeleteFunction**
> functionsDeleteFunction(name)

Delete a function

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    apiInstance.functionsDeleteFunction(name)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#functionsDeleteFunction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#functionsDeleteFunction")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

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

<a id="functionsGetFunction"></a>
# **functionsGetFunction**
> FunctionsFunctionDetail functionsGetFunction(name)

Get a function (with triggers, recent invocations, secrets)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : FunctionsFunctionDetail = apiInstance.functionsGetFunction(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#functionsGetFunction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#functionsGetFunction")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**FunctionsFunctionDetail**](FunctionsFunctionDetail.md)

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

<a id="functionsGetFunctionLogs"></a>
# **functionsGetFunctionLogs**
> FunctionsGetFunctionLogs200Response functionsGetFunctionLogs(name)

Get the latest invocation logs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : FunctionsGetFunctionLogs200Response = apiInstance.functionsGetFunctionLogs(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#functionsGetFunctionLogs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#functionsGetFunctionLogs")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**FunctionsGetFunctionLogs200Response**](FunctionsGetFunctionLogs200Response.md)

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

<a id="functionsInvokeFunction"></a>
# **functionsInvokeFunction**
> FunctionsInvocation functionsInvokeFunction(name, functionsInvokeRequest)

Invoke a function (metered compute)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
val name : kotlin.String = name_example // kotlin.String | 
val functionsInvokeRequest : FunctionsInvokeRequest =  // FunctionsInvokeRequest | 
try {
    val result : FunctionsInvocation = apiInstance.functionsInvokeFunction(name, functionsInvokeRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#functionsInvokeFunction")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#functionsInvokeFunction")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **functionsInvokeRequest** | [**FunctionsInvokeRequest**](FunctionsInvokeRequest.md)|  | [optional] |

### Return type

[**FunctionsInvocation**](FunctionsInvocation.md)

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

<a id="functionsListDeployments"></a>
# **functionsListDeployments**
> FunctionsListFunctions200Response functionsListDeployments()

List deployed functions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
try {
    val result : FunctionsListFunctions200Response = apiInstance.functionsListDeployments()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#functionsListDeployments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#functionsListDeployments")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**FunctionsListFunctions200Response**](FunctionsListFunctions200Response.md)

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

<a id="functionsListFunctionSecrets"></a>
# **functionsListFunctionSecrets**
> FunctionsListFunctionSecrets200Response functionsListFunctionSecrets()

List function secrets (names only)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
try {
    val result : FunctionsListFunctionSecrets200Response = apiInstance.functionsListFunctionSecrets()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#functionsListFunctionSecrets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#functionsListFunctionSecrets")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**FunctionsListFunctionSecrets200Response**](FunctionsListFunctionSecrets200Response.md)

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

<a id="functionsListFunctions"></a>
# **functionsListFunctions**
> FunctionsListFunctions200Response functionsListFunctions()

List functions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
try {
    val result : FunctionsListFunctions200Response = apiInstance.functionsListFunctions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#functionsListFunctions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#functionsListFunctions")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**FunctionsListFunctions200Response**](FunctionsListFunctions200Response.md)

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

<a id="functionsListInvocations"></a>
# **functionsListInvocations**
> FunctionsListInvocations200Response functionsListInvocations(name, limit)

List a function&#39;s invocations

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
val name : kotlin.String = name_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : FunctionsListInvocations200Response = apiInstance.functionsListInvocations(name, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#functionsListInvocations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#functionsListInvocations")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**FunctionsListInvocations200Response**](FunctionsListInvocations200Response.md)

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

<a id="functionsListTriggers"></a>
# **functionsListTriggers**
> FunctionsListTriggers200Response functionsListTriggers()

List triggers across functions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = FunctionsApi()
try {
    val result : FunctionsListTriggers200Response = apiInstance.functionsListTriggers()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FunctionsApi#functionsListTriggers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FunctionsApi#functionsListTriggers")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**FunctionsListTriggers200Response**](FunctionsListTriggers200Response.md)

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

