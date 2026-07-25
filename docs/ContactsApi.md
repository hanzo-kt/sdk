# ContactsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**crmCreateContact**](ContactsApi.md#crmCreateContact) | **POST** /v1/crm/contacts | Create a contact |
| [**crmDeleteContact**](ContactsApi.md#crmDeleteContact) | **DELETE** /v1/crm/contacts/{id} | Delete a contact (clears opportunity point-of-contact refs) |
| [**crmGetContact**](ContactsApi.md#crmGetContact) | **GET** /v1/crm/contacts/{id} | Contact detail |
| [**crmListContacts**](ContactsApi.md#crmListContacts) | **GET** /v1/crm/contacts | List contacts |
| [**crmUpdateContact**](ContactsApi.md#crmUpdateContact) | **PUT** /v1/crm/contacts/{id} | Update a contact |


<a id="crmCreateContact"></a>
# **crmCreateContact**
> CrmContact crmCreateContact(crmContactInput)

Create a contact

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContactsApi()
val crmContactInput : CrmContactInput =  // CrmContactInput | 
try {
    val result : CrmContact = apiInstance.crmCreateContact(crmContactInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContactsApi#crmCreateContact")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactsApi#crmCreateContact")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **crmContactInput** | [**CrmContactInput**](CrmContactInput.md)|  | |

### Return type

[**CrmContact**](CrmContact.md)

### Authorization


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

<a id="crmDeleteContact"></a>
# **crmDeleteContact**
> crmDeleteContact(id)

Delete a contact (clears opportunity point-of-contact refs)

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContactsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.crmDeleteContact(id)
} catch (e: ClientException) {
    println("4xx response calling ContactsApi#crmDeleteContact")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactsApi#crmDeleteContact")
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

<a id="crmGetContact"></a>
# **crmGetContact**
> CrmContact crmGetContact(id)

Contact detail

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContactsApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : CrmContact = apiInstance.crmGetContact(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContactsApi#crmGetContact")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactsApi#crmGetContact")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**CrmContact**](CrmContact.md)

### Authorization


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

<a id="crmListContacts"></a>
# **crmListContacts**
> CrmListContacts200Response crmListContacts(companyId, limit)

List contacts

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContactsApi()
val companyId : kotlin.String = companyId_example // kotlin.String | Filter to one company
val limit : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : CrmListContacts200Response = apiInstance.crmListContacts(companyId, limit)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContactsApi#crmListContacts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactsApi#crmListContacts")
    e.printStackTrace()
}
```

### Parameters
| **companyId** | **kotlin.String**| Filter to one company | [optional] |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **limit** | **kotlin.Int**|  | [optional] [default to 200] |

### Return type

[**CrmListContacts200Response**](CrmListContacts200Response.md)

### Authorization


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

<a id="crmUpdateContact"></a>
# **crmUpdateContact**
> CrmContact crmUpdateContact(id, crmContactInput)

Update a contact

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = ContactsApi()
val id : kotlin.String = id_example // kotlin.String | 
val crmContactInput : CrmContactInput =  // CrmContactInput | 
try {
    val result : CrmContact = apiInstance.crmUpdateContact(id, crmContactInput)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContactsApi#crmUpdateContact")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactsApi#crmUpdateContact")
    e.printStackTrace()
}
```

### Parameters
| **id** | **kotlin.String**|  | |
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **crmContactInput** | [**CrmContactInput**](CrmContactInput.md)|  | |

### Return type

[**CrmContact**](CrmContact.md)

### Authorization


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

