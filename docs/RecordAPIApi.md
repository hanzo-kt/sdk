# RecordAPIApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**cloudApiControllerAddRecord**](RecordAPIApi.md#cloudApiControllerAddRecord) | **POST** /v1/cloud/add-record | Api Controller Add Record |
| [**cloudApiControllerAddRecords**](RecordAPIApi.md#cloudApiControllerAddRecords) | **POST** /v1/cloud/add-records | Api Controller Add Records |
| [**cloudApiControllerCommitRecord**](RecordAPIApi.md#cloudApiControllerCommitRecord) | **POST** /v1/cloud/commit-record | Api Controller Commit Record |
| [**cloudApiControllerCommitRecordSecond**](RecordAPIApi.md#cloudApiControllerCommitRecordSecond) | **POST** /v1/cloud/commit-record-second | Api Controller Commit Record Second |
| [**cloudApiControllerDeleteRecord**](RecordAPIApi.md#cloudApiControllerDeleteRecord) | **POST** /v1/cloud/delete-record | Api Controller Delete Record |
| [**cloudApiControllerGetRecord**](RecordAPIApi.md#cloudApiControllerGetRecord) | **GET** /v1/cloud/get-record | Api Controller Get Record |
| [**cloudApiControllerGetRecords**](RecordAPIApi.md#cloudApiControllerGetRecords) | **GET** /v1/cloud/get-records | Api Controller Get Records |
| [**cloudApiControllerQueryRecord**](RecordAPIApi.md#cloudApiControllerQueryRecord) | **GET** /v1/cloud/query-record | Api Controller Query Record |
| [**cloudApiControllerQueryRecordSecond**](RecordAPIApi.md#cloudApiControllerQueryRecordSecond) | **GET** /v1/cloud/query-record-second | Api Controller Query Record Second |
| [**cloudApiControllerUpdateRecord**](RecordAPIApi.md#cloudApiControllerUpdateRecord) | **POST** /v1/cloud/update-record | Api Controller Update Record |
| [**nexusAddRecord**](RecordAPIApi.md#nexusAddRecord) | **POST** /v1/nexus/add-record | add Record |
| [**nexusAddRecords**](RecordAPIApi.md#nexusAddRecords) | **POST** /v1/nexus/add-records | add Records |
| [**nexusCommitRecord**](RecordAPIApi.md#nexusCommitRecord) | **POST** /v1/nexus/commit-record | commit Record |
| [**nexusCommitRecordSecond**](RecordAPIApi.md#nexusCommitRecordSecond) | **POST** /v1/nexus/commit-record-second | commit Record Second |
| [**nexusDeleteRecord**](RecordAPIApi.md#nexusDeleteRecord) | **POST** /v1/nexus/delete-record | delete Record |
| [**nexusGetRecord**](RecordAPIApi.md#nexusGetRecord) | **GET** /v1/nexus/get-record | get Record |
| [**nexusGetRecords**](RecordAPIApi.md#nexusGetRecords) | **GET** /v1/nexus/get-records | get Records |
| [**nexusQueryRecord**](RecordAPIApi.md#nexusQueryRecord) | **GET** /v1/nexus/query-record | query Record |
| [**nexusQueryRecordSecond**](RecordAPIApi.md#nexusQueryRecordSecond) | **GET** /v1/nexus/query-record-second | query Record Second |
| [**nexusUpdateRecord**](RecordAPIApi.md#nexusUpdateRecord) | **POST** /v1/nexus/update-record | update Record |


<a id="cloudApiControllerAddRecord"></a>
# **cloudApiControllerAddRecord**
> CloudControllersResponse cloudApiControllerAddRecord(cloudObjectRecord)

Api Controller Add Record

add a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val cloudObjectRecord : CloudObjectRecord =  // CloudObjectRecord | The details of the record
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddRecord(cloudObjectRecord)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#cloudApiControllerAddRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#cloudApiControllerAddRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectRecord** | [**CloudObjectRecord**](CloudObjectRecord.md)| The details of the record | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerAddRecords"></a>
# **cloudApiControllerAddRecords**
> CloudControllersResponse cloudApiControllerAddRecords(cloudObjectRecord)

Api Controller Add Records

add multiple records

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val cloudObjectRecord : kotlin.collections.List<CloudObjectRecord> =  // kotlin.collections.List<CloudObjectRecord> | The details of the record
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerAddRecords(cloudObjectRecord)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#cloudApiControllerAddRecords")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#cloudApiControllerAddRecords")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectRecord** | [**kotlin.collections.List&lt;CloudObjectRecord&gt;**](CloudObjectRecord.md)| The details of the record | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerCommitRecord"></a>
# **cloudApiControllerCommitRecord**
> CloudControllersResponse cloudApiControllerCommitRecord(cloudObjectRecord)

Api Controller Commit Record

commit a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val cloudObjectRecord : CloudObjectRecord =  // CloudObjectRecord | The details of the record
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerCommitRecord(cloudObjectRecord)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#cloudApiControllerCommitRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#cloudApiControllerCommitRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectRecord** | [**CloudObjectRecord**](CloudObjectRecord.md)| The details of the record | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerCommitRecordSecond"></a>
# **cloudApiControllerCommitRecordSecond**
> CloudControllersResponse cloudApiControllerCommitRecordSecond(cloudObjectRecord)

Api Controller Commit Record Second

commit a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val cloudObjectRecord : CloudObjectRecord =  // CloudObjectRecord | The details of the record
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerCommitRecordSecond(cloudObjectRecord)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#cloudApiControllerCommitRecordSecond")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#cloudApiControllerCommitRecordSecond")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectRecord** | [**CloudObjectRecord**](CloudObjectRecord.md)| The details of the record | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerDeleteRecord"></a>
# **cloudApiControllerDeleteRecord**
> CloudControllersResponse cloudApiControllerDeleteRecord(cloudObjectRecord)

Api Controller Delete Record

delete a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val cloudObjectRecord : CloudObjectRecord =  // CloudObjectRecord | The details of the record
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerDeleteRecord(cloudObjectRecord)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#cloudApiControllerDeleteRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#cloudApiControllerDeleteRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectRecord** | [**CloudObjectRecord**](CloudObjectRecord.md)| The details of the record | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="cloudApiControllerGetRecord"></a>
# **cloudApiControllerGetRecord**
> CloudObjectRecord cloudApiControllerGetRecord(id)

Api Controller Get Record

get record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the record
try {
    val result : CloudObjectRecord = apiInstance.cloudApiControllerGetRecord(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#cloudApiControllerGetRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#cloudApiControllerGetRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the record | |

### Return type

[**CloudObjectRecord**](CloudObjectRecord.md)

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

<a id="cloudApiControllerGetRecords"></a>
# **cloudApiControllerGetRecords**
> CloudObjectRecord cloudApiControllerGetRecords(pageSize, p)

Api Controller Get Records

get all records

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The number of the page
try {
    val result : CloudObjectRecord = apiInstance.cloudApiControllerGetRecords(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#cloudApiControllerGetRecords")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#cloudApiControllerGetRecords")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The number of the page | |

### Return type

[**CloudObjectRecord**](CloudObjectRecord.md)

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

<a id="cloudApiControllerQueryRecord"></a>
# **cloudApiControllerQueryRecord**
> CloudObjectRecord cloudApiControllerQueryRecord(id)

Api Controller Query Record

query record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the record
try {
    val result : CloudObjectRecord = apiInstance.cloudApiControllerQueryRecord(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#cloudApiControllerQueryRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#cloudApiControllerQueryRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the record | |

### Return type

[**CloudObjectRecord**](CloudObjectRecord.md)

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

<a id="cloudApiControllerQueryRecordSecond"></a>
# **cloudApiControllerQueryRecordSecond**
> CloudObjectRecord cloudApiControllerQueryRecordSecond(id)

Api Controller Query Record Second

query record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the record
try {
    val result : CloudObjectRecord = apiInstance.cloudApiControllerQueryRecordSecond(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#cloudApiControllerQueryRecordSecond")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#cloudApiControllerQueryRecordSecond")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the record | |

### Return type

[**CloudObjectRecord**](CloudObjectRecord.md)

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

<a id="cloudApiControllerUpdateRecord"></a>
# **cloudApiControllerUpdateRecord**
> CloudControllersResponse cloudApiControllerUpdateRecord(id, cloudObjectRecord)

Api Controller Update Record

update record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the record
val cloudObjectRecord : CloudObjectRecord =  // CloudObjectRecord | The details of the record
try {
    val result : CloudControllersResponse = apiInstance.cloudApiControllerUpdateRecord(id, cloudObjectRecord)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#cloudApiControllerUpdateRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#cloudApiControllerUpdateRecord")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the record | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectRecord** | [**CloudObjectRecord**](CloudObjectRecord.md)| The details of the record | |

### Return type

[**CloudControllersResponse**](CloudControllersResponse.md)

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

<a id="nexusAddRecord"></a>
# **nexusAddRecord**
> NexusResponse nexusAddRecord(cloudObjectRecord)

add Record

Add a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val cloudObjectRecord : CloudObjectRecord =  // CloudObjectRecord | The details of the record
try {
    val result : NexusResponse = apiInstance.nexusAddRecord(cloudObjectRecord)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#nexusAddRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#nexusAddRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectRecord** | [**CloudObjectRecord**](CloudObjectRecord.md)| The details of the record | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusAddRecords"></a>
# **nexusAddRecords**
> NexusResponse nexusAddRecords(cloudObjectRecord)

add Records

Add multiple records

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val cloudObjectRecord : kotlin.collections.List<CloudObjectRecord> =  // kotlin.collections.List<CloudObjectRecord> | The details of the records
try {
    val result : NexusResponse = apiInstance.nexusAddRecords(cloudObjectRecord)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#nexusAddRecords")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#nexusAddRecords")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectRecord** | [**kotlin.collections.List&lt;CloudObjectRecord&gt;**](CloudObjectRecord.md)| The details of the records | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusCommitRecord"></a>
# **nexusCommitRecord**
> NexusResponse nexusCommitRecord(cloudObjectRecord)

commit Record

Commit a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val cloudObjectRecord : CloudObjectRecord =  // CloudObjectRecord | The details of the record
try {
    val result : NexusResponse = apiInstance.nexusCommitRecord(cloudObjectRecord)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#nexusCommitRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#nexusCommitRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectRecord** | [**CloudObjectRecord**](CloudObjectRecord.md)| The details of the record | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusCommitRecordSecond"></a>
# **nexusCommitRecordSecond**
> NexusResponse nexusCommitRecordSecond(cloudObjectRecord)

commit Record Second

Commit a record (secondary)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val cloudObjectRecord : CloudObjectRecord =  // CloudObjectRecord | The details of the record
try {
    val result : NexusResponse = apiInstance.nexusCommitRecordSecond(cloudObjectRecord)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#nexusCommitRecordSecond")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#nexusCommitRecordSecond")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectRecord** | [**CloudObjectRecord**](CloudObjectRecord.md)| The details of the record | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusDeleteRecord"></a>
# **nexusDeleteRecord**
> NexusResponse nexusDeleteRecord(cloudObjectRecord)

delete Record

Delete a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val cloudObjectRecord : CloudObjectRecord =  // CloudObjectRecord | The details of the record
try {
    val result : NexusResponse = apiInstance.nexusDeleteRecord(cloudObjectRecord)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#nexusDeleteRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#nexusDeleteRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectRecord** | [**CloudObjectRecord**](CloudObjectRecord.md)| The details of the record | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

<a id="nexusGetRecord"></a>
# **nexusGetRecord**
> CloudObjectRecord nexusGetRecord(id)

get Record

Get a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the record
try {
    val result : CloudObjectRecord = apiInstance.nexusGetRecord(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#nexusGetRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#nexusGetRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the record | |

### Return type

[**CloudObjectRecord**](CloudObjectRecord.md)

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

<a id="nexusGetRecords"></a>
# **nexusGetRecords**
> CloudObjectRecord nexusGetRecords(pageSize, p)

get Records

Get all records

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The page number
try {
    val result : CloudObjectRecord = apiInstance.nexusGetRecords(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#nexusGetRecords")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#nexusGetRecords")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The page number | |

### Return type

[**CloudObjectRecord**](CloudObjectRecord.md)

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

<a id="nexusQueryRecord"></a>
# **nexusQueryRecord**
> CloudObjectRecord nexusQueryRecord(id)

query Record

Query a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the record
try {
    val result : CloudObjectRecord = apiInstance.nexusQueryRecord(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#nexusQueryRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#nexusQueryRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the record | |

### Return type

[**CloudObjectRecord**](CloudObjectRecord.md)

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

<a id="nexusQueryRecordSecond"></a>
# **nexusQueryRecordSecond**
> CloudObjectRecord nexusQueryRecordSecond(id)

query Record Second

Query a record (secondary)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the record
try {
    val result : CloudObjectRecord = apiInstance.nexusQueryRecordSecond(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#nexusQueryRecordSecond")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#nexusQueryRecordSecond")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of the record | |

### Return type

[**CloudObjectRecord**](CloudObjectRecord.md)

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

<a id="nexusUpdateRecord"></a>
# **nexusUpdateRecord**
> NexusResponse nexusUpdateRecord(id, cloudObjectRecord)

update Record

Update a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RecordAPIApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the record
val cloudObjectRecord : CloudObjectRecord =  // CloudObjectRecord | The details of the record
try {
    val result : NexusResponse = apiInstance.nexusUpdateRecord(id, cloudObjectRecord)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecordAPIApi#nexusUpdateRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecordAPIApi#nexusUpdateRecord")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the record | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **cloudObjectRecord** | [**CloudObjectRecord**](CloudObjectRecord.md)| The details of the record | |

### Return type

[**NexusResponse**](NexusResponse.md)

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

