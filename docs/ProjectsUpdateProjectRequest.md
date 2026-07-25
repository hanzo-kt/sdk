
# ProjectsUpdateProjectRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Must not be blank when supplied. |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **framework** | [**inline**](#Framework) |  |  [optional] |
| **cacheControl** | **kotlin.String** | Per-project HTML/document Cache-Control policy; must not contain newlines. |  [optional] |
| **repo** | [**ProjectsCreateProjectRequestRepo**](ProjectsCreateProjectRequestRepo.md) |  |  [optional] |


<a id="Framework"></a>
## Enum: framework
| Name | Value |
| ---- | ----- |
| framework | static, vite, next, react, astro, svelte, vue, remix, nuxt, unity, unreal, godot |



