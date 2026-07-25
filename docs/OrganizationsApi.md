# OrganizationsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**consoleDeleteOrganizationMembership**](OrganizationsApi.md#consoleDeleteOrganizationMembership) | **DELETE** /v1/console/organizations/memberships | Delete an organization membership |
| [**consoleDeleteProjectMembership**](OrganizationsApi.md#consoleDeleteProjectMembership) | **DELETE** /v1/console/projects/{projectId}/memberships | Delete a project membership |
| [**consoleListOrganizationApiKeys**](OrganizationsApi.md#consoleListOrganizationApiKeys) | **GET** /v1/console/organizations/apiKeys | Get all API keys for the organization |
| [**consoleListOrganizationMemberships**](OrganizationsApi.md#consoleListOrganizationMemberships) | **GET** /v1/console/organizations/memberships | Get all memberships for the organization |
| [**consoleListOrganizationProjects**](OrganizationsApi.md#consoleListOrganizationProjects) | **GET** /v1/console/organizations/projects | Get all projects for the organization |
| [**consoleListProjectMemberships**](OrganizationsApi.md#consoleListProjectMemberships) | **GET** /v1/console/projects/{projectId}/memberships | Get all memberships for a project |
| [**consoleUpdateOrganizationMembership**](OrganizationsApi.md#consoleUpdateOrganizationMembership) | **PUT** /v1/console/organizations/memberships | Create or update an organization membership |
| [**consoleUpdateProjectMembership**](OrganizationsApi.md#consoleUpdateProjectMembership) | **PUT** /v1/console/projects/{projectId}/memberships | Create or update a project membership |
| [**iamApiControllerAddGroup**](OrganizationsApi.md#iamApiControllerAddGroup) | **POST** /v1/iam/groups | Api Controller Add Group |
| [**iamApiControllerAddInvitation**](OrganizationsApi.md#iamApiControllerAddInvitation) | **POST** /v1/iam/invitations | Api Controller Add Invitation |
| [**iamApiControllerAddOrganization**](OrganizationsApi.md#iamApiControllerAddOrganization) | **POST** /v1/iam/organizations | Api Controller Add Organization |
| [**iamApiControllerDeleteGroup**](OrganizationsApi.md#iamApiControllerDeleteGroup) | **DELETE** /v1/iam/groups/{id} | Api Controller Delete Group |
| [**iamApiControllerDeleteInvitation**](OrganizationsApi.md#iamApiControllerDeleteInvitation) | **DELETE** /v1/iam/invitations/{id} | Api Controller Delete Invitation |
| [**iamApiControllerDeleteOrganization**](OrganizationsApi.md#iamApiControllerDeleteOrganization) | **DELETE** /v1/iam/organizations/{id} | Api Controller Delete Organization |
| [**iamApiControllerGetDefaultApplication**](OrganizationsApi.md#iamApiControllerGetDefaultApplication) | **GET** /v1/iam/applications/default | Api Controller Get Default Application |
| [**iamApiControllerGetGroup**](OrganizationsApi.md#iamApiControllerGetGroup) | **GET** /v1/iam/groups/{id} | Api Controller Get Group |
| [**iamApiControllerGetGroups**](OrganizationsApi.md#iamApiControllerGetGroups) | **GET** /v1/iam/groups | Api Controller Get Groups |
| [**iamApiControllerGetInvitation**](OrganizationsApi.md#iamApiControllerGetInvitation) | **GET** /v1/iam/invitations/{id} | Api Controller Get Invitation |
| [**iamApiControllerGetInvitationCodeInfo**](OrganizationsApi.md#iamApiControllerGetInvitationCodeInfo) | **GET** /v1/iam/invitation-infos/{id} | Api Controller Get Invitation Code Info |
| [**iamApiControllerGetInvitations**](OrganizationsApi.md#iamApiControllerGetInvitations) | **GET** /v1/iam/invitations | Api Controller Get Invitations |
| [**iamApiControllerGetOrganization**](OrganizationsApi.md#iamApiControllerGetOrganization) | **GET** /v1/iam/organizations/{id} | Api Controller Get Organization |
| [**iamApiControllerGetOrganizationNames**](OrganizationsApi.md#iamApiControllerGetOrganizationNames) | **GET** /v1/iam/organizations/names | Api Controller Get Organization Names |
| [**iamApiControllerGetOrganizations**](OrganizationsApi.md#iamApiControllerGetOrganizations) | **GET** /v1/iam/organizations | Api Controller Get Organizations |
| [**iamApiControllerUpdateGroup**](OrganizationsApi.md#iamApiControllerUpdateGroup) | **PUT** /v1/iam/groups/{id} | Api Controller Update Group |
| [**iamApiControllerUpdateInvitation**](OrganizationsApi.md#iamApiControllerUpdateInvitation) | **PUT** /v1/iam/invitations/{id} | Api Controller Update Invitation |
| [**iamApiControllerUpdateOrganization**](OrganizationsApi.md#iamApiControllerUpdateOrganization) | **PUT** /v1/iam/organizations/{id} | Api Controller Update Organization |
| [**iamApiControllerVerifyInvitationGet**](OrganizationsApi.md#iamApiControllerVerifyInvitationGet) | **GET** /v1/iam/invitations/verify | Api Controller Verify Invitation |
| [**iamApiControllerVerifyInvitationPost**](OrganizationsApi.md#iamApiControllerVerifyInvitationPost) | **POST** /v1/iam/invitations/send | Api Controller Verify Invitation |
| [**kmsGetOrganization**](OrganizationsApi.md#kmsGetOrganization) | **GET** /v1/kms/organization/{organizationId} | Get an organization by ID |
| [**kmsListOrganizations**](OrganizationsApi.md#kmsListOrganizations) | **GET** /v1/kms/organization | List organizations the user belongs to |
| [**kmsUpdateOrganization**](OrganizationsApi.md#kmsUpdateOrganization) | **PATCH** /v1/kms/organization/{organizationId} | Update an organization |
| [**paasCreateOrganization**](OrganizationsApi.md#paasCreateOrganization) | **POST** /v1/paas/org | Create organization |
| [**paasDeleteOrganization**](OrganizationsApi.md#paasDeleteOrganization) | **DELETE** /v1/paas/org/{orgId} | Delete organization |
| [**paasGetOrganization**](OrganizationsApi.md#paasGetOrganization) | **GET** /v1/paas/org/{orgId} | Get organization |
| [**paasListOrganizations**](OrganizationsApi.md#paasListOrganizations) | **GET** /v1/paas/org | List organizations |
| [**paasUpdateOrganization**](OrganizationsApi.md#paasUpdateOrganization) | **PUT** /v1/paas/org/{orgId} | Update organization |


<a id="consoleDeleteOrganizationMembership"></a>
# **consoleDeleteOrganizationMembership**
> ConsoleDeleteOrganizationMembership200Response consoleDeleteOrganizationMembership(consoleDeleteOrganizationMembershipRequest)

Delete an organization membership

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val consoleDeleteOrganizationMembershipRequest : ConsoleDeleteOrganizationMembershipRequest =  // ConsoleDeleteOrganizationMembershipRequest | 
try {
    val result : ConsoleDeleteOrganizationMembership200Response = apiInstance.consoleDeleteOrganizationMembership(consoleDeleteOrganizationMembershipRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#consoleDeleteOrganizationMembership")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#consoleDeleteOrganizationMembership")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleDeleteOrganizationMembershipRequest** | [**ConsoleDeleteOrganizationMembershipRequest**](ConsoleDeleteOrganizationMembershipRequest.md)|  | |

### Return type

[**ConsoleDeleteOrganizationMembership200Response**](ConsoleDeleteOrganizationMembership200Response.md)

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

<a id="consoleDeleteProjectMembership"></a>
# **consoleDeleteProjectMembership**
> ConsoleDeleteOrganizationMembership200Response consoleDeleteProjectMembership(projectId, consoleDeleteOrganizationMembershipRequest)

Delete a project membership

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val projectId : kotlin.String = projectId_example // kotlin.String | 
val consoleDeleteOrganizationMembershipRequest : ConsoleDeleteOrganizationMembershipRequest =  // ConsoleDeleteOrganizationMembershipRequest | 
try {
    val result : ConsoleDeleteOrganizationMembership200Response = apiInstance.consoleDeleteProjectMembership(projectId, consoleDeleteOrganizationMembershipRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#consoleDeleteProjectMembership")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#consoleDeleteProjectMembership")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleDeleteOrganizationMembershipRequest** | [**ConsoleDeleteOrganizationMembershipRequest**](ConsoleDeleteOrganizationMembershipRequest.md)|  | |

### Return type

[**ConsoleDeleteOrganizationMembership200Response**](ConsoleDeleteOrganizationMembership200Response.md)

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

<a id="consoleListOrganizationApiKeys"></a>
# **consoleListOrganizationApiKeys**
> ConsoleListOrganizationApiKeys200Response consoleListOrganizationApiKeys()

Get all API keys for the organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
try {
    val result : ConsoleListOrganizationApiKeys200Response = apiInstance.consoleListOrganizationApiKeys()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#consoleListOrganizationApiKeys")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#consoleListOrganizationApiKeys")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="consoleListOrganizationMemberships"></a>
# **consoleListOrganizationMemberships**
> ConsoleListOrganizationMemberships200Response consoleListOrganizationMemberships()

Get all memberships for the organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
try {
    val result : ConsoleListOrganizationMemberships200Response = apiInstance.consoleListOrganizationMemberships()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#consoleListOrganizationMemberships")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#consoleListOrganizationMemberships")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ConsoleListOrganizationMemberships200Response**](ConsoleListOrganizationMemberships200Response.md)

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

<a id="consoleListOrganizationProjects"></a>
# **consoleListOrganizationProjects**
> ConsoleListOrganizationProjects200Response consoleListOrganizationProjects()

Get all projects for the organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
try {
    val result : ConsoleListOrganizationProjects200Response = apiInstance.consoleListOrganizationProjects()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#consoleListOrganizationProjects")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#consoleListOrganizationProjects")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ConsoleListOrganizationProjects200Response**](ConsoleListOrganizationProjects200Response.md)

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

<a id="consoleListProjectMemberships"></a>
# **consoleListProjectMemberships**
> ConsoleListOrganizationMemberships200Response consoleListProjectMemberships(projectId)

Get all memberships for a project

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val projectId : kotlin.String = projectId_example // kotlin.String | 
try {
    val result : ConsoleListOrganizationMemberships200Response = apiInstance.consoleListProjectMemberships(projectId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#consoleListProjectMemberships")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#consoleListProjectMemberships")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **projectId** | **kotlin.String**|  | |

### Return type

[**ConsoleListOrganizationMemberships200Response**](ConsoleListOrganizationMemberships200Response.md)

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

<a id="consoleUpdateOrganizationMembership"></a>
# **consoleUpdateOrganizationMembership**
> ConsoleMembership consoleUpdateOrganizationMembership(consoleUpdateOrganizationMembershipRequest)

Create or update an organization membership

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val consoleUpdateOrganizationMembershipRequest : ConsoleUpdateOrganizationMembershipRequest =  // ConsoleUpdateOrganizationMembershipRequest | 
try {
    val result : ConsoleMembership = apiInstance.consoleUpdateOrganizationMembership(consoleUpdateOrganizationMembershipRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#consoleUpdateOrganizationMembership")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#consoleUpdateOrganizationMembership")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleUpdateOrganizationMembershipRequest** | [**ConsoleUpdateOrganizationMembershipRequest**](ConsoleUpdateOrganizationMembershipRequest.md)|  | |

### Return type

[**ConsoleMembership**](ConsoleMembership.md)

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

<a id="consoleUpdateProjectMembership"></a>
# **consoleUpdateProjectMembership**
> ConsoleMembership consoleUpdateProjectMembership(projectId, consoleUpdateOrganizationMembershipRequest)

Create or update a project membership

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val projectId : kotlin.String = projectId_example // kotlin.String | 
val consoleUpdateOrganizationMembershipRequest : ConsoleUpdateOrganizationMembershipRequest =  // ConsoleUpdateOrganizationMembershipRequest | 
try {
    val result : ConsoleMembership = apiInstance.consoleUpdateProjectMembership(projectId, consoleUpdateOrganizationMembershipRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#consoleUpdateProjectMembership")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#consoleUpdateProjectMembership")
    e.printStackTrace()
}
```

### Parameters
| **projectId** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **consoleUpdateOrganizationMembershipRequest** | [**ConsoleUpdateOrganizationMembershipRequest**](ConsoleUpdateOrganizationMembershipRequest.md)|  | |

### Return type

[**ConsoleMembership**](ConsoleMembership.md)

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

<a id="iamApiControllerAddGroup"></a>
# **iamApiControllerAddGroup**
> IamControllersResponse iamApiControllerAddGroup(iamObjectGroup)

Api Controller Add Group

add group

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val iamObjectGroup : IamObjectGroup =  // IamObjectGroup | The details of the group
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddGroup(iamObjectGroup)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerAddGroup")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerAddGroup")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectGroup** | [**IamObjectGroup**](IamObjectGroup.md)| The details of the group | |

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

<a id="iamApiControllerAddInvitation"></a>
# **iamApiControllerAddInvitation**
> IamControllersResponse iamApiControllerAddInvitation(iamObjectInvitation)

Api Controller Add Invitation

add invitation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val iamObjectInvitation : IamObjectInvitation =  // IamObjectInvitation | The details of the invitation
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddInvitation(iamObjectInvitation)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerAddInvitation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerAddInvitation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectInvitation** | [**IamObjectInvitation**](IamObjectInvitation.md)| The details of the invitation | |

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

<a id="iamApiControllerAddOrganization"></a>
# **iamApiControllerAddOrganization**
> IamControllersResponse iamApiControllerAddOrganization(iamObjectOrganization)

Api Controller Add Organization

add organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val iamObjectOrganization : IamObjectOrganization =  // IamObjectOrganization | The details of the organization
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerAddOrganization(iamObjectOrganization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerAddOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerAddOrganization")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectOrganization** | [**IamObjectOrganization**](IamObjectOrganization.md)| The details of the organization | |

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

<a id="iamApiControllerDeleteGroup"></a>
# **iamApiControllerDeleteGroup**
> IamControllersResponse iamApiControllerDeleteGroup(id, iamObjectGroup)

Api Controller Delete Group

delete group

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectGroup : IamObjectGroup =  // IamObjectGroup | The details of the group
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteGroup(id, iamObjectGroup)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerDeleteGroup")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerDeleteGroup")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectGroup** | [**IamObjectGroup**](IamObjectGroup.md)| The details of the group | |

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

<a id="iamApiControllerDeleteInvitation"></a>
# **iamApiControllerDeleteInvitation**
> IamControllersResponse iamApiControllerDeleteInvitation(id, iamObjectInvitation)

Api Controller Delete Invitation

delete invitation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectInvitation : IamObjectInvitation =  // IamObjectInvitation | The details of the invitation
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteInvitation(id, iamObjectInvitation)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerDeleteInvitation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerDeleteInvitation")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectInvitation** | [**IamObjectInvitation**](IamObjectInvitation.md)| The details of the invitation | |

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

<a id="iamApiControllerDeleteOrganization"></a>
# **iamApiControllerDeleteOrganization**
> IamControllersResponse iamApiControllerDeleteOrganization(id, iamObjectOrganization)

Api Controller Delete Organization

delete organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val iamObjectOrganization : IamObjectOrganization =  // IamObjectOrganization | The details of the organization
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerDeleteOrganization(id, iamObjectOrganization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerDeleteOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerDeleteOrganization")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectOrganization** | [**IamObjectOrganization**](IamObjectOrganization.md)| The details of the organization | |

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

<a id="iamApiControllerGetDefaultApplication"></a>
# **iamApiControllerGetDefaultApplication**
> IamControllersResponse iamApiControllerGetDefaultApplication(id)

Api Controller Get Default Application

get default application

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val id : kotlin.String = id_example // kotlin.String | organization id
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerGetDefaultApplication(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerGetDefaultApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerGetDefaultApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| organization id | |

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

<a id="iamApiControllerGetGroup"></a>
# **iamApiControllerGetGroup**
> IamObjectGroup iamApiControllerGetGroup(id)

Api Controller Get Group

get group

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the group
try {
    val result : IamObjectGroup = apiInstance.iamApiControllerGetGroup(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerGetGroup")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerGetGroup")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the group | |

### Return type

[**IamObjectGroup**](IamObjectGroup.md)

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

<a id="iamApiControllerGetGroups"></a>
# **iamApiControllerGetGroups**
> kotlin.collections.List&lt;IamObjectGroup&gt; iamApiControllerGetGroups(owner)

Api Controller Get Groups

get groups

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of groups
try {
    val result : kotlin.collections.List<IamObjectGroup> = apiInstance.iamApiControllerGetGroups(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerGetGroups")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerGetGroups")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of groups | |

### Return type

[**kotlin.collections.List&lt;IamObjectGroup&gt;**](IamObjectGroup.md)

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

<a id="iamApiControllerGetInvitation"></a>
# **iamApiControllerGetInvitation**
> IamObjectInvitation iamApiControllerGetInvitation(id)

Api Controller Get Invitation

get invitation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the invitation
try {
    val result : IamObjectInvitation = apiInstance.iamApiControllerGetInvitation(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerGetInvitation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerGetInvitation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the invitation | |

### Return type

[**IamObjectInvitation**](IamObjectInvitation.md)

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

<a id="iamApiControllerGetInvitationCodeInfo"></a>
# **iamApiControllerGetInvitationCodeInfo**
> IamObjectInvitation iamApiControllerGetInvitationCodeInfo(id, code)

Api Controller Get Invitation Code Info

get invitation code information

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val id : kotlin.String = id_example // kotlin.String | Resource identifier (owner/name)
val code : kotlin.String = code_example // kotlin.String | Invitation code
try {
    val result : IamObjectInvitation = apiInstance.iamApiControllerGetInvitationCodeInfo(id, code)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerGetInvitationCodeInfo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerGetInvitationCodeInfo")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| Resource identifier (owner/name) | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **code** | **kotlin.String**| Invitation code | |

### Return type

[**IamObjectInvitation**](IamObjectInvitation.md)

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

<a id="iamApiControllerGetInvitations"></a>
# **iamApiControllerGetInvitations**
> kotlin.collections.List&lt;IamObjectInvitation&gt; iamApiControllerGetInvitations(owner)

Api Controller Get Invitations

get invitations

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val owner : kotlin.String = owner_example // kotlin.String | The owner of invitations
try {
    val result : kotlin.collections.List<IamObjectInvitation> = apiInstance.iamApiControllerGetInvitations(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerGetInvitations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerGetInvitations")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| The owner of invitations | |

### Return type

[**kotlin.collections.List&lt;IamObjectInvitation&gt;**](IamObjectInvitation.md)

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

<a id="iamApiControllerGetOrganization"></a>
# **iamApiControllerGetOrganization**
> IamObjectOrganization iamApiControllerGetOrganization(id)

Api Controller Get Organization

get organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val id : kotlin.String = id_example // kotlin.String | organization id
try {
    val result : IamObjectOrganization = apiInstance.iamApiControllerGetOrganization(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerGetOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerGetOrganization")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| organization id | |

### Return type

[**IamObjectOrganization**](IamObjectOrganization.md)

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

<a id="iamApiControllerGetOrganizationNames"></a>
# **iamApiControllerGetOrganizationNames**
> kotlin.collections.List&lt;IamObjectOrganization&gt; iamApiControllerGetOrganizationNames(owner)

Api Controller Get Organization Names

get all organization name and displayName

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val owner : kotlin.String = owner_example // kotlin.String | owner
try {
    val result : kotlin.collections.List<IamObjectOrganization> = apiInstance.iamApiControllerGetOrganizationNames(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerGetOrganizationNames")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerGetOrganizationNames")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| owner | |

### Return type

[**kotlin.collections.List&lt;IamObjectOrganization&gt;**](IamObjectOrganization.md)

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

<a id="iamApiControllerGetOrganizations"></a>
# **iamApiControllerGetOrganizations**
> kotlin.collections.List&lt;IamObjectOrganization&gt; iamApiControllerGetOrganizations(owner)

Api Controller Get Organizations

get organizations

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val owner : kotlin.String = owner_example // kotlin.String | owner
try {
    val result : kotlin.collections.List<IamObjectOrganization> = apiInstance.iamApiControllerGetOrganizations(owner)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerGetOrganizations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerGetOrganizations")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **owner** | **kotlin.String**| owner | |

### Return type

[**kotlin.collections.List&lt;IamObjectOrganization&gt;**](IamObjectOrganization.md)

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

<a id="iamApiControllerUpdateGroup"></a>
# **iamApiControllerUpdateGroup**
> IamControllersResponse iamApiControllerUpdateGroup(id, iamObjectGroup)

Api Controller Update Group

update group

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the group
val iamObjectGroup : IamObjectGroup =  // IamObjectGroup | The details of the group
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateGroup(id, iamObjectGroup)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerUpdateGroup")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerUpdateGroup")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the group | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectGroup** | [**IamObjectGroup**](IamObjectGroup.md)| The details of the group | |

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

<a id="iamApiControllerUpdateInvitation"></a>
# **iamApiControllerUpdateInvitation**
> IamControllersResponse iamApiControllerUpdateInvitation(id, iamObjectInvitation)

Api Controller Update Invitation

update invitation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the invitation
val iamObjectInvitation : IamObjectInvitation =  // IamObjectInvitation | The details of the invitation
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateInvitation(id, iamObjectInvitation)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerUpdateInvitation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerUpdateInvitation")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the invitation | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectInvitation** | [**IamObjectInvitation**](IamObjectInvitation.md)| The details of the invitation | |

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

<a id="iamApiControllerUpdateOrganization"></a>
# **iamApiControllerUpdateOrganization**
> IamControllersResponse iamApiControllerUpdateOrganization(id, iamObjectOrganization)

Api Controller Update Organization

update organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the organization
val iamObjectOrganization : IamObjectOrganization =  // IamObjectOrganization | The details of the organization
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerUpdateOrganization(id, iamObjectOrganization)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerUpdateOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerUpdateOrganization")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the organization | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iamObjectOrganization** | [**IamObjectOrganization**](IamObjectOrganization.md)| The details of the organization | |

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

<a id="iamApiControllerVerifyInvitationGet"></a>
# **iamApiControllerVerifyInvitationGet**
> IamControllersResponse iamApiControllerVerifyInvitationGet(id)

Api Controller Verify Invitation

verify invitation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the invitation
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerVerifyInvitationGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerVerifyInvitationGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerVerifyInvitationGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**| The id ( owner/name ) of the invitation | |

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

<a id="iamApiControllerVerifyInvitationPost"></a>
# **iamApiControllerVerifyInvitationPost**
> IamControllersResponse iamApiControllerVerifyInvitationPost(id, requestBody)

Api Controller Verify Invitation

verify invitation

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val id : kotlin.String = id_example // kotlin.String | The id ( owner/name ) of the invitation
val requestBody : kotlin.collections.List<kotlin.String> =  // kotlin.collections.List<kotlin.String> | The details of the invitation
try {
    val result : IamControllersResponse = apiInstance.iamApiControllerVerifyInvitationPost(id, requestBody)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#iamApiControllerVerifyInvitationPost")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#iamApiControllerVerifyInvitationPost")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**| The id ( owner/name ) of the invitation | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **requestBody** | [**kotlin.collections.List&lt;kotlin.String&gt;**](kotlin.String.md)| The details of the invitation | |

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

<a id="kmsGetOrganization"></a>
# **kmsGetOrganization**
> KmsGetOrganization200Response kmsGetOrganization(organizationId)

Get an organization by ID

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val organizationId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KmsGetOrganization200Response = apiInstance.kmsGetOrganization(organizationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#kmsGetOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#kmsGetOrganization")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **organizationId** | **java.util.UUID**|  | |

### Return type

[**KmsGetOrganization200Response**](KmsGetOrganization200Response.md)

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

<a id="kmsListOrganizations"></a>
# **kmsListOrganizations**
> KmsListOrganizations200Response kmsListOrganizations()

List organizations the user belongs to

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
try {
    val result : KmsListOrganizations200Response = apiInstance.kmsListOrganizations()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#kmsListOrganizations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#kmsListOrganizations")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**KmsListOrganizations200Response**](KmsListOrganizations200Response.md)

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

<a id="kmsUpdateOrganization"></a>
# **kmsUpdateOrganization**
> KmsGetOrganization200Response kmsUpdateOrganization(organizationId, kmsUpdateOrganizationRequest)

Update an organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val organizationId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kmsUpdateOrganizationRequest : KmsUpdateOrganizationRequest =  // KmsUpdateOrganizationRequest | 
try {
    val result : KmsGetOrganization200Response = apiInstance.kmsUpdateOrganization(organizationId, kmsUpdateOrganizationRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#kmsUpdateOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#kmsUpdateOrganization")
    e.printStackTrace()
}
```

### Parameters
| **organizationId** | **java.util.UUID**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kmsUpdateOrganizationRequest** | [**KmsUpdateOrganizationRequest**](KmsUpdateOrganizationRequest.md)|  | |

### Return type

[**KmsGetOrganization200Response**](KmsGetOrganization200Response.md)

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

<a id="paasCreateOrganization"></a>
# **paasCreateOrganization**
> PaasOrganization paasCreateOrganization(paasCreateOrganizationRequest)

Create organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val paasCreateOrganizationRequest : PaasCreateOrganizationRequest =  // PaasCreateOrganizationRequest | 
try {
    val result : PaasOrganization = apiInstance.paasCreateOrganization(paasCreateOrganizationRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#paasCreateOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#paasCreateOrganization")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **paasCreateOrganizationRequest** | [**PaasCreateOrganizationRequest**](PaasCreateOrganizationRequest.md)|  | |

### Return type

[**PaasOrganization**](PaasOrganization.md)

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

<a id="paasDeleteOrganization"></a>
# **paasDeleteOrganization**
> kotlin.Any paasDeleteOrganization(orgId)

Delete organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.paasDeleteOrganization(orgId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#paasDeleteOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#paasDeleteOrganization")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orgId** | **kotlin.String**|  | |

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

<a id="paasGetOrganization"></a>
# **paasGetOrganization**
> PaasOrganization paasGetOrganization(orgId)

Get organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
try {
    val result : PaasOrganization = apiInstance.paasGetOrganization(orgId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#paasGetOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#paasGetOrganization")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orgId** | **kotlin.String**|  | |

### Return type

[**PaasOrganization**](PaasOrganization.md)

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

<a id="paasListOrganizations"></a>
# **paasListOrganizations**
> kotlin.collections.List&lt;PaasOrganization&gt; paasListOrganizations()

List organizations

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
try {
    val result : kotlin.collections.List<PaasOrganization> = apiInstance.paasListOrganizations()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#paasListOrganizations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#paasListOrganizations")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;PaasOrganization&gt;**](PaasOrganization.md)

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

<a id="paasUpdateOrganization"></a>
# **paasUpdateOrganization**
> kotlin.Any paasUpdateOrganization(orgId, paasUpdateOrganizationRequest)

Update organization

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = OrganizationsApi()
val orgId : kotlin.String = orgId_example // kotlin.String | 
val paasUpdateOrganizationRequest : PaasUpdateOrganizationRequest =  // PaasUpdateOrganizationRequest | 
try {
    val result : kotlin.Any = apiInstance.paasUpdateOrganization(orgId, paasUpdateOrganizationRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrganizationsApi#paasUpdateOrganization")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrganizationsApi#paasUpdateOrganization")
    e.printStackTrace()
}
```

### Parameters
| **orgId** | **kotlin.String**|  | |
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

