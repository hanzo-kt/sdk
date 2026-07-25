# DatasetsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**consoleCreateDataset**](DatasetsApi.md#consoleCreateDataset) | **POST** /v1/console/datasets | Create a dataset |
| [**consoleDeleteDatasetRun**](DatasetsApi.md#consoleDeleteDatasetRun) | **DELETE** /v1/console/datasets/{datasetName}/runs/{runName} | Delete a dataset run and all its run items |
| [**consoleGetDataset**](DatasetsApi.md#consoleGetDataset) | **GET** /v1/console/datasets/{datasetName} | Get a dataset by name |
| [**consoleGetDatasetRun**](DatasetsApi.md#consoleGetDatasetRun) | **GET** /v1/console/datasets/{datasetName}/runs/{runName} | Get a dataset run and its items |
| [**consoleListDatasetRuns**](DatasetsApi.md#consoleListDatasetRuns) | **GET** /v1/console/datasets/{datasetName}/runs | Get dataset runs |
| [**consoleListDatasets**](DatasetsApi.md#consoleListDatasets) | **GET** /v1/console/datasets | Get all datasets |
| [**evalsPostV1EvalsDatasetItems**](DatasetsApi.md#evalsPostV1EvalsDatasetItems) | **POST** /v1/evals/dataset-items | Add an item (input + optional expected output) to a dataset |
| [**evalsPostV1EvalsDatasets**](DatasetsApi.md#evalsPostV1EvalsDatasets) | **POST** /v1/evals/datasets | Create a dataset |


<a id="consoleCreateDataset"></a>
# **consoleCreateDataset**
> ConsoleDataset consoleCreateDataset(consoleCreateDatasetRequest)

Create a dataset

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatasetsApi()
val consoleCreateDatasetRequest : ConsoleCreateDatasetRequest =  // ConsoleCreateDatasetRequest | 
try {
    val result : ConsoleDataset = apiInstance.consoleCreateDataset(consoleCreateDatasetRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatasetsApi#consoleCreateDataset")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatasetsApi#consoleCreateDataset")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleCreateDatasetRequest** | [**ConsoleCreateDatasetRequest**](ConsoleCreateDatasetRequest.md)|  | |

### Return type

[**ConsoleDataset**](ConsoleDataset.md)

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

<a id="consoleDeleteDatasetRun"></a>
# **consoleDeleteDatasetRun**
> ConsoleDeleteDatasetItem200Response consoleDeleteDatasetRun(datasetName, runName)

Delete a dataset run and all its run items

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatasetsApi()
val datasetName : kotlin.String = datasetName_example // kotlin.String | 
val runName : kotlin.String = runName_example // kotlin.String | 
try {
    val result : ConsoleDeleteDatasetItem200Response = apiInstance.consoleDeleteDatasetRun(datasetName, runName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatasetsApi#consoleDeleteDatasetRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatasetsApi#consoleDeleteDatasetRun")
    e.printStackTrace()
}
```

### Parameters
| **datasetName** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **runName** | **kotlin.String**|  | |

### Return type

[**ConsoleDeleteDatasetItem200Response**](ConsoleDeleteDatasetItem200Response.md)

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

<a id="consoleGetDataset"></a>
# **consoleGetDataset**
> ConsoleDataset consoleGetDataset(datasetName)

Get a dataset by name

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatasetsApi()
val datasetName : kotlin.String = datasetName_example // kotlin.String | 
try {
    val result : ConsoleDataset = apiInstance.consoleGetDataset(datasetName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatasetsApi#consoleGetDataset")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatasetsApi#consoleGetDataset")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **datasetName** | **kotlin.String**|  | |

### Return type

[**ConsoleDataset**](ConsoleDataset.md)

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

<a id="consoleGetDatasetRun"></a>
# **consoleGetDatasetRun**
> ConsoleGetDatasetRun200Response consoleGetDatasetRun(datasetName, runName)

Get a dataset run and its items

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatasetsApi()
val datasetName : kotlin.String = datasetName_example // kotlin.String | 
val runName : kotlin.String = runName_example // kotlin.String | 
try {
    val result : ConsoleGetDatasetRun200Response = apiInstance.consoleGetDatasetRun(datasetName, runName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatasetsApi#consoleGetDatasetRun")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatasetsApi#consoleGetDatasetRun")
    e.printStackTrace()
}
```

### Parameters
| **datasetName** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **runName** | **kotlin.String**|  | |

### Return type

[**ConsoleGetDatasetRun200Response**](ConsoleGetDatasetRun200Response.md)

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

<a id="consoleListDatasetRuns"></a>
# **consoleListDatasetRuns**
> ConsoleListDatasetRuns200Response consoleListDatasetRuns(datasetName, page, limit)

Get dataset runs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatasetsApi()
val datasetName : kotlin.String = datasetName_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : ConsoleListDatasetRuns200Response = apiInstance.consoleListDatasetRuns(datasetName, page, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatasetsApi#consoleListDatasetRuns")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatasetsApi#consoleListDatasetRuns")
    e.printStackTrace()
}
```

### Parameters
| **datasetName** | **kotlin.String**|  | |
| **page** | **kotlin.Int**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**ConsoleListDatasetRuns200Response**](ConsoleListDatasetRuns200Response.md)

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

<a id="consoleListDatasets"></a>
# **consoleListDatasets**
> ConsoleListDatasets200Response consoleListDatasets(page, limit)

Get all datasets

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatasetsApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : ConsoleListDatasets200Response = apiInstance.consoleListDatasets(page, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatasetsApi#consoleListDatasets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatasetsApi#consoleListDatasets")
    e.printStackTrace()
}
```

### Parameters
| **page** | **kotlin.Int**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] |

### Return type

[**ConsoleListDatasets200Response**](ConsoleListDatasets200Response.md)

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

<a id="evalsPostV1EvalsDatasetItems"></a>
# **evalsPostV1EvalsDatasetItems**
> EvalsDatasetItem evalsPostV1EvalsDatasetItems(evalsDatasetItemCreate)

Add an item (input + optional expected output) to a dataset

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatasetsApi()
val evalsDatasetItemCreate : EvalsDatasetItemCreate =  // EvalsDatasetItemCreate | 
try {
    val result : EvalsDatasetItem = apiInstance.evalsPostV1EvalsDatasetItems(evalsDatasetItemCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatasetsApi#evalsPostV1EvalsDatasetItems")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatasetsApi#evalsPostV1EvalsDatasetItems")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **evalsDatasetItemCreate** | [**EvalsDatasetItemCreate**](EvalsDatasetItemCreate.md)|  | |

### Return type

[**EvalsDatasetItem**](EvalsDatasetItem.md)

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

<a id="evalsPostV1EvalsDatasets"></a>
# **evalsPostV1EvalsDatasets**
> EvalsDataset evalsPostV1EvalsDatasets(evalsDatasetCreate)

Create a dataset

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = DatasetsApi()
val evalsDatasetCreate : EvalsDatasetCreate =  // EvalsDatasetCreate | 
try {
    val result : EvalsDataset = apiInstance.evalsPostV1EvalsDatasets(evalsDatasetCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatasetsApi#evalsPostV1EvalsDatasets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatasetsApi#evalsPostV1EvalsDatasets")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **evalsDatasetCreate** | [**EvalsDatasetCreate**](EvalsDatasetCreate.md)|  | |

### Return type

[**EvalsDataset**](EvalsDataset.md)

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

