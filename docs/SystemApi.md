# SystemApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**iamApiControllerAddAdapter**](SystemApi.md#iamApiControllerAddAdapter) | **POST** /v1/iam/adapters | Api Controller Add Adapter |
| [**iamApiControllerAddCert**](SystemApi.md#iamApiControllerAddCert) | **POST** /v1/iam/certs | Api Controller Add Cert |
| [**iamApiControllerAddForm**](SystemApi.md#iamApiControllerAddForm) | **POST** /v1/iam/forms | Api Controller Add Form |
| [**iamApiControllerAddRecord**](SystemApi.md#iamApiControllerAddRecord) | **POST** /v1/iam/records | Api Controller Add Record |
| [**iamApiControllerAddSyncer**](SystemApi.md#iamApiControllerAddSyncer) | **POST** /v1/iam/syncers | Api Controller Add Syncer |
| [**iamApiControllerAddTicket**](SystemApi.md#iamApiControllerAddTicket) | **POST** /v1/iam/tickets | Api Controller Add Ticket |
| [**iamApiControllerAddTicketMessage**](SystemApi.md#iamApiControllerAddTicketMessage) | **POST** /v1/iam/ticket-messages | Api Controller Add Ticket Message |
| [**iamApiControllerDeleteAdapter**](SystemApi.md#iamApiControllerDeleteAdapter) | **DELETE** /v1/iam/adapters/{id} | Api Controller Delete Adapter |
| [**iamApiControllerDeleteCert**](SystemApi.md#iamApiControllerDeleteCert) | **DELETE** /v1/iam/certs/{id} | Api Controller Delete Cert |
| [**iamApiControllerDeleteForm**](SystemApi.md#iamApiControllerDeleteForm) | **DELETE** /v1/iam/forms/{id} | Api Controller Delete Form |
| [**iamApiControllerDeleteSyncer**](SystemApi.md#iamApiControllerDeleteSyncer) | **DELETE** /v1/iam/syncers/{id} | Api Controller Delete Syncer |
| [**iamApiControllerDeleteTicket**](SystemApi.md#iamApiControllerDeleteTicket) | **DELETE** /v1/iam/tickets/{id} | Api Controller Delete Ticket |
| [**iamApiControllerGetAdapter**](SystemApi.md#iamApiControllerGetAdapter) | **GET** /v1/iam/adapters/{id} | Api Controller Get Adapter |
| [**iamApiControllerGetAdapters**](SystemApi.md#iamApiControllerGetAdapters) | **GET** /v1/iam/adapters | Api Controller Get Adapters |
| [**iamApiControllerGetCert**](SystemApi.md#iamApiControllerGetCert) | **GET** /v1/iam/certs/{id} | Api Controller Get Cert |
| [**iamApiControllerGetCerts**](SystemApi.md#iamApiControllerGetCerts) | **GET** /v1/iam/certs | Api Controller Get Certs |
| [**iamApiControllerGetDashboard**](SystemApi.md#iamApiControllerGetDashboard) | **GET** /v1/iam/dashboard | Api Controller Get Dashboard |
| [**iamApiControllerGetForm**](SystemApi.md#iamApiControllerGetForm) | **GET** /v1/iam/forms/{id} | Api Controller Get Form |
| [**iamApiControllerGetForms**](SystemApi.md#iamApiControllerGetForms) | **GET** /v1/iam/forms | Api Controller Get Forms |
| [**iamApiControllerGetGlobalCerts**](SystemApi.md#iamApiControllerGetGlobalCerts) | **GET** /v1/iam/global-certs | Api Controller Get Global Certs |
| [**iamApiControllerGetGlobalForms**](SystemApi.md#iamApiControllerGetGlobalForms) | **GET** /v1/iam/global-forms | Api Controller Get Global Forms |
| [**iamApiControllerGetMetrics**](SystemApi.md#iamApiControllerGetMetrics) | **GET** /v1/iam/metrics | Api Controller Get Metrics |
| [**iamApiControllerGetPrometheusInfo**](SystemApi.md#iamApiControllerGetPrometheusInfo) | **GET** /v1/iam/metrics/prometheus | Api Controller Get Prometheus Info |
| [**iamApiControllerGetRecords**](SystemApi.md#iamApiControllerGetRecords) | **GET** /v1/iam/records | Api Controller Get Records |
| [**iamApiControllerGetRecordsByFilter**](SystemApi.md#iamApiControllerGetRecordsByFilter) | **GET** /v1/iam/records-filters/{id} | Api Controller Get Records By Filter |
| [**iamApiControllerGetSyncer**](SystemApi.md#iamApiControllerGetSyncer) | **GET** /v1/iam/syncers/{id} | Api Controller Get Syncer |
| [**iamApiControllerGetSyncers**](SystemApi.md#iamApiControllerGetSyncers) | **GET** /v1/iam/syncers | Api Controller Get Syncers |
| [**iamApiControllerGetSystemInfo**](SystemApi.md#iamApiControllerGetSystemInfo) | **GET** /v1/iam/system | Api Controller Get System Info |
| [**iamApiControllerGetTicket**](SystemApi.md#iamApiControllerGetTicket) | **GET** /v1/iam/tickets/{id} | Api Controller Get Ticket |
| [**iamApiControllerGetTickets**](SystemApi.md#iamApiControllerGetTickets) | **GET** /v1/iam/tickets | Api Controller Get Tickets |
| [**iamApiControllerGetVersionInfo**](SystemApi.md#iamApiControllerGetVersionInfo) | **GET** /v1/iam/version-infos/{id} | Api Controller Get Version Info |
| [**iamApiControllerGetWebhookEventType**](SystemApi.md#iamApiControllerGetWebhookEventType) | **GET** /v1/iam/webhook-events/{id} | Api Controller Get Webhook Event Type |
| [**iamApiControllerGetWechatQRCode**](SystemApi.md#iamApiControllerGetWechatQRCode) | **GET** /v1/iam/qrcodes/{id} | Api Controller Get Wechat QR Code |
| [**iamApiControllerHandleOfficialAccountEvent**](SystemApi.md#iamApiControllerHandleOfficialAccountEvent) | **POST** /v1/iam/webhook | Api Controller Handle Official Account Event |
| [**iamApiControllerHealth**](SystemApi.md#iamApiControllerHealth) | **GET** /v1/iam/health | Api Controller Health |
| [**iamApiControllerRefreshEngines**](SystemApi.md#iamApiControllerRefreshEngines) | **POST** /v1/iam/refresh-engines | Api Controller Refresh Engines |
| [**iamApiControllerRunSyncer**](SystemApi.md#iamApiControllerRunSyncer) | **GET** /v1/iam/syncers/run | Api Controller Run Syncer |
| [**iamApiControllerSendEmail**](SystemApi.md#iamApiControllerSendEmail) | **POST** /v1/iam/messaging/email | Api Controller Send Email |
| [**iamApiControllerSendNotification**](SystemApi.md#iamApiControllerSendNotification) | **POST** /v1/iam/messaging/notification | Api Controller Send Notification |
| [**iamApiControllerSendSms**](SystemApi.md#iamApiControllerSendSms) | **POST** /v1/iam/messaging/sms | Api Controller Send Sms |
| [**iamApiControllerUpdateAdapter**](SystemApi.md#iamApiControllerUpdateAdapter) | **PUT** /v1/iam/adapters/{id} | Api Controller Update Adapter |
| [**iamApiControllerUpdateCert**](SystemApi.md#iamApiControllerUpdateCert) | **PUT** /v1/iam/certs/{id} | Api Controller Update Cert |
| [**iamApiControllerUpdateForm**](SystemApi.md#iamApiControllerUpdateForm) | **PUT** /v1/iam/forms/{id} | Api Controller Update Form |
| [**iamApiControllerUpdateSyncer**](SystemApi.md#iamApiControllerUpdateSyncer) | **PUT** /v1/iam/syncers/{id} | Api Controller Update Syncer |
| [**iamApiControllerUpdateTicket**](SystemApi.md#iamApiControllerUpdateTicket) | **PUT** /v1/iam/tickets/{id} | Api Controller Update Ticket |
| [**paasListTemplates**](SystemApi.md#paasListTemplates) | **GET** /v1/paas/system/templates | List available templates |
| [**tasksTasksCluster**](SystemApi.md#tasksTasksCluster) | **GET** /v1/tasks/cluster | Cluster status (open probe) |
| [**tasksTasksClusterHealth**](SystemApi.md#tasksTasksClusterHealth) | **GET** /v1/tasks/cluster/health | Cluster health (open probe) |
| [**tasksTasksHealth**](SystemApi.md#tasksTasksHealth) | **GET** /v1/tasks/health | Liveness probe |
| [**tasksTasksSettings**](SystemApi.md#tasksTasksSettings) | **GET** /v1/tasks/settings | Capability flags (open bootstrap) |


<a id="iamApiControllerAddAdapter"></a>
# **iamApiControllerAddAdapter**
> IamControllersResponse iamApiControllerAddAdapter(iamObjectAdapter)

Api Controller Add Adapter

add adapter

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val iamObjectAdapter : IamObjectAdapter =  // IamObjectAdapter | The details of the adapter
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddAdapter(iamObjectAdapter)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerAddAdapter")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerAddAdapter")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectAdapter** | [**IamObjectAdapter**](IamObjectAdapter.md)| The details of the adapter | |

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

<a id="iamApiControllerAddCert"></a>
# **iamApiControllerAddCert**
> IamControllersResponse iamApiControllerAddCert(iamObjectCert)

Api Controller Add Cert

add cert

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val iamObjectCert : IamObjectCert =  // IamObjectCert | The details of the cert
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddCert(iamObjectCert)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerAddCert")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerAddCert")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectCert** | [**IamObjectCert**](IamObjectCert.md)| The details of the cert | |

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

<a id="iamApiControllerAddForm"></a>
# **iamApiControllerAddForm**
> IamControllersResponse iamApiControllerAddForm(iamObjectForm)

Api Controller Add Form

add form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val iamObjectForm : IamObjectForm =  // IamObjectForm | The details of the form
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddForm(iamObjectForm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerAddForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerAddForm")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectForm** | [**IamObjectForm**](IamObjectForm.md)| The details of the form | |

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

<a id="iamApiControllerAddRecord"></a>
# **iamApiControllerAddRecord**
> IamControllersResponse iamApiControllerAddRecord(body)

Api Controller Add Record

add a record

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val body : kotlin.Any = Object // kotlin.Any | The details of the record
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddRecord(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerAddRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerAddRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The details of the record | |

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

<a id="iamApiControllerAddSyncer"></a>
# **iamApiControllerAddSyncer**
> IamControllersResponse iamApiControllerAddSyncer(iamObjectSyncer)

Api Controller Add Syncer

add syncer

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val iamObjectSyncer : IamObjectSyncer =  // IamObjectSyncer | The details of the syncer
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddSyncer(iamObjectSyncer)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerAddSyncer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerAddSyncer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectSyncer** | [**IamObjectSyncer**](IamObjectSyncer.md)| The details of the syncer | |

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

<a id="iamApiControllerAddTicket"></a>
# **iamApiControllerAddTicket**
> IamControllersResponse iamApiControllerAddTicket(iamObjectTicket)

Api Controller Add Ticket

add ticket

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val iamObjectTicket : IamObjectTicket =  // IamObjectTicket | The details of the ticket
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddTicket(iamObjectTicket)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerAddTicket")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerAddTicket")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectTicket** | [**IamObjectTicket**](IamObjectTicket.md)| The details of the ticket | |

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

<a id="iamApiControllerAddTicketMessage"></a>
# **iamApiControllerAddTicketMessage**
> IamControllersResponse iamApiControllerAddTicketMessage(id, iamObjectTicketMessage)

Api Controller Add Ticket Message

add a message to a ticket

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the ticket
val iamObjectTicketMessage : IamObjectTicketMessage =  // IamObjectTicketMessage | The message to add
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddTicketMessage(id, iamObjectTicketMessage)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerAddTicketMessage")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerAddTicketMessage")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the ticket | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectTicketMessage** | [**IamObjectTicketMessage**](IamObjectTicketMessage.md)| The message to add | |

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

<a id="iamApiControllerDeleteAdapter"></a>
# **iamApiControllerDeleteAdapter**
> IamControllersResponse iamApiControllerDeleteAdapter(id, iamObjectAdapter)

Api Controller Delete Adapter

delete adapter

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectAdapter : IamObjectAdapter =  // IamObjectAdapter | The details of the adapter
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteAdapter(id, iamObjectAdapter)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerDeleteAdapter")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerDeleteAdapter")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectAdapter** | [**IamObjectAdapter**](IamObjectAdapter.md)| The details of the adapter | |

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

<a id="iamApiControllerDeleteCert"></a>
# **iamApiControllerDeleteCert**
> IamControllersResponse iamApiControllerDeleteCert(id, iamObjectCert)

Api Controller Delete Cert

delete cert

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectCert : IamObjectCert =  // IamObjectCert | The details of the cert
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteCert(id, iamObjectCert)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerDeleteCert")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerDeleteCert")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectCert** | [**IamObjectCert**](IamObjectCert.md)| The details of the cert | |

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

<a id="iamApiControllerDeleteForm"></a>
# **iamApiControllerDeleteForm**
> IamControllersResponse iamApiControllerDeleteForm(id, iamObjectForm)

Api Controller Delete Form

delete form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectForm : IamObjectForm =  // IamObjectForm | The details of the form
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteForm(id, iamObjectForm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerDeleteForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerDeleteForm")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectForm** | [**IamObjectForm**](IamObjectForm.md)| The details of the form | |

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

<a id="iamApiControllerDeleteSyncer"></a>
# **iamApiControllerDeleteSyncer**
> IamControllersResponse iamApiControllerDeleteSyncer(id, iamObjectSyncer)

Api Controller Delete Syncer

delete syncer

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectSyncer : IamObjectSyncer =  // IamObjectSyncer | The details of the syncer
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteSyncer(id, iamObjectSyncer)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerDeleteSyncer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerDeleteSyncer")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectSyncer** | [**IamObjectSyncer**](IamObjectSyncer.md)| The details of the syncer | |

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

<a id="iamApiControllerDeleteTicket"></a>
# **iamApiControllerDeleteTicket**
> IamControllersResponse iamApiControllerDeleteTicket(id, iamObjectTicket)

Api Controller Delete Ticket

delete ticket

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectTicket : IamObjectTicket =  // IamObjectTicket | The details of the ticket
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteTicket(id, iamObjectTicket)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerDeleteTicket")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerDeleteTicket")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectTicket** | [**IamObjectTicket**](IamObjectTicket.md)| The details of the ticket | |

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

<a id="iamApiControllerGetAdapter"></a>
# **iamApiControllerGetAdapter**
> IamObjectAdapter iamApiControllerGetAdapter(id)

Api Controller Get Adapter

get adapter

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the adapter
try {
    val result : IamObjectAdapter = apiInstance.iamApiControllerGetAdapter(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetAdapter")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetAdapter")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the adapter | |

### Return type

[**IamObjectAdapter**](IamObjectAdapter.md)

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

<a id="iamApiControllerGetAdapters"></a>
# **iamApiControllerGetAdapters**
> kotlin.collections.List&lt;IamObjectAdapter&gt; iamApiControllerGetAdapters(owner)

Api Controller Get Adapters

get adapters

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of adapters
try {
    val result : kotlin.collections.List<IamObjectAdapter> = apiInstance.iamApiControllerGetAdapters(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetAdapters")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetAdapters")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of adapters | |

### Return type

[**kotlin.collections.List&lt;IamObjectAdapter&gt;**](IamObjectAdapter.md)

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

<a id="iamApiControllerGetCert"></a>
# **iamApiControllerGetCert**
> IamObjectCert iamApiControllerGetCert(id)

Api Controller Get Cert

get cert

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the cert
try {
    val result : IamObjectCert = apiInstance.iamApiControllerGetCert(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetCert")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetCert")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the cert | |

### Return type

[**IamObjectCert**](IamObjectCert.md)

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

<a id="iamApiControllerGetCerts"></a>
# **iamApiControllerGetCerts**
> kotlin.collections.List&lt;IamObjectCert&gt; iamApiControllerGetCerts(owner)

Api Controller Get Certs

get certs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of certs
try {
    val result : kotlin.collections.List<IamObjectCert> = apiInstance.iamApiControllerGetCerts(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetCerts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetCerts")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of certs | |

### Return type

[**kotlin.collections.List&lt;IamObjectCert&gt;**](IamObjectCert.md)

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

<a id="iamApiControllerGetDashboard"></a>
# **iamApiControllerGetDashboard**
> IamControllersResponse iamApiControllerGetDashboard()

Api Controller Get Dashboard

get information of dashboard

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerGetDashboard()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetDashboard")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetDashboard")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="iamApiControllerGetForm"></a>
# **iamApiControllerGetForm**
> IamObjectForm iamApiControllerGetForm(id)

Api Controller Get Form

get form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of form
try {
    val result : IamObjectForm = apiInstance.iamApiControllerGetForm(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetForm")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id (owner/name) of form | |

### Return type

[**IamObjectForm**](IamObjectForm.md)

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

<a id="iamApiControllerGetForms"></a>
# **iamApiControllerGetForms**
> kotlin.collections.List&lt;IamObjectForm&gt; iamApiControllerGetForms(owner)

Api Controller Get Forms

get forms

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of form
try {
    val result : kotlin.collections.List<IamObjectForm> = apiInstance.iamApiControllerGetForms(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetForms")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetForms")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of form | |

### Return type

[**kotlin.collections.List&lt;IamObjectForm&gt;**](IamObjectForm.md)

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

<a id="iamApiControllerGetGlobalCerts"></a>
# **iamApiControllerGetGlobalCerts**
> kotlin.collections.List&lt;IamObjectCert&gt; iamApiControllerGetGlobalCerts()

Api Controller Get Global Certs

get global certs

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : kotlin.collections.List<IamObjectCert> = apiInstance.iamApiControllerGetGlobalCerts()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetGlobalCerts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetGlobalCerts")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;IamObjectCert&gt;**](IamObjectCert.md)

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

<a id="iamApiControllerGetGlobalForms"></a>
# **iamApiControllerGetGlobalForms**
> kotlin.collections.List&lt;IamObjectForm&gt; iamApiControllerGetGlobalForms()

Api Controller Get Global Forms

get global forms

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : kotlin.collections.List<IamObjectForm> = apiInstance.iamApiControllerGetGlobalForms()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetGlobalForms")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetGlobalForms")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;IamObjectForm&gt;**](IamObjectForm.md)

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

<a id="iamApiControllerGetMetrics"></a>
# **iamApiControllerGetMetrics**
> kotlin.Any iamApiControllerGetMetrics()

Api Controller Get Metrics

get Prometheus metrics

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : kotlin.Any = apiInstance.iamApiControllerGetMetrics()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetMetrics")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetMetrics")
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

<a id="iamApiControllerGetPrometheusInfo"></a>
# **iamApiControllerGetPrometheusInfo**
> IamObjectPrometheusInfo iamApiControllerGetPrometheusInfo()

Api Controller Get Prometheus Info

get Prometheus Info

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : IamObjectPrometheusInfo = apiInstance.iamApiControllerGetPrometheusInfo()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetPrometheusInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetPrometheusInfo")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**IamObjectPrometheusInfo**](IamObjectPrometheusInfo.md)

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

<a id="iamApiControllerGetRecords"></a>
# **iamApiControllerGetRecords**
> kotlin.Any iamApiControllerGetRecords(pageSize, p)

Api Controller Get Records

get all records

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val pageSize : kotlin.String = pageSize_example // kotlin.String | The size of each page
val p : kotlin.String = p_example // kotlin.String | The number of the page
try {
    val result : kotlin.Any = apiInstance.iamApiControllerGetRecords(pageSize, p)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetRecords")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetRecords")
    e.printStackTrace()
}
```

### Parameters
| **pageSize** | **kotlin.String**| The size of each page | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **p** | **kotlin.String**| The number of the page | |

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

<a id="iamApiControllerGetRecordsByFilter"></a>
# **iamApiControllerGetRecordsByFilter**
> kotlin.Any iamApiControllerGetRecordsByFilter(id, body)

Api Controller Get Records By Filter

get records by filter

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val body : kotlin.String = body_example // kotlin.String | filter Record message
try {
    val result : kotlin.Any = apiInstance.iamApiControllerGetRecordsByFilter(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetRecordsByFilter")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetRecordsByFilter")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.String**| filter Record message | |

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

<a id="iamApiControllerGetSyncer"></a>
# **iamApiControllerGetSyncer**
> IamObjectSyncer iamApiControllerGetSyncer(id)

Api Controller Get Syncer

get syncer

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the syncer
try {
    val result : IamObjectSyncer = apiInstance.iamApiControllerGetSyncer(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetSyncer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetSyncer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the syncer | |

### Return type

[**IamObjectSyncer**](IamObjectSyncer.md)

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

<a id="iamApiControllerGetSyncers"></a>
# **iamApiControllerGetSyncers**
> kotlin.collections.List&lt;IamObjectSyncer&gt; iamApiControllerGetSyncers(owner)

Api Controller Get Syncers

get syncers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of syncers
try {
    val result : kotlin.collections.List<IamObjectSyncer> = apiInstance.iamApiControllerGetSyncers(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetSyncers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetSyncers")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of syncers | |

### Return type

[**kotlin.collections.List&lt;IamObjectSyncer&gt;**](IamObjectSyncer.md)

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

<a id="iamApiControllerGetSystemInfo"></a>
# **iamApiControllerGetSystemInfo**
> CloudUtilSystemInfo iamApiControllerGetSystemInfo()

Api Controller Get System Info

get system info like CPU and memory usage

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : CloudUtilSystemInfo = apiInstance.iamApiControllerGetSystemInfo()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetSystemInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetSystemInfo")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CloudUtilSystemInfo**](CloudUtilSystemInfo.md)

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

<a id="iamApiControllerGetTicket"></a>
# **iamApiControllerGetTicket**
> IamObjectTicket iamApiControllerGetTicket(id)

Api Controller Get Ticket

get ticket

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the ticket
try {
    val result : IamObjectTicket = apiInstance.iamApiControllerGetTicket(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetTicket")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetTicket")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the ticket | |

### Return type

[**IamObjectTicket**](IamObjectTicket.md)

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

<a id="iamApiControllerGetTickets"></a>
# **iamApiControllerGetTickets**
> kotlin.collections.List&lt;IamObjectTicket&gt; iamApiControllerGetTickets(owner)

Api Controller Get Tickets

get tickets

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of tickets
try {
    val result : kotlin.collections.List<IamObjectTicket> = apiInstance.iamApiControllerGetTickets(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetTickets")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetTickets")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of tickets | |

### Return type

[**kotlin.collections.List&lt;IamObjectTicket&gt;**](IamObjectTicket.md)

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

<a id="iamApiControllerGetVersionInfo"></a>
# **iamApiControllerGetVersionInfo**
> CloudUtilVersionInfo iamApiControllerGetVersionInfo(id)

Api Controller Get Version Info

get version info like Hanzo IAM release version and commit ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
try {
    val result : CloudUtilVersionInfo = apiInstance.iamApiControllerGetVersionInfo(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetVersionInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetVersionInfo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Resource identifier (owner/name) | |

### Return type

[**CloudUtilVersionInfo**](CloudUtilVersionInfo.md)

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

<a id="iamApiControllerGetWebhookEventType"></a>
# **iamApiControllerGetWebhookEventType**
> IamControllersResponse iamApiControllerGetWebhookEventType(id, ticket)

Api Controller Get Webhook Event Type

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val ticket : kotlin.String = ticket_example // kotlin.String | The eventId of QRCode
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerGetWebhookEventType(id, ticket)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetWebhookEventType")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetWebhookEventType")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **ticket** | **kotlin.String**| The eventId of QRCode | |

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="iamApiControllerGetWechatQRCode"></a>
# **iamApiControllerGetWechatQRCode**
> IamControllersResponse iamApiControllerGetWechatQRCode(id)

Api Controller Get Wechat QR Code

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of provider
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerGetWechatQRCode(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerGetWechatQRCode")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerGetWechatQRCode")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of provider | |

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="iamApiControllerHandleOfficialAccountEvent"></a>
# **iamApiControllerHandleOfficialAccountEvent**
> IamControllersResponse iamApiControllerHandleOfficialAccountEvent()

Api Controller Handle Official Account Event

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerHandleOfficialAccountEvent()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerHandleOfficialAccountEvent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerHandleOfficialAccountEvent")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="iamApiControllerHealth"></a>
# **iamApiControllerHealth**
> IamControllersResponse iamApiControllerHealth()

Api Controller Health

check if the system is live

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerHealth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="iamApiControllerRefreshEngines"></a>
# **iamApiControllerRefreshEngines**
> IamControllersResponse iamApiControllerRefreshEngines(m, t)

Api Controller Refresh Engines

Refresh all CLI engines

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val m : kotlin.String = m_example // kotlin.String | Hash for request validation
val t : kotlin.String = t_example // kotlin.String | Timestamp for request validation
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerRefreshEngines(m, t)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerRefreshEngines")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerRefreshEngines")
    e.printStackTrace()
}
```

### Parameters
| **m** | **kotlin.String**| Hash for request validation | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **t** | **kotlin.String**| Timestamp for request validation | |

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="iamApiControllerRunSyncer"></a>
# **iamApiControllerRunSyncer**
> IamControllersResponse iamApiControllerRunSyncer(iamObjectSyncer)

Api Controller Run Syncer

run syncer

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val iamObjectSyncer : IamObjectSyncer =  // IamObjectSyncer | The details of the syncer
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerRunSyncer(iamObjectSyncer)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerRunSyncer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerRunSyncer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectSyncer** | [**IamObjectSyncer**](IamObjectSyncer.md)| The details of the syncer | |

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

<a id="iamApiControllerSendEmail"></a>
# **iamApiControllerSendEmail**
> IamControllersResponse iamApiControllerSendEmail(clientId, clientSecret, iamControllersEmailForm)

Api Controller Send Email

This API is not for Hanzo IAM frontend to call, it is for Hanzo IAM SDKs.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val clientId : kotlin.String = clientId_example // kotlin.String | The clientId of the application
val clientSecret : kotlin.String = clientSecret_example // kotlin.String | The clientSecret of the application
val iamControllersEmailForm : IamControllersEmailForm =  // IamControllersEmailForm | Details of the email request
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerSendEmail(clientId, clientSecret, iamControllersEmailForm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerSendEmail")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerSendEmail")
    e.printStackTrace()
}
```

### Parameters
| **clientId** | **kotlin.String**| The clientId of the application | |
| **clientSecret** | **kotlin.String**| The clientSecret of the application | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamControllersEmailForm** | [**IamControllersEmailForm**](IamControllersEmailForm.md)| Details of the email request | |

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

<a id="iamApiControllerSendNotification"></a>
# **iamApiControllerSendNotification**
> IamControllersResponse iamApiControllerSendNotification(iamControllersNotificationForm)

Api Controller Send Notification

This API is not for Hanzo IAM frontend to call, it is for Hanzo IAM SDKs.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val iamControllersNotificationForm : IamControllersNotificationForm =  // IamControllersNotificationForm | Details of the notification request
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerSendNotification(iamControllersNotificationForm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerSendNotification")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerSendNotification")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamControllersNotificationForm** | [**IamControllersNotificationForm**](IamControllersNotificationForm.md)| Details of the notification request | |

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

<a id="iamApiControllerSendSms"></a>
# **iamApiControllerSendSms**
> IamControllersResponse iamApiControllerSendSms(clientId, clientSecret, iamControllersSmsForm)

Api Controller Send Sms

This API is not for Hanzo IAM frontend to call, it is for Hanzo IAM SDKs.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val clientId : kotlin.String = clientId_example // kotlin.String | The clientId of the application
val clientSecret : kotlin.String = clientSecret_example // kotlin.String | The clientSecret of the application
val iamControllersSmsForm : IamControllersSmsForm =  // IamControllersSmsForm | Details of the sms request
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerSendSms(clientId, clientSecret, iamControllersSmsForm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerSendSms")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerSendSms")
    e.printStackTrace()
}
```

### Parameters
| **clientId** | **kotlin.String**| The clientId of the application | |
| **clientSecret** | **kotlin.String**| The clientSecret of the application | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamControllersSmsForm** | [**IamControllersSmsForm**](IamControllersSmsForm.md)| Details of the sms request | |

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

<a id="iamApiControllerUpdateAdapter"></a>
# **iamApiControllerUpdateAdapter**
> IamControllersResponse iamApiControllerUpdateAdapter(id, iamObjectAdapter)

Api Controller Update Adapter

update adapter

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the adapter
val iamObjectAdapter : IamObjectAdapter =  // IamObjectAdapter | The details of the adapter
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateAdapter(id, iamObjectAdapter)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerUpdateAdapter")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerUpdateAdapter")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the adapter | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectAdapter** | [**IamObjectAdapter**](IamObjectAdapter.md)| The details of the adapter | |

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

<a id="iamApiControllerUpdateCert"></a>
# **iamApiControllerUpdateCert**
> IamControllersResponse iamApiControllerUpdateCert(id, iamObjectCert)

Api Controller Update Cert

update cert

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the cert
val iamObjectCert : IamObjectCert =  // IamObjectCert | The details of the cert
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateCert(id, iamObjectCert)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerUpdateCert")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerUpdateCert")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the cert | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectCert** | [**IamObjectCert**](IamObjectCert.md)| The details of the cert | |

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

<a id="iamApiControllerUpdateForm"></a>
# **iamApiControllerUpdateForm**
> IamControllersResponse iamApiControllerUpdateForm(id, iamObjectForm)

Api Controller Update Form

update form

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | The id (owner/name) of the form
val iamObjectForm : IamObjectForm =  // IamObjectForm | The details of the form
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateForm(id, iamObjectForm)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerUpdateForm")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerUpdateForm")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id (owner/name) of the form | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectForm** | [**IamObjectForm**](IamObjectForm.md)| The details of the form | |

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

<a id="iamApiControllerUpdateSyncer"></a>
# **iamApiControllerUpdateSyncer**
> IamControllersResponse iamApiControllerUpdateSyncer(id, iamObjectSyncer)

Api Controller Update Syncer

update syncer

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the syncer
val iamObjectSyncer : IamObjectSyncer =  // IamObjectSyncer | The details of the syncer
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateSyncer(id, iamObjectSyncer)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerUpdateSyncer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerUpdateSyncer")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the syncer | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectSyncer** | [**IamObjectSyncer**](IamObjectSyncer.md)| The details of the syncer | |

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

<a id="iamApiControllerUpdateTicket"></a>
# **iamApiControllerUpdateTicket**
> IamControllersResponse iamApiControllerUpdateTicket(id, iamObjectTicket)

Api Controller Update Ticket

update ticket

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the ticket
val iamObjectTicket : IamObjectTicket =  // IamObjectTicket | The details of the ticket
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateTicket(id, iamObjectTicket)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#iamApiControllerUpdateTicket")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#iamApiControllerUpdateTicket")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the ticket | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectTicket** | [**IamObjectTicket**](IamObjectTicket.md)| The details of the ticket | |

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

<a id="paasListTemplates"></a>
# **paasListTemplates**
> kotlin.collections.List&lt;PaasListTemplates200ResponseInner&gt; paasListTemplates()

List available templates

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : kotlin.collections.List<PaasListTemplates200ResponseInner> = apiInstance.paasListTemplates()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#paasListTemplates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#paasListTemplates")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;PaasListTemplates200ResponseInner&gt;**](PaasListTemplates200ResponseInner.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="tasksTasksCluster"></a>
# **tasksTasksCluster**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; tasksTasksCluster()

Cluster status (open probe)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.tasksTasksCluster()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#tasksTasksCluster")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#tasksTasksCluster")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="tasksTasksClusterHealth"></a>
# **tasksTasksClusterHealth**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; tasksTasksClusterHealth()

Cluster health (open probe)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.tasksTasksClusterHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#tasksTasksClusterHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#tasksTasksClusterHealth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="tasksTasksHealth"></a>
# **tasksTasksHealth**
> EvalsGetV1EvalsHealth200Response tasksTasksHealth()

Liveness probe

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : EvalsGetV1EvalsHealth200Response = apiInstance.tasksTasksHealth()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#tasksTasksHealth")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#tasksTasksHealth")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**EvalsGetV1EvalsHealth200Response**](EvalsGetV1EvalsHealth200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="tasksTasksSettings"></a>
# **tasksTasksSettings**
> kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt; tasksTasksSettings()

Capability flags (open bootstrap)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = SystemApi()
try {
    val result : kotlin.collections.Map<kotlin.String, kotlin.Any> = apiInstance.tasksTasksSettings()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SystemApi#tasksTasksSettings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SystemApi#tasksTasksSettings")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.Map&lt;kotlin.String, kotlin.Any&gt;**](kotlin.Any.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

