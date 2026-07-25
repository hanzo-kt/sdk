
# ProjectsCreateProjectRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Display name (required). |  |
| **slug** | **kotlin.String** | Org-unique handle; derived from name when omitted. |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **framework** | [**inline**](#Framework) | Build hint; defaults to \&quot;static\&quot;. |  [optional] |
| **repo** | [**ProjectsCreateProjectRequestRepo**](ProjectsCreateProjectRequestRepo.md) |  |  [optional] |


<a id="Framework"></a>
## Enum: framework
| Name | Value |
| ---- | ----- |
| framework | static, vite, next, react, astro, svelte, vue, remix, nuxt, unity, unreal, godot |



