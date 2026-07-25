# PluginsApi

All URIs are relative to *https://api.hanzo.ai*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**pluginListPlugins**](PluginsApi.md#pluginListPlugins) | **GET** /v1/plugins | List mounted plugins |


<a id="pluginListPlugins"></a>
# **pluginListPlugins**
> PluginPluginList pluginListPlugins()

List mounted plugins

Returns every plugin currently mounted from the runtime manifest, as a flat list of &#x60;{name, kind, prefix}&#x60;. This is introspection only — it does not expose the plugins&#39; own routes, which live at each plugin&#39;s &#x60;prefix&#x60;. The list is empty when no manifest is configured (&#x60;CLOUD_PLUGINS&#x60; unset). 

### Example
```kotlin
// Import classes:
//import ai.hanzo.sdk.infrastructure.*
//import ai.hanzo.sdk.models.*

val apiInstance = PluginsApi()
try {
    val result : PluginPluginList = apiInstance.pluginListPlugins()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PluginsApi#pluginListPlugins")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PluginsApi#pluginListPlugins")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PluginPluginList**](PluginPluginList.md)

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

