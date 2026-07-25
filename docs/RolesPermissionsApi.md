# RolesPermissionsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**iamApiControllerAddEnforcer**](RolesPermissionsApi.md#iamApiControllerAddEnforcer) | **POST** /v1/iam/enforcers | Api Controller Add Enforcer |
| [**iamApiControllerAddModel**](RolesPermissionsApi.md#iamApiControllerAddModel) | **POST** /v1/iam/models | Api Controller Add Model |
| [**iamApiControllerAddPermission**](RolesPermissionsApi.md#iamApiControllerAddPermission) | **POST** /v1/iam/permissions | Api Controller Add Permission |
| [**iamApiControllerAddPolicy**](RolesPermissionsApi.md#iamApiControllerAddPolicy) | **POST** /v1/iam/policies | Api Controller Add Policy |
| [**iamApiControllerAddRole**](RolesPermissionsApi.md#iamApiControllerAddRole) | **POST** /v1/iam/roles | Api Controller Add Role |
| [**iamApiControllerBatchEnforce**](RolesPermissionsApi.md#iamApiControllerBatchEnforce) | **POST** /v1/iam/enforce/batch | Api Controller Batch Enforce |
| [**iamApiControllerDeleteEnforcer**](RolesPermissionsApi.md#iamApiControllerDeleteEnforcer) | **DELETE** /v1/iam/enforcers/{id} | Api Controller Delete Enforcer |
| [**iamApiControllerDeleteModel**](RolesPermissionsApi.md#iamApiControllerDeleteModel) | **DELETE** /v1/iam/models/{id} | Api Controller Delete Model |
| [**iamApiControllerDeletePermission**](RolesPermissionsApi.md#iamApiControllerDeletePermission) | **DELETE** /v1/iam/permissions/{id} | Api Controller Delete Permission |
| [**iamApiControllerDeleteRole**](RolesPermissionsApi.md#iamApiControllerDeleteRole) | **DELETE** /v1/iam/roles/{id} | Api Controller Delete Role |
| [**iamApiControllerEnforce**](RolesPermissionsApi.md#iamApiControllerEnforce) | **POST** /v1/iam/enforce | Api Controller Enforce |
| [**iamApiControllerGetAllActions**](RolesPermissionsApi.md#iamApiControllerGetAllActions) | **GET** /v1/iam/all-actions | Api Controller Get All Actions |
| [**iamApiControllerGetAllObjects**](RolesPermissionsApi.md#iamApiControllerGetAllObjects) | **GET** /v1/iam/all-objects | Api Controller Get All Objects |
| [**iamApiControllerGetAllRoles**](RolesPermissionsApi.md#iamApiControllerGetAllRoles) | **GET** /v1/iam/all-roles | Api Controller Get All Roles |
| [**iamApiControllerGetEnforcer**](RolesPermissionsApi.md#iamApiControllerGetEnforcer) | **GET** /v1/iam/enforcers/{id} | Api Controller Get Enforcer |
| [**iamApiControllerGetEnforcers**](RolesPermissionsApi.md#iamApiControllerGetEnforcers) | **GET** /v1/iam/enforcers | Api Controller Get Enforcers |
| [**iamApiControllerGetFilteredPolicies**](RolesPermissionsApi.md#iamApiControllerGetFilteredPolicies) | **GET** /v1/iam/filtered-policies | Api Controller Get Filtered Policies |
| [**iamApiControllerGetModel**](RolesPermissionsApi.md#iamApiControllerGetModel) | **GET** /v1/iam/models/{id} | Api Controller Get Model |
| [**iamApiControllerGetModels**](RolesPermissionsApi.md#iamApiControllerGetModels) | **GET** /v1/iam/models | Api Controller Get Models |
| [**iamApiControllerGetPermission**](RolesPermissionsApi.md#iamApiControllerGetPermission) | **GET** /v1/iam/permissions/{id} | Api Controller Get Permission |
| [**iamApiControllerGetPermissions**](RolesPermissionsApi.md#iamApiControllerGetPermissions) | **GET** /v1/iam/permissions | Api Controller Get Permissions |
| [**iamApiControllerGetPermissionsByRole**](RolesPermissionsApi.md#iamApiControllerGetPermissionsByRole) | **GET** /v1/iam/permissions-by-roles/{id} | Api Controller Get Permissions By Role |
| [**iamApiControllerGetPermissionsBySubmitter**](RolesPermissionsApi.md#iamApiControllerGetPermissionsBySubmitter) | **GET** /v1/iam/permissions-by-submitters/{id} | Api Controller Get Permissions By Submitter |
| [**iamApiControllerGetPolicies**](RolesPermissionsApi.md#iamApiControllerGetPolicies) | **GET** /v1/iam/policies | Api Controller Get Policies |
| [**iamApiControllerGetRole**](RolesPermissionsApi.md#iamApiControllerGetRole) | **GET** /v1/iam/roles/{id} | Api Controller Get Role |
| [**iamApiControllerGetRoles**](RolesPermissionsApi.md#iamApiControllerGetRoles) | **GET** /v1/iam/roles | Api Controller Get Roles |
| [**iamApiControllerRemovePolicy**](RolesPermissionsApi.md#iamApiControllerRemovePolicy) | **POST** /v1/iam/remove-policy | Api Controller Remove Policy |
| [**iamApiControllerRunCasbinCommand**](RolesPermissionsApi.md#iamApiControllerRunCasbinCommand) | **GET** /v1/iam/run-casbin-command | Api Controller Run Casbin Command |
| [**iamApiControllerUpdateEnforcer**](RolesPermissionsApi.md#iamApiControllerUpdateEnforcer) | **PUT** /v1/iam/enforcers/{id} | Api Controller Update Enforcer |
| [**iamApiControllerUpdateModel**](RolesPermissionsApi.md#iamApiControllerUpdateModel) | **PUT** /v1/iam/models/{id} | Api Controller Update Model |
| [**iamApiControllerUpdatePermission**](RolesPermissionsApi.md#iamApiControllerUpdatePermission) | **PUT** /v1/iam/permissions/{id} | Api Controller Update Permission |
| [**iamApiControllerUpdatePolicy**](RolesPermissionsApi.md#iamApiControllerUpdatePolicy) | **PUT** /v1/iam/policies/{id} | Api Controller Update Policy |
| [**iamApiControllerUpdateRole**](RolesPermissionsApi.md#iamApiControllerUpdateRole) | **PUT** /v1/iam/roles/{id} | Api Controller Update Role |


<a id="iamApiControllerAddEnforcer"></a>
# **iamApiControllerAddEnforcer**
> IamObjectEnforcer iamApiControllerAddEnforcer(body)

Api Controller Add Enforcer

add enforcer

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val body : kotlin.Any = Object // kotlin.Any | The enforcer object
try {
    val result : IamObjectEnforcer = apiInstance.iamApiControllerAddEnforcer(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerAddEnforcer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerAddEnforcer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The enforcer object | |

### Return type

[**IamObjectEnforcer**](IamObjectEnforcer.md)

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

<a id="iamApiControllerAddModel"></a>
# **iamApiControllerAddModel**
> IamControllersResponse iamApiControllerAddModel(iamObjectModel)

Api Controller Add Model

add model

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val iamObjectModel : IamObjectModel =  // IamObjectModel | The details of the model
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddModel(iamObjectModel)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerAddModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerAddModel")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectModel** | [**IamObjectModel**](IamObjectModel.md)| The details of the model | |

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

<a id="iamApiControllerAddPermission"></a>
# **iamApiControllerAddPermission**
> IamControllersResponse iamApiControllerAddPermission(iamObjectPermission)

Api Controller Add Permission

add permission

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val iamObjectPermission : IamObjectPermission =  // IamObjectPermission | The details of the permission
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddPermission(iamObjectPermission)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerAddPermission")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerAddPermission")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectPermission** | [**IamObjectPermission**](IamObjectPermission.md)| The details of the permission | |

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

<a id="iamApiControllerAddPolicy"></a>
# **iamApiControllerAddPolicy**
> kotlin.Any iamApiControllerAddPolicy(id, body)

Api Controller Add Policy

add policy

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name )  of enforcer
val body : kotlin.Any = Object // kotlin.Any | The policy to add
try {
    val result : kotlin.Any = apiInstance.iamApiControllerAddPolicy(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerAddPolicy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerAddPolicy")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name )  of enforcer | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The policy to add | |

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

<a id="iamApiControllerAddRole"></a>
# **iamApiControllerAddRole**
> IamControllersResponse iamApiControllerAddRole(iamObjectRole)

Api Controller Add Role

add role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val iamObjectRole : IamObjectRole =  // IamObjectRole | The details of the role
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddRole(iamObjectRole)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerAddRole")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerAddRole")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectRole** | [**IamObjectRole**](IamObjectRole.md)| The details of the role | |

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

<a id="iamApiControllerBatchEnforce"></a>
# **iamApiControllerBatchEnforce**
> IamControllersResponse iamApiControllerBatchEnforce(requestBody, permissionId, modelId, owner)

Api Controller Batch Enforce

Call Casbin BatchEnforce API

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val requestBody : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | array of casbin requests
val permissionId : kotlin.String = permissionId_example // kotlin.String | permission id
val modelId : kotlin.String = modelId_example // kotlin.String | model id
val owner : kotlin.String = owner_example // kotlin.String | owner
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerBatchEnforce(requestBody, permissionId, modelId, owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerBatchEnforce")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerBatchEnforce")
    e.printStackTrace()
}
```

### Parameters
| **requestBody** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| array of casbin requests | |
| **permissionId** | **kotlin.String**| permission id | [optional] |
| **modelId** | **kotlin.String**| model id | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| owner | [optional] |

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

<a id="iamApiControllerDeleteEnforcer"></a>
# **iamApiControllerDeleteEnforcer**
> IamObjectEnforcer iamApiControllerDeleteEnforcer(id, iamObjectEnforcer)

Api Controller Delete Enforcer

delete enforcer

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectEnforcer : IamObjectEnforcer =  // IamObjectEnforcer | The enforcer object
try {
    val result : IamObjectEnforcer = apiInstance.iamApiControllerDeleteEnforcer(id, iamObjectEnforcer)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerDeleteEnforcer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerDeleteEnforcer")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectEnforcer** | [**IamObjectEnforcer**](IamObjectEnforcer.md)| The enforcer object | |

### Return type

[**IamObjectEnforcer**](IamObjectEnforcer.md)

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

<a id="iamApiControllerDeleteModel"></a>
# **iamApiControllerDeleteModel**
> IamControllersResponse iamApiControllerDeleteModel(id, iamObjectModel)

Api Controller Delete Model

delete model

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectModel : IamObjectModel =  // IamObjectModel | The details of the model
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteModel(id, iamObjectModel)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerDeleteModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerDeleteModel")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectModel** | [**IamObjectModel**](IamObjectModel.md)| The details of the model | |

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

<a id="iamApiControllerDeletePermission"></a>
# **iamApiControllerDeletePermission**
> IamControllersResponse iamApiControllerDeletePermission(id, iamObjectPermission)

Api Controller Delete Permission

delete permission

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectPermission : IamObjectPermission =  // IamObjectPermission | The details of the permission
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeletePermission(id, iamObjectPermission)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerDeletePermission")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerDeletePermission")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectPermission** | [**IamObjectPermission**](IamObjectPermission.md)| The details of the permission | |

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

<a id="iamApiControllerDeleteRole"></a>
# **iamApiControllerDeleteRole**
> IamControllersResponse iamApiControllerDeleteRole(id, iamObjectRole)

Api Controller Delete Role

delete role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectRole : IamObjectRole =  // IamObjectRole | The details of the role
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteRole(id, iamObjectRole)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerDeleteRole")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerDeleteRole")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectRole** | [**IamObjectRole**](IamObjectRole.md)| The details of the role | |

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

<a id="iamApiControllerEnforce"></a>
# **iamApiControllerEnforce**
> IamControllersResponse iamApiControllerEnforce(requestBody, permissionId, modelId, resourceId, owner)

Api Controller Enforce

Call Casbin Enforce API

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val requestBody : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | Casbin request
val permissionId : kotlin.String = permissionId_example // kotlin.String | permission id
val modelId : kotlin.String = modelId_example // kotlin.String | model id
val resourceId : kotlin.String = resourceId_example // kotlin.String | resource id
val owner : kotlin.String = owner_example // kotlin.String | owner
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerEnforce(requestBody, permissionId, modelId, resourceId, owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerEnforce")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerEnforce")
    e.printStackTrace()
}
```

### Parameters
| **requestBody** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| Casbin request | |
| **permissionId** | **kotlin.String**| permission id | [optional] |
| **modelId** | **kotlin.String**| model id | [optional] |
| **resourceId** | **kotlin.String**| resource id | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| owner | [optional] |

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

<a id="iamApiControllerGetAllActions"></a>
# **iamApiControllerGetAllActions**
> IamControllersResponse iamApiControllerGetAllActions(userId)

Api Controller Get All Actions

Get all actions for a user (Casbin API)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val userId : kotlin.String = userId_example // kotlin.String | user id like built-in/admin
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerGetAllActions(userId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetAllActions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetAllActions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userId** | **kotlin.String**| user id like built-in/admin | [optional] |

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

<a id="iamApiControllerGetAllObjects"></a>
# **iamApiControllerGetAllObjects**
> IamControllersResponse iamApiControllerGetAllObjects(userId)

Api Controller Get All Objects

Get all objects for a user (Casbin API)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val userId : kotlin.String = userId_example // kotlin.String | user id like built-in/admin
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerGetAllObjects(userId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetAllObjects")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetAllObjects")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userId** | **kotlin.String**| user id like built-in/admin | [optional] |

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

<a id="iamApiControllerGetAllRoles"></a>
# **iamApiControllerGetAllRoles**
> IamControllersResponse iamApiControllerGetAllRoles(userId)

Api Controller Get All Roles

Get all roles for a user (Casbin API)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val userId : kotlin.String = userId_example // kotlin.String | user id like built-in/admin
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerGetAllRoles(userId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetAllRoles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetAllRoles")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userId** | **kotlin.String**| user id like built-in/admin | [optional] |

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

<a id="iamApiControllerGetEnforcer"></a>
# **iamApiControllerGetEnforcer**
> IamObjectEnforcer iamApiControllerGetEnforcer(id)

Api Controller Get Enforcer

get enforcer

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name )  of enforcer
try {
    val result : IamObjectEnforcer = apiInstance.iamApiControllerGetEnforcer(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetEnforcer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetEnforcer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name )  of enforcer | |

### Return type

[**IamObjectEnforcer**](IamObjectEnforcer.md)

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

<a id="iamApiControllerGetEnforcers"></a>
# **iamApiControllerGetEnforcers**
> kotlin.collections.List&lt;IamObjectEnforcer&gt; iamApiControllerGetEnforcers(owner)

Api Controller Get Enforcers

get enforcers

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of enforcers
try {
    val result : kotlin.collections.List<IamObjectEnforcer> = apiInstance.iamApiControllerGetEnforcers(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetEnforcers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetEnforcers")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of enforcers | |

### Return type

[**kotlin.collections.List&lt;IamObjectEnforcer&gt;**](IamObjectEnforcer.md)

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

<a id="iamApiControllerGetFilteredPolicies"></a>
# **iamApiControllerGetFilteredPolicies**
> kotlin.collections.List&lt;kotlin.Any&gt; iamApiControllerGetFilteredPolicies(id, iamObjectFilter)

Api Controller Get Filtered Policies

get filtered policies with support for multiple filters via POST body

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name )  of enforcer
val iamObjectFilter : kotlin.collections.List<IamObjectFilter> =  // kotlin.collections.List<IamObjectFilter> | Array of filter objects for multiple filters
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.iamApiControllerGetFilteredPolicies(id, iamObjectFilter)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetFilteredPolicies")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetFilteredPolicies")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name )  of enforcer | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectFilter** | [**kotlin.collections.List&lt;IamObjectFilter&gt;**](IamObjectFilter.md)| Array of filter objects for multiple filters | |

### Return type

[**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="iamApiControllerGetModel"></a>
# **iamApiControllerGetModel**
> IamObjectModel iamApiControllerGetModel(id)

Api Controller Get Model

get model

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the model
try {
    val result : IamObjectModel = apiInstance.iamApiControllerGetModel(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetModel")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the model | |

### Return type

[**IamObjectModel**](IamObjectModel.md)

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

<a id="iamApiControllerGetModels"></a>
# **iamApiControllerGetModels**
> kotlin.collections.List&lt;IamObjectModel&gt; iamApiControllerGetModels(owner)

Api Controller Get Models

get models

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of models
try {
    val result : kotlin.collections.List<IamObjectModel> = apiInstance.iamApiControllerGetModels(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetModels")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetModels")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of models | |

### Return type

[**kotlin.collections.List&lt;IamObjectModel&gt;**](IamObjectModel.md)

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

<a id="iamApiControllerGetPermission"></a>
# **iamApiControllerGetPermission**
> IamObjectPermission iamApiControllerGetPermission(id)

Api Controller Get Permission

get permission

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the permission
try {
    val result : IamObjectPermission = apiInstance.iamApiControllerGetPermission(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetPermission")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetPermission")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the permission | |

### Return type

[**IamObjectPermission**](IamObjectPermission.md)

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

<a id="iamApiControllerGetPermissions"></a>
# **iamApiControllerGetPermissions**
> kotlin.collections.List&lt;IamObjectPermission&gt; iamApiControllerGetPermissions(owner)

Api Controller Get Permissions

get permissions

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of permissions
try {
    val result : kotlin.collections.List<IamObjectPermission> = apiInstance.iamApiControllerGetPermissions(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetPermissions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetPermissions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of permissions | |

### Return type

[**kotlin.collections.List&lt;IamObjectPermission&gt;**](IamObjectPermission.md)

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

<a id="iamApiControllerGetPermissionsByRole"></a>
# **iamApiControllerGetPermissionsByRole**
> kotlin.collections.List&lt;IamObjectPermission&gt; iamApiControllerGetPermissionsByRole(id)

Api Controller Get Permissions By Role

get permissions by role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the role
try {
    val result : kotlin.collections.List<IamObjectPermission> = apiInstance.iamApiControllerGetPermissionsByRole(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetPermissionsByRole")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetPermissionsByRole")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the role | |

### Return type

[**kotlin.collections.List&lt;IamObjectPermission&gt;**](IamObjectPermission.md)

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

<a id="iamApiControllerGetPermissionsBySubmitter"></a>
# **iamApiControllerGetPermissionsBySubmitter**
> kotlin.collections.List&lt;IamObjectPermission&gt; iamApiControllerGetPermissionsBySubmitter(id)

Api Controller Get Permissions By Submitter

get permissions by submitter

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
try {
    val result : kotlin.collections.List<IamObjectPermission> = apiInstance.iamApiControllerGetPermissionsBySubmitter(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetPermissionsBySubmitter")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetPermissionsBySubmitter")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| Resource identifier (owner/name) | |

### Return type

[**kotlin.collections.List&lt;IamObjectPermission&gt;**](IamObjectPermission.md)

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

<a id="iamApiControllerGetPolicies"></a>
# **iamApiControllerGetPolicies**
> kotlin.collections.List&lt;kotlin.Any&gt; iamApiControllerGetPolicies(id, adapterId)

Api Controller Get Policies

get policies

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name )  of enforcer
val adapterId : kotlin.String = adapterId_example // kotlin.String | The adapter id
try {
    val result : kotlin.collections.List<kotlin.Any> = apiInstance.iamApiControllerGetPolicies(id, adapterId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetPolicies")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetPolicies")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name )  of enforcer | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **adapterId** | **kotlin.String**| The adapter id | [optional] |

### Return type

[**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)

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

<a id="iamApiControllerGetRole"></a>
# **iamApiControllerGetRole**
> IamObjectRole iamApiControllerGetRole(id)

Api Controller Get Role

get role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the role
try {
    val result : IamObjectRole = apiInstance.iamApiControllerGetRole(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetRole")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetRole")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the role | |

### Return type

[**IamObjectRole**](IamObjectRole.md)

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

<a id="iamApiControllerGetRoles"></a>
# **iamApiControllerGetRoles**
> kotlin.collections.List&lt;IamObjectRole&gt; iamApiControllerGetRoles(owner)

Api Controller Get Roles

get roles

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of roles
try {
    val result : kotlin.collections.List<IamObjectRole> = apiInstance.iamApiControllerGetRoles(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerGetRoles")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerGetRoles")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of roles | |

### Return type

[**kotlin.collections.List&lt;IamObjectRole&gt;**](IamObjectRole.md)

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

<a id="iamApiControllerRemovePolicy"></a>
# **iamApiControllerRemovePolicy**
> kotlin.Any iamApiControllerRemovePolicy(id, body)

Api Controller Remove Policy

remove policy

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name )  of enforcer
val body : kotlin.Any = Object // kotlin.Any | The policy to remove
try {
    val result : kotlin.Any = apiInstance.iamApiControllerRemovePolicy(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerRemovePolicy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerRemovePolicy")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name )  of enforcer | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The policy to remove | |

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

<a id="iamApiControllerRunCasbinCommand"></a>
# **iamApiControllerRunCasbinCommand**
> IamControllersResponse iamApiControllerRunCasbinCommand()

Api Controller Run Casbin Command

Call Casbin CLI commands

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerRunCasbinCommand()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerRunCasbinCommand")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerRunCasbinCommand")
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

<a id="iamApiControllerUpdateEnforcer"></a>
# **iamApiControllerUpdateEnforcer**
> IamObjectEnforcer iamApiControllerUpdateEnforcer(id, body)

Api Controller Update Enforcer

update enforcer

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name )  of enforcer
val body : kotlin.Any = Object // kotlin.Any | The enforcer object
try {
    val result : IamObjectEnforcer = apiInstance.iamApiControllerUpdateEnforcer(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerUpdateEnforcer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerUpdateEnforcer")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name )  of enforcer | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**| The enforcer object | |

### Return type

[**IamObjectEnforcer**](IamObjectEnforcer.md)

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

<a id="iamApiControllerUpdateModel"></a>
# **iamApiControllerUpdateModel**
> IamControllersResponse iamApiControllerUpdateModel(id, iamObjectModel)

Api Controller Update Model

update model

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the model
val iamObjectModel : IamObjectModel =  // IamObjectModel | The details of the model
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateModel(id, iamObjectModel)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerUpdateModel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerUpdateModel")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the model | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectModel** | [**IamObjectModel**](IamObjectModel.md)| The details of the model | |

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

<a id="iamApiControllerUpdatePermission"></a>
# **iamApiControllerUpdatePermission**
> IamControllersResponse iamApiControllerUpdatePermission(id, iamObjectPermission)

Api Controller Update Permission

update permission

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the permission
val iamObjectPermission : IamObjectPermission =  // IamObjectPermission | The details of the permission
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdatePermission(id, iamObjectPermission)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerUpdatePermission")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerUpdatePermission")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the permission | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectPermission** | [**IamObjectPermission**](IamObjectPermission.md)| The details of the permission | |

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

<a id="iamApiControllerUpdatePolicy"></a>
# **iamApiControllerUpdatePolicy**
> kotlin.Any iamApiControllerUpdatePolicy(id, requestBody)

Api Controller Update Policy

update policy

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name )  of enforcer
val requestBody : kotlin.collections.List<kotlin.Any> =  // kotlin.collections.List<kotlin.Any> | Array containing old and new policy
try {
    val result : kotlin.Any = apiInstance.iamApiControllerUpdatePolicy(id, requestBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerUpdatePolicy")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerUpdatePolicy")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name )  of enforcer | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **requestBody** | [**kotlin.collections.List&lt;kotlin.Any&gt;**](kotlin.Any.md)| Array containing old and new policy | |

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

<a id="iamApiControllerUpdateRole"></a>
# **iamApiControllerUpdateRole**
> IamControllersResponse iamApiControllerUpdateRole(id, iamObjectRole)

Api Controller Update Role

update role

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = RolesPermissionsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the role
val iamObjectRole : IamObjectRole =  // IamObjectRole | The details of the role
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateRole(id, iamObjectRole)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RolesPermissionsApi#iamApiControllerUpdateRole")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RolesPermissionsApi#iamApiControllerUpdateRole")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the role | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectRole** | [**IamObjectRole**](IamObjectRole.md)| The details of the role | |

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

