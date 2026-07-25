# ProjectsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**autoGetProject**](ProjectsApi.md#autoGetProject) | **GET** /v1/auto/projects/{id} | Get a project by id |
| [**autoListProjects**](ProjectsApi.md#autoListProjects) | **GET** /v1/auto/projects | List projects |
| [**autoUpdateProject**](ProjectsApi.md#autoUpdateProject) | **POST** /v1/auto/projects/{id} | Update project settings |
| [**consoleCreateProject**](ProjectsApi.md#consoleCreateProject) | **POST** /v1/console/projects | Create a new project (requires organization-scoped API key) |
| [**consoleCreateProjectApiKey**](ProjectsApi.md#consoleCreateProjectApiKey) | **POST** /v1/console/projects/{projectId}/apiKeys | Create an API key for a project |
| [**consoleDeleteProject**](ProjectsApi.md#consoleDeleteProject) | **DELETE** /v1/console/projects/{projectId} | Delete a project (async) |
| [**consoleDeleteProjectApiKey**](ProjectsApi.md#consoleDeleteProjectApiKey) | **DELETE** /v1/console/projects/{projectId}/apiKeys/{apiKeyId} | Delete a project API key |
| [**consoleGetProject**](ProjectsApi.md#consoleGetProject) | **GET** /v1/console/projects | Get project associated with API key |
| [**consoleGetProjectById**](ProjectsApi.md#consoleGetProjectById) | **GET** /v1/console/projects/{projectId} | Get a project by ID |
| [**consoleListProjectApiKeys**](ProjectsApi.md#consoleListProjectApiKeys) | **GET** /v1/console/projects/{projectId}/apiKeys | Get all API keys for a project |
| [**consoleUpdateProject**](ProjectsApi.md#consoleUpdateProject) | **PUT** /v1/console/projects/{projectId} | Update a project |
| [**dbCreateProject**](ProjectsApi.md#dbCreateProject) | **POST** /v1/db/projects | Create project |
| [**dbDeleteProject**](ProjectsApi.md#dbDeleteProject) | **DELETE** /v1/db/projects/{id} | Delete project |
| [**dbGetConnectionUri**](ProjectsApi.md#dbGetConnectionUri) | **GET** /v1/db/projects/{id}/connection_uri | Get connection URI |
| [**dbGetProject**](ProjectsApi.md#dbGetProject) | **GET** /v1/db/projects/{id} | Get project |
| [**dbListProjects**](ProjectsApi.md#dbListProjects) | **GET** /v1/db/projects | List projects |
| [**dbUpdateProject**](ProjectsApi.md#dbUpdateProject) | **PUT** /v1/db/projects/{id} | Update project |
| [**flowGetProject**](ProjectsApi.md#flowGetProject) | **GET** /v1/flow/projects/{id} | Get a project by id |
| [**flowListProjects**](ProjectsApi.md#flowListProjects) | **GET** /v1/flow/projects | List projects |
| [**flowUpdateProject**](ProjectsApi.md#flowUpdateProject) | **POST** /v1/flow/projects/{id} | Update project settings |
| [**kmsCreateProject**](ProjectsApi.md#kmsCreateProject) | **POST** /v1/kms/projects | Create a project |
| [**kmsDeleteProject**](ProjectsApi.md#kmsDeleteProject) | **DELETE** /v1/kms/projects/{projectId} | Delete a project |
| [**kmsGetProject**](ProjectsApi.md#kmsGetProject) | **GET** /v1/kms/projects/{projectId} | Get a project by ID |
| [**kmsListProjectUsers**](ProjectsApi.md#kmsListProjectUsers) | **GET** /v1/kms/projects/{projectId}/users | List project members |
| [**kmsUpdateProject**](ProjectsApi.md#kmsUpdateProject) | **PATCH** /v1/kms/projects/{projectId} | Update a project |
| [**paasCreateProject**](ProjectsApi.md#paasCreateProject) | **POST** /v1/paas/org/{orgId}/project | Create project |
| [**paasDeleteProject**](ProjectsApi.md#paasDeleteProject) | **DELETE** /v1/paas/org/{orgId}/project/{projectId} | Delete project |
| [**paasGetProject**](ProjectsApi.md#paasGetProject) | **GET** /v1/paas/org/{orgId}/project/{projectId} | Get project |
| [**paasListProjects**](ProjectsApi.md#paasListProjects) | **GET** /v1/paas/org/{orgId}/project | List projects |
| [**paasUpdateProject**](ProjectsApi.md#paasUpdateProject) | **PUT** /v1/paas/org/{orgId}/project/{projectId} | Update project |
| [**projectsCreateProject**](ProjectsApi.md#projectsCreateProject) | **POST** /v1/projects | Create a project |
| [**projectsDeleteProject**](ProjectsApi.md#projectsDeleteProject) | **DELETE** /v1/projects/{slug} | Delete a project |
| [**projectsForkProject**](ProjectsApi.md#projectsForkProject) | **POST** /v1/projects/fork | Fork a starter template into a new project |
| [**projectsGetProject**](ProjectsApi.md#projectsGetProject) | **GET** /v1/projects/{slug} | Get a project |
| [**projectsListProjects**](ProjectsApi.md#projectsListProjects) | **GET** /v1/projects | List projects |
| [**projectsUpdateProject**](ProjectsApi.md#projectsUpdateProject) | **PATCH** /v1/projects/{slug} | Update a project |
| [**registryCreateProject**](ProjectsApi.md#registryCreateProject) | **POST** /v1/registry/projects | Create project |
| [**registryDeleteProject**](ProjectsApi.md#registryDeleteProject) | **DELETE** /v1/registry/projects/{name} | Delete project |
| [**registryGetProject**](ProjectsApi.md#registryGetProject) | **GET** /v1/registry/projects/{name} | Get project |
| [**registryListProjects**](ProjectsApi.md#registryListProjects) | **GET** /v1/registry/projects | List projects |
| [**registryUpdateProject**](ProjectsApi.md#registryUpdateProject) | **PUT** /v1/registry/projects/{name} | Update project |
| [**trackerCreateProject**](ProjectsApi.md#trackerCreateProject) | **POST** /v1/tracker/projects | Create a project |
| [**trackerDeleteProject**](ProjectsApi.md#trackerDeleteProject) | **DELETE** /v1/tracker/projects/{key} | Delete a project and all its issues |
| [**trackerGetProject**](ProjectsApi.md#trackerGetProject) | **GET** /v1/tracker/projects/{key} | Get a project |
| [**trackerListProjects**](ProjectsApi.md#trackerListProjects) | **GET** /v1/tracker/projects | List projects |
| [**trackerUpdateProject**](ProjectsApi.md#trackerUpdateProject) | **PATCH** /v1/tracker/projects/{key} | Update a project |


<a id="autoGetProject"></a>
# **autoGetProject**
> kotlin.Any autoGetProject(id)

Get a project by id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.autoGetProject(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#autoGetProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#autoGetProject")
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

<a id="autoListProjects"></a>
# **autoListProjects**
> kotlin.collections.List&lt;AutoProject&gt; autoListProjects()

List projects

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
try {
    val result : kotlin.collections.List<AutoProject> = apiInstance.autoListProjects()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#autoListProjects")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#autoListProjects")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;AutoProject&gt;**](AutoProject.md)

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

<a id="autoUpdateProject"></a>
# **autoUpdateProject**
> kotlin.Any autoUpdateProject(id, autoUpdateAppConnectionRequest)

Update project settings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val id : kotlin.String = id_example // kotlin.String | 
val autoUpdateAppConnectionRequest : AutoUpdateAppConnectionRequest =  // AutoUpdateAppConnectionRequest | 
try {
    val result : kotlin.Any = apiInstance.autoUpdateProject(id, autoUpdateAppConnectionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#autoUpdateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#autoUpdateProject")
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

<a id="consoleCreateProject"></a>
# **consoleCreateProject**
> ConsoleProject consoleCreateProject(consoleCreateProjectRequest)

Create a new project (requires organization-scoped API key)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val consoleCreateProjectRequest : ConsoleCreateProjectRequest =  // ConsoleCreateProjectRequest | 
try {
    val result : ConsoleProject = apiInstance.consoleCreateProject(consoleCreateProjectRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#consoleCreateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#consoleCreateProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleCreateProjectRequest** | [**ConsoleCreateProjectRequest**](ConsoleCreateProjectRequest.md)|  | |

### Return type

[**ConsoleProject**](ConsoleProject.md)

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

<a id="consoleCreateProjectApiKey"></a>
# **consoleCreateProjectApiKey**
> ConsoleCreateProjectApiKey200Response consoleCreateProjectApiKey(projectId, consoleCreateProjectApiKeyRequest)

Create an API key for a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val projectId : kotlin.String = projectId_example // kotlin.String | 
val consoleCreateProjectApiKeyRequest : ConsoleCreateProjectApiKeyRequest =  // ConsoleCreateProjectApiKeyRequest | 
try {
    val result : ConsoleCreateProjectApiKey200Response = apiInstance.consoleCreateProjectApiKey(projectId, consoleCreateProjectApiKeyRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#consoleCreateProjectApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#consoleCreateProjectApiKey")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleCreateProjectApiKeyRequest** | [**ConsoleCreateProjectApiKeyRequest**](ConsoleCreateProjectApiKeyRequest.md)|  | |

### Return type

[**ConsoleCreateProjectApiKey200Response**](ConsoleCreateProjectApiKey200Response.md)

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

<a id="consoleDeleteProject"></a>
# **consoleDeleteProject**
> ConsoleDeleteProject202Response consoleDeleteProject(projectId)

Delete a project (async)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val projectId : kotlin.String = projectId_example // kotlin.String | 
try {
    val result : ConsoleDeleteProject202Response = apiInstance.consoleDeleteProject(projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#consoleDeleteProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#consoleDeleteProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **kotlin.String**|  | |

### Return type

[**ConsoleDeleteProject202Response**](ConsoleDeleteProject202Response.md)

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

<a id="consoleDeleteProjectApiKey"></a>
# **consoleDeleteProjectApiKey**
> ConsoleDeleteProjectApiKey200Response consoleDeleteProjectApiKey(projectId, apiKeyId)

Delete a project API key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val projectId : kotlin.String = projectId_example // kotlin.String | 
val apiKeyId : kotlin.String = apiKeyId_example // kotlin.String | 
try {
    val result : ConsoleDeleteProjectApiKey200Response = apiInstance.consoleDeleteProjectApiKey(projectId, apiKeyId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#consoleDeleteProjectApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#consoleDeleteProjectApiKey")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **apiKeyId** | **kotlin.String**|  | |

### Return type

[**ConsoleDeleteProjectApiKey200Response**](ConsoleDeleteProjectApiKey200Response.md)

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

<a id="consoleGetProject"></a>
# **consoleGetProject**
> ConsoleGetProject200Response consoleGetProject()

Get project associated with API key

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
try {
    val result : ConsoleGetProject200Response = apiInstance.consoleGetProject()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#consoleGetProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#consoleGetProject")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ConsoleGetProject200Response**](ConsoleGetProject200Response.md)

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

<a id="consoleGetProjectById"></a>
# **consoleGetProjectById**
> ConsoleProject consoleGetProjectById(projectId)

Get a project by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val projectId : kotlin.String = projectId_example // kotlin.String | 
try {
    val result : ConsoleProject = apiInstance.consoleGetProjectById(projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#consoleGetProjectById")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#consoleGetProjectById")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **kotlin.String**|  | |

### Return type

[**ConsoleProject**](ConsoleProject.md)

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

<a id="consoleListProjectApiKeys"></a>
# **consoleListProjectApiKeys**
> ConsoleListOrganizationApiKeys200Response consoleListProjectApiKeys(projectId)

Get all API keys for a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val projectId : kotlin.String = projectId_example // kotlin.String | 
try {
    val result : ConsoleListOrganizationApiKeys200Response = apiInstance.consoleListProjectApiKeys(projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#consoleListProjectApiKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#consoleListProjectApiKeys")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **kotlin.String**|  | |

### Return type

[**ConsoleListOrganizationApiKeys200Response**](ConsoleListOrganizationApiKeys200Response.md)

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

<a id="consoleUpdateProject"></a>
# **consoleUpdateProject**
> ConsoleProject consoleUpdateProject(projectId, consoleUpdateProjectRequest)

Update a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val projectId : kotlin.String = projectId_example // kotlin.String | 
val consoleUpdateProjectRequest : ConsoleUpdateProjectRequest =  // ConsoleUpdateProjectRequest | 
try {
    val result : ConsoleProject = apiInstance.consoleUpdateProject(projectId, consoleUpdateProjectRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#consoleUpdateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#consoleUpdateProject")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleUpdateProjectRequest** | [**ConsoleUpdateProjectRequest**](ConsoleUpdateProjectRequest.md)|  | |

### Return type

[**ConsoleProject**](ConsoleProject.md)

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

<a id="dbCreateProject"></a>
# **dbCreateProject**
> DbCreateProject201Response dbCreateProject(dbCreateProjectRequest)

Create project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val dbCreateProjectRequest : DbCreateProjectRequest =  // DbCreateProjectRequest | 
try {
    val result : DbCreateProject201Response = apiInstance.dbCreateProject(dbCreateProjectRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#dbCreateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#dbCreateProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dbCreateProjectRequest** | [**DbCreateProjectRequest**](DbCreateProjectRequest.md)|  | |

### Return type

[**DbCreateProject201Response**](DbCreateProject201Response.md)

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

<a id="dbDeleteProject"></a>
# **dbDeleteProject**
> DbGetProject200Response dbDeleteProject(id)

Delete project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : DbGetProject200Response = apiInstance.dbDeleteProject(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#dbDeleteProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#dbDeleteProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**DbGetProject200Response**](DbGetProject200Response.md)

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

<a id="dbGetConnectionUri"></a>
# **dbGetConnectionUri**
> DbConnectionUri dbGetConnectionUri(id, roleName, branchId, endpointId, databaseName, pooled)

Get connection URI

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val id : kotlin.String = id_example // kotlin.String | 
val roleName : kotlin.String = roleName_example // kotlin.String | 
val branchId : kotlin.String = branchId_example // kotlin.String | 
val endpointId : kotlin.String = endpointId_example // kotlin.String | 
val databaseName : kotlin.String = databaseName_example // kotlin.String | 
val pooled : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : DbConnectionUri = apiInstance.dbGetConnectionUri(id, roleName, branchId, endpointId, databaseName, pooled)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#dbGetConnectionUri")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#dbGetConnectionUri")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| **roleName** | **kotlin.String**|  | |
| **branchId** | **kotlin.String**|  | [optional] |
| **endpointId** | **kotlin.String**|  | [optional] |
| **databaseName** | **kotlin.String**|  | [optional] [default to &quot;neondb&quot;] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **pooled** | **kotlin.Boolean**|  | [optional] [default to true] |

### Return type

[**DbConnectionUri**](DbConnectionUri.md)

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

<a id="dbGetProject"></a>
# **dbGetProject**
> DbGetProject200Response dbGetProject(id)

Get project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : DbGetProject200Response = apiInstance.dbGetProject(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#dbGetProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#dbGetProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**DbGetProject200Response**](DbGetProject200Response.md)

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

<a id="dbListProjects"></a>
# **dbListProjects**
> DbListProjects200Response dbListProjects(cursor, limit)

List projects

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val cursor : kotlin.String = cursor_example // kotlin.String | 
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : DbListProjects200Response = apiInstance.dbListProjects(cursor, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#dbListProjects")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#dbListProjects")
    e.printStackTrace()
}
```

### Parameters
| **cursor** | **kotlin.String**|  | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 10] |

### Return type

[**DbListProjects200Response**](DbListProjects200Response.md)

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

<a id="dbUpdateProject"></a>
# **dbUpdateProject**
> DbGetProject200Response dbUpdateProject(id, dbUpdateProjectRequest)

Update project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val id : kotlin.String = id_example // kotlin.String | 
val dbUpdateProjectRequest : DbUpdateProjectRequest =  // DbUpdateProjectRequest | 
try {
    val result : DbGetProject200Response = apiInstance.dbUpdateProject(id, dbUpdateProjectRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#dbUpdateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#dbUpdateProject")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dbUpdateProjectRequest** | [**DbUpdateProjectRequest**](DbUpdateProjectRequest.md)|  | |

### Return type

[**DbGetProject200Response**](DbGetProject200Response.md)

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

<a id="flowGetProject"></a>
# **flowGetProject**
> FlowProject flowGetProject(id)

Get a project by id

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : FlowProject = apiInstance.flowGetProject(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#flowGetProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#flowGetProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**FlowProject**](FlowProject.md)

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

<a id="flowListProjects"></a>
# **flowListProjects**
> kotlin.collections.List&lt;FlowProject&gt; flowListProjects()

List projects

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
try {
    val result : kotlin.collections.List<FlowProject> = apiInstance.flowListProjects()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#flowListProjects")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#flowListProjects")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;FlowProject&gt;**](FlowProject.md)

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

<a id="flowUpdateProject"></a>
# **flowUpdateProject**
> FlowProject flowUpdateProject(id, autoUpdateAppConnectionRequest)

Update project settings

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val id : kotlin.String = id_example // kotlin.String | 
val autoUpdateAppConnectionRequest : AutoUpdateAppConnectionRequest =  // AutoUpdateAppConnectionRequest | 
try {
    val result : FlowProject = apiInstance.flowUpdateProject(id, autoUpdateAppConnectionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#flowUpdateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#flowUpdateProject")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **autoUpdateAppConnectionRequest** | [**AutoUpdateAppConnectionRequest**](AutoUpdateAppConnectionRequest.md)|  | |

### Return type

[**FlowProject**](FlowProject.md)

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

<a id="kmsCreateProject"></a>
# **kmsCreateProject**
> KmsCreateProject200Response kmsCreateProject(kmsCreateProjectRequest)

Create a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val kmsCreateProjectRequest : KmsCreateProjectRequest =  // KmsCreateProjectRequest | 
try {
    val result : KmsCreateProject200Response = apiInstance.kmsCreateProject(kmsCreateProjectRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#kmsCreateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#kmsCreateProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsCreateProjectRequest** | [**KmsCreateProjectRequest**](KmsCreateProjectRequest.md)|  | |

### Return type

[**KmsCreateProject200Response**](KmsCreateProject200Response.md)

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

<a id="kmsDeleteProject"></a>
# **kmsDeleteProject**
> kotlin.Any kmsDeleteProject(projectId)

Delete a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.kmsDeleteProject(projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#kmsDeleteProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#kmsDeleteProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **java.util.UUID**|  | |

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

<a id="kmsGetProject"></a>
# **kmsGetProject**
> KmsCreateProject200Response kmsGetProject(projectId)

Get a project by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsCreateProject200Response = apiInstance.kmsGetProject(projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#kmsGetProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#kmsGetProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **java.util.UUID**|  | |

### Return type

[**KmsCreateProject200Response**](KmsCreateProject200Response.md)

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

<a id="kmsListProjectUsers"></a>
# **kmsListProjectUsers**
> KmsListProjectUsers200Response kmsListProjectUsers(projectId, includeGroupMembers)

List project members

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val includeGroupMembers : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : KmsListProjectUsers200Response = apiInstance.kmsListProjectUsers(projectId, includeGroupMembers)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#kmsListProjectUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#kmsListProjectUsers")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **includeGroupMembers** | **kotlin.Boolean**|  | [optional] [default to false] |

### Return type

[**KmsListProjectUsers200Response**](KmsListProjectUsers200Response.md)

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

<a id="kmsUpdateProject"></a>
# **kmsUpdateProject**
> KmsCreateProject200Response kmsUpdateProject(projectId, kmsUpdateProjectRequest)

Update a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val projectId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsUpdateProjectRequest : KmsUpdateProjectRequest =  // KmsUpdateProjectRequest | 
try {
    val result : KmsCreateProject200Response = apiInstance.kmsUpdateProject(projectId, kmsUpdateProjectRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#kmsUpdateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#kmsUpdateProject")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUpdateProjectRequest** | [**KmsUpdateProjectRequest**](KmsUpdateProjectRequest.md)|  | |

### Return type

[**KmsCreateProject200Response**](KmsCreateProject200Response.md)

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

<a id="paasCreateProject"></a>
# **paasCreateProject**
> PaasProject paasCreateProject(orgId, paasCreateOrganizationRequest)

Create project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val paasCreateOrganizationRequest : PaasCreateOrganizationRequest =  // PaasCreateOrganizationRequest | 
try {
    val result : PaasProject = apiInstance.paasCreateProject(orgId, paasCreateOrganizationRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#paasCreateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#paasCreateProject")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **paasCreateOrganizationRequest** | [**PaasCreateOrganizationRequest**](PaasCreateOrganizationRequest.md)|  | |

### Return type

[**PaasProject**](PaasProject.md)

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

<a id="paasDeleteProject"></a>
# **paasDeleteProject**
> kotlin.Any paasDeleteProject(orgId, projectId)

Delete project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.paasDeleteProject(orgId, projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#paasDeleteProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#paasDeleteProject")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **kotlin.String**|  | |

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

<a id="paasGetProject"></a>
# **paasGetProject**
> PaasProject paasGetProject(orgId, projectId)

Get project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
try {
    val result : PaasProject = apiInstance.paasGetProject(orgId, projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#paasGetProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#paasGetProject")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **kotlin.String**|  | |

### Return type

[**PaasProject**](PaasProject.md)

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

<a id="paasListProjects"></a>
# **paasListProjects**
> kotlin.collections.List&lt;PaasProject&gt; paasListProjects(orgId)

List projects

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<PaasProject> = apiInstance.paasListProjects(orgId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#paasListProjects")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#paasListProjects")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orgId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;PaasProject&gt;**](PaasProject.md)

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

<a id="paasUpdateProject"></a>
# **paasUpdateProject**
> kotlin.Any paasUpdateProject(orgId, projectId, paasUpdateOrganizationRequest)

Update project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val projectId : kotlin.String = projectId_example // kotlin.String | 
val paasUpdateOrganizationRequest : PaasUpdateOrganizationRequest =  // PaasUpdateOrganizationRequest | 
try {
    val result : kotlin.Any = apiInstance.paasUpdateProject(orgId, projectId, paasUpdateOrganizationRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#paasUpdateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#paasUpdateProject")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
| **projectId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **paasUpdateOrganizationRequest** | [**PaasUpdateOrganizationRequest**](PaasUpdateOrganizationRequest.md)|  | |

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

<a id="projectsCreateProject"></a>
# **projectsCreateProject**
> ProjectsProject projectsCreateProject(projectsCreateProjectRequest)

Create a project

Create an org-scoped project. When &#x60;slug&#x60; is omitted it is derived from &#x60;name&#x60; (slugified). The slug must match &#x60;^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$&#x60;, must not be a reserved subdomain, and must be unique within the org. &#x60;framework&#x60; defaults to &#x60;static&#x60; and must be one of the known build hints. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val projectsCreateProjectRequest : ProjectsCreateProjectRequest =  // ProjectsCreateProjectRequest | 
try {
    val result : ProjectsProject = apiInstance.projectsCreateProject(projectsCreateProjectRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#projectsCreateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#projectsCreateProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectsCreateProjectRequest** | [**ProjectsCreateProjectRequest**](ProjectsCreateProjectRequest.md)|  | |

### Return type

[**ProjectsProject**](ProjectsProject.md)

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

<a id="projectsDeleteProject"></a>
# **projectsDeleteProject**
> projectsDeleteProject(slug)

Delete a project

Delete the project and its deployment history, purge the S3 origin under &#x60;&lt;org&gt;/&lt;slug&gt;/&#x60;, release the subdomain binding, and flush the edge cache-tag &#x60;site-&lt;org&gt;-&lt;slug&gt;&#x60;. The metadata delete is authoritative; the S3-origin purge, host unbind, and edge flush are best-effort. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val slug : kotlin.String = slug_example // kotlin.String | Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label.
try {
    apiInstance.projectsDeleteProject(slug)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#projectsDeleteProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#projectsDeleteProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**| Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label. | |

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

<a id="projectsForkProject"></a>
# **projectsForkProject**
> ProjectsProject projectsForkProject(projectsForkProjectRequest)

Fork a starter template into a new project

Create a project seeded from a starter-kit gallery template. &#x60;slug&#x60; is the template slug to fork (required); &#x60;name&#x60; defaults to the template title; &#x60;target&#x60; overrides the derived project slug. Funnels through the same create path, so slug/framework validation and conflict handling apply identically. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val projectsForkProjectRequest : ProjectsForkProjectRequest =  // ProjectsForkProjectRequest | 
try {
    val result : ProjectsProject = apiInstance.projectsForkProject(projectsForkProjectRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#projectsForkProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#projectsForkProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectsForkProjectRequest** | [**ProjectsForkProjectRequest**](ProjectsForkProjectRequest.md)|  | |

### Return type

[**ProjectsProject**](ProjectsProject.md)

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

<a id="projectsGetProject"></a>
# **projectsGetProject**
> ProjectsProject projectsGetProject(slug)

Get a project

Read one org-scoped project by slug.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val slug : kotlin.String = slug_example // kotlin.String | Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label.
try {
    val result : ProjectsProject = apiInstance.projectsGetProject(slug)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#projectsGetProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#projectsGetProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **slug** | **kotlin.String**| Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label. | |

### Return type

[**ProjectsProject**](ProjectsProject.md)

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

<a id="projectsListProjects"></a>
# **projectsListProjects**
> kotlin.collections.List&lt;ProjectsProject&gt; projectsListProjects()

List projects

List every project for the caller&#39;s org, most-recently-updated first.

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
try {
    val result : kotlin.collections.List<ProjectsProject> = apiInstance.projectsListProjects()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#projectsListProjects")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#projectsListProjects")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ProjectsProject&gt;**](ProjectsProject.md)

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

<a id="projectsUpdateProject"></a>
# **projectsUpdateProject**
> ProjectsProject projectsUpdateProject(slug, projectsUpdateProjectRequest)

Update a project

Partial update; only supplied fields change. &#x60;name&#x60; may not be blanked. &#x60;framework&#x60; must remain a known build hint. &#x60;cacheControl&#x60; is capped at 256 chars and must not contain newlines. 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val slug : kotlin.String = slug_example // kotlin.String | Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label.
val projectsUpdateProjectRequest : ProjectsUpdateProjectRequest =  // ProjectsUpdateProjectRequest | 
try {
    val result : ProjectsProject = apiInstance.projectsUpdateProject(slug, projectsUpdateProjectRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#projectsUpdateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#projectsUpdateProject")
    e.printStackTrace()
}
```

### Parameters
| **slug** | **kotlin.String**| Org-unique project handle (lowercased); also the S3-origin key segment and the subdomain label. | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectsUpdateProjectRequest** | [**ProjectsUpdateProjectRequest**](ProjectsUpdateProjectRequest.md)|  | |

### Return type

[**ProjectsProject**](ProjectsProject.md)

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

<a id="registryCreateProject"></a>
# **registryCreateProject**
> kotlin.Any registryCreateProject(registryProjectCreate)

Create project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val registryProjectCreate : RegistryProjectCreate =  // RegistryProjectCreate | 
try {
    val result : kotlin.Any = apiInstance.registryCreateProject(registryProjectCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#registryCreateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#registryCreateProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **registryProjectCreate** | [**RegistryProjectCreate**](RegistryProjectCreate.md)|  | |

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

<a id="registryDeleteProject"></a>
# **registryDeleteProject**
> kotlin.Any registryDeleteProject(name)

Delete project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.registryDeleteProject(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#registryDeleteProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#registryDeleteProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

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

<a id="registryGetProject"></a>
# **registryGetProject**
> RegistryProject registryGetProject(name)

Get project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val name : kotlin.String = name_example // kotlin.String | 
try {
    val result : RegistryProject = apiInstance.registryGetProject(name)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#registryGetProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#registryGetProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **name** | **kotlin.String**|  | |

### Return type

[**RegistryProject**](RegistryProject.md)

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

<a id="registryListProjects"></a>
# **registryListProjects**
> kotlin.collections.List&lt;RegistryProject&gt; registryListProjects(name, `public`, page, pageSize, sort)

List projects

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val name : kotlin.String = name_example // kotlin.String | Filter by project name (fuzzy match)
val `public` : kotlin.Boolean = true // kotlin.Boolean | Filter by public/private
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val sort : kotlin.String = sort_example // kotlin.String | 
try {
    val result : kotlin.collections.List<RegistryProject> = apiInstance.registryListProjects(name, `public`, page, pageSize, sort)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#registryListProjects")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#registryListProjects")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**| Filter by project name (fuzzy match) | [optional] |
| **&#x60;public&#x60;** | **kotlin.Boolean**| Filter by public/private | [optional] |
| **page** | **kotlin.Int**|  | [optional] [default to 1] |
| **pageSize** | **kotlin.Int**|  | [optional] [default to 10] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **sort** | **kotlin.String**|  | [optional] [default to &quot;creation_time&quot;] |

### Return type

[**kotlin.collections.List&lt;RegistryProject&gt;**](RegistryProject.md)

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

<a id="registryUpdateProject"></a>
# **registryUpdateProject**
> kotlin.Any registryUpdateProject(name, registryUpdateProjectRequest)

Update project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val name : kotlin.String = name_example // kotlin.String | 
val registryUpdateProjectRequest : RegistryUpdateProjectRequest =  // RegistryUpdateProjectRequest | 
try {
    val result : kotlin.Any = apiInstance.registryUpdateProject(name, registryUpdateProjectRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#registryUpdateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#registryUpdateProject")
    e.printStackTrace()
}
```

### Parameters
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **registryUpdateProjectRequest** | [**RegistryUpdateProjectRequest**](RegistryUpdateProjectRequest.md)|  | |

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

<a id="trackerCreateProject"></a>
# **trackerCreateProject**
> TrackerProject trackerCreateProject(trackerCreateProjectRequest)

Create a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val trackerCreateProjectRequest : TrackerCreateProjectRequest =  // TrackerCreateProjectRequest | 
try {
    val result : TrackerProject = apiInstance.trackerCreateProject(trackerCreateProjectRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#trackerCreateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#trackerCreateProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **trackerCreateProjectRequest** | [**TrackerCreateProjectRequest**](TrackerCreateProjectRequest.md)|  | |

### Return type

[**TrackerProject**](TrackerProject.md)

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

<a id="trackerDeleteProject"></a>
# **trackerDeleteProject**
> trackerDeleteProject(key)

Delete a project and all its issues

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val key : kotlin.String = key_example // kotlin.String | Project key (uppercase, ^[A-Z][A-Z0-9]{1,7}$)
try {
    apiInstance.trackerDeleteProject(key)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#trackerDeleteProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#trackerDeleteProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**| Project key (uppercase, ^[A-Z][A-Z0-9]{1,7}$) | |

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

<a id="trackerGetProject"></a>
# **trackerGetProject**
> TrackerProject trackerGetProject(key)

Get a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val key : kotlin.String = key_example // kotlin.String | Project key (uppercase, ^[A-Z][A-Z0-9]{1,7}$)
try {
    val result : TrackerProject = apiInstance.trackerGetProject(key)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#trackerGetProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#trackerGetProject")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**| Project key (uppercase, ^[A-Z][A-Z0-9]{1,7}$) | |

### Return type

[**TrackerProject**](TrackerProject.md)

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

<a id="trackerListProjects"></a>
# **trackerListProjects**
> kotlin.collections.List&lt;TrackerProject&gt; trackerListProjects()

List projects

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
try {
    val result : kotlin.collections.List<TrackerProject> = apiInstance.trackerListProjects()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#trackerListProjects")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#trackerListProjects")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;TrackerProject&gt;**](TrackerProject.md)

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

<a id="trackerUpdateProject"></a>
# **trackerUpdateProject**
> TrackerProject trackerUpdateProject(key, trackerUpdateProjectRequest)

Update a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ProjectsApi()
val key : kotlin.String = key_example // kotlin.String | Project key (uppercase, ^[A-Z][A-Z0-9]{1,7}$)
val trackerUpdateProjectRequest : TrackerUpdateProjectRequest =  // TrackerUpdateProjectRequest | 
try {
    val result : TrackerProject = apiInstance.trackerUpdateProject(key, trackerUpdateProjectRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProjectsApi#trackerUpdateProject")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProjectsApi#trackerUpdateProject")
    e.printStackTrace()
}
```

### Parameters
| **key** | **kotlin.String**| Project key (uppercase, ^[A-Z][A-Z0-9]{1,7}$) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **trackerUpdateProjectRequest** | [**TrackerUpdateProjectRequest**](TrackerUpdateProjectRequest.md)|  | |

### Return type

[**TrackerProject**](TrackerProject.md)

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

