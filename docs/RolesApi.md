# RolesApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**chatGetRolesByrolename**](RolesApi.md#chatGetRolesByrolename) | **GET** /v1/chat/roles/{roleName} | Get a role by name |
| [**chatPutRolesByrolenameAgents**](RolesApi.md#chatPutRolesByrolenameAgents) | **PUT** /v1/chat/roles/{roleName}/agents | Update agent permissions for a role |
| [**chatPutRolesByrolenameMarketplace**](RolesApi.md#chatPutRolesByrolenameMarketplace) | **PUT** /v1/chat/roles/{roleName}/marketplace | Update marketplace permissions for a role |
| [**chatPutRolesByrolenameMcpServers**](RolesApi.md#chatPutRolesByrolenameMcpServers) | **PUT** /v1/chat/roles/{roleName}/mcp-servers | Update MCP servers permissions for a role |
| [**chatPutRolesByrolenameMemories**](RolesApi.md#chatPutRolesByrolenameMemories) | **PUT** /v1/chat/roles/{roleName}/memories | Update memory permissions for a role |
| [**chatPutRolesByrolenamePeoplePicker**](RolesApi.md#chatPutRolesByrolenamePeoplePicker) | **PUT** /v1/chat/roles/{roleName}/people-picker | Update people picker permissions for a role |
| [**chatPutRolesByrolenamePrompts**](RolesApi.md#chatPutRolesByrolenamePrompts) | **PUT** /v1/chat/roles/{roleName}/prompts | Update prompt permissions for a role |
| [**chatPutRolesByrolenameRemoteAgents**](RolesApi.md#chatPutRolesByrolenameRemoteAgents) | **PUT** /v1/chat/roles/{roleName}/remote-agents | Update remote agents permissions for a role |
| [**dbCreateRole**](RolesApi.md#dbCreateRole) | **POST** /v1/db/projects/{id}/roles | Create role |
| [**dbDeleteRole**](RolesApi.md#dbDeleteRole) | **DELETE** /v1/db/projects/{id}/roles/{name} | Delete role |
| [**dbGetRole**](RolesApi.md#dbGetRole) | **GET** /v1/db/projects/{id}/roles/{name} | Get role |
| [**dbListRoles**](RolesApi.md#dbListRoles) | **GET** /v1/db/projects/{id}/roles | List roles |
| [**dbResetRolePassword**](RolesApi.md#dbResetRolePassword) | **POST** /v1/db/projects/{id}/roles/{name}/reset_password | Reset role password |
| [**frameworkAssignRole**](RolesApi.md#frameworkAssignRole) | **POST** /v1/framework/roles | Assign a role to a user |
| [**frameworkListRoles**](RolesApi.md#frameworkListRoles) | **GET** /v1/framework/roles | List per-org role assignments |
| [**frameworkRevokeRole**](RolesApi.md#frameworkRevokeRole) | **DELETE** /v1/framework/roles/{user}/{role} | Revoke a role from a user |


<a id="chatGetRolesByrolename"></a>
# **chatGetRolesByrolename**
> kotlin.Any chatGetRolesByrolename(roleName)

Get a role by name

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val roleName : kotlin.String = roleName_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.chatGetRolesByrolename(roleName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#chatGetRolesByrolename")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#chatGetRolesByrolename")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **roleName** | **kotlin.String**|  | |

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

<a id="chatPutRolesByrolenameAgents"></a>
# **chatPutRolesByrolenameAgents**
> kotlin.Any chatPutRolesByrolenameAgents(roleName, body)

Update agent permissions for a role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val roleName : kotlin.String = roleName_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPutRolesByrolenameAgents(roleName, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#chatPutRolesByrolenameAgents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#chatPutRolesByrolenameAgents")
    e.printStackTrace()
}
```

### Parameters
| **roleName** | **kotlin.String**|  | |
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

<a id="chatPutRolesByrolenameMarketplace"></a>
# **chatPutRolesByrolenameMarketplace**
> kotlin.Any chatPutRolesByrolenameMarketplace(roleName, body)

Update marketplace permissions for a role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val roleName : kotlin.String = roleName_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPutRolesByrolenameMarketplace(roleName, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#chatPutRolesByrolenameMarketplace")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#chatPutRolesByrolenameMarketplace")
    e.printStackTrace()
}
```

### Parameters
| **roleName** | **kotlin.String**|  | |
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

<a id="chatPutRolesByrolenameMcpServers"></a>
# **chatPutRolesByrolenameMcpServers**
> kotlin.Any chatPutRolesByrolenameMcpServers(roleName, body)

Update MCP servers permissions for a role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val roleName : kotlin.String = roleName_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPutRolesByrolenameMcpServers(roleName, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#chatPutRolesByrolenameMcpServers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#chatPutRolesByrolenameMcpServers")
    e.printStackTrace()
}
```

### Parameters
| **roleName** | **kotlin.String**|  | |
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

<a id="chatPutRolesByrolenameMemories"></a>
# **chatPutRolesByrolenameMemories**
> kotlin.Any chatPutRolesByrolenameMemories(roleName, body)

Update memory permissions for a role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val roleName : kotlin.String = roleName_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPutRolesByrolenameMemories(roleName, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#chatPutRolesByrolenameMemories")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#chatPutRolesByrolenameMemories")
    e.printStackTrace()
}
```

### Parameters
| **roleName** | **kotlin.String**|  | |
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

<a id="chatPutRolesByrolenamePeoplePicker"></a>
# **chatPutRolesByrolenamePeoplePicker**
> kotlin.Any chatPutRolesByrolenamePeoplePicker(roleName, body)

Update people picker permissions for a role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val roleName : kotlin.String = roleName_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPutRolesByrolenamePeoplePicker(roleName, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#chatPutRolesByrolenamePeoplePicker")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#chatPutRolesByrolenamePeoplePicker")
    e.printStackTrace()
}
```

### Parameters
| **roleName** | **kotlin.String**|  | |
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

<a id="chatPutRolesByrolenamePrompts"></a>
# **chatPutRolesByrolenamePrompts**
> kotlin.Any chatPutRolesByrolenamePrompts(roleName, body)

Update prompt permissions for a role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val roleName : kotlin.String = roleName_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPutRolesByrolenamePrompts(roleName, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#chatPutRolesByrolenamePrompts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#chatPutRolesByrolenamePrompts")
    e.printStackTrace()
}
```

### Parameters
| **roleName** | **kotlin.String**|  | |
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

<a id="chatPutRolesByrolenameRemoteAgents"></a>
# **chatPutRolesByrolenameRemoteAgents**
> kotlin.Any chatPutRolesByrolenameRemoteAgents(roleName, body)

Update remote agents permissions for a role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val roleName : kotlin.String = roleName_example // kotlin.String | 
val body : kotlin.Any = Object // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.chatPutRolesByrolenameRemoteAgents(roleName, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#chatPutRolesByrolenameRemoteAgents")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#chatPutRolesByrolenameRemoteAgents")
    e.printStackTrace()
}
```

### Parameters
| **roleName** | **kotlin.String**|  | |
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

<a id="dbCreateRole"></a>
# **dbCreateRole**
> DbCreateRole201Response dbCreateRole(id, dbCreateRoleRequest)

Create role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val id : kotlin.String = id_example // kotlin.String | 
val dbCreateRoleRequest : DbCreateRoleRequest =  // DbCreateRoleRequest | 
try {
    val result : DbCreateRole201Response = apiInstance.dbCreateRole(id, dbCreateRoleRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#dbCreateRole")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#dbCreateRole")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dbCreateRoleRequest** | [**DbCreateRoleRequest**](DbCreateRoleRequest.md)|  | |

### Return type

[**DbCreateRole201Response**](DbCreateRole201Response.md)

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

<a id="dbDeleteRole"></a>
# **dbDeleteRole**
> DbCreateRole201Response dbDeleteRole(id, name, branchId)

Delete role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val id : kotlin.String = id_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val branchId : kotlin.String = branchId_example // kotlin.String | 
try {
    val result : DbCreateRole201Response = apiInstance.dbDeleteRole(id, name, branchId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#dbDeleteRole")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#dbDeleteRole")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **branchId** | **kotlin.String**|  | |

### Return type

[**DbCreateRole201Response**](DbCreateRole201Response.md)

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

<a id="dbGetRole"></a>
# **dbGetRole**
> DbCreateRole201Response dbGetRole(id, name, branchId)

Get role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val id : kotlin.String = id_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val branchId : kotlin.String = branchId_example // kotlin.String | 
try {
    val result : DbCreateRole201Response = apiInstance.dbGetRole(id, name, branchId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#dbGetRole")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#dbGetRole")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **branchId** | **kotlin.String**|  | |

### Return type

[**DbCreateRole201Response**](DbCreateRole201Response.md)

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

<a id="dbListRoles"></a>
# **dbListRoles**
> DbListRoles200Response dbListRoles(id, branchId)

List roles

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val id : kotlin.String = id_example // kotlin.String | 
val branchId : kotlin.String = branchId_example // kotlin.String | 
try {
    val result : DbListRoles200Response = apiInstance.dbListRoles(id, branchId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#dbListRoles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#dbListRoles")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **branchId** | **kotlin.String**|  | |

### Return type

[**DbListRoles200Response**](DbListRoles200Response.md)

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

<a id="dbResetRolePassword"></a>
# **dbResetRolePassword**
> DbCreateRole201Response dbResetRolePassword(id, name, branchId)

Reset role password

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val id : kotlin.String = id_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val branchId : kotlin.String = branchId_example // kotlin.String | 
try {
    val result : DbCreateRole201Response = apiInstance.dbResetRolePassword(id, name, branchId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#dbResetRolePassword")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#dbResetRolePassword")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| **name** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **branchId** | **kotlin.String**|  | |

### Return type

[**DbCreateRole201Response**](DbCreateRole201Response.md)

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

<a id="frameworkAssignRole"></a>
# **frameworkAssignRole**
> FrameworkRole frameworkAssignRole(frameworkRole)

Assign a role to a user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val frameworkRole : FrameworkRole =  // FrameworkRole | 
try {
    val result : FrameworkRole = apiInstance.frameworkAssignRole(frameworkRole)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#frameworkAssignRole")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#frameworkAssignRole")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **frameworkRole** | [**FrameworkRole**](FrameworkRole.md)|  | |

### Return type

[**FrameworkRole**](FrameworkRole.md)

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

<a id="frameworkListRoles"></a>
# **frameworkListRoles**
> FrameworkListRoles200Response frameworkListRoles()

List per-org role assignments

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
try {
    val result : FrameworkListRoles200Response = apiInstance.frameworkListRoles()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#frameworkListRoles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#frameworkListRoles")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**FrameworkListRoles200Response**](FrameworkListRoles200Response.md)

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

<a id="frameworkRevokeRole"></a>
# **frameworkRevokeRole**
> frameworkRevokeRole(user, role)

Revoke a role from a user

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesApi()
val user : kotlin.String = user_example // kotlin.String | 
val role : kotlin.String = role_example // kotlin.String | 
try {
    apiInstance.frameworkRevokeRole(user, role)
} catch (e: ClientException) {
    println("4xx response calling RolesApi#frameworkRevokeRole")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesApi#frameworkRevokeRole")
    e.printStackTrace()
}
```

### Parameters
| **user** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **role** | **kotlin.String**|  | |

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

