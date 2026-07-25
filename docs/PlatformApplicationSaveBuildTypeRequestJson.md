
# PlatformApplicationSaveBuildTypeRequestJson

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **applicationId** | **kotlin.String** |  |  |
| **buildType** | [**inline**](#BuildType) |  |  |
| **dockerfile** | **kotlin.String** |  |  [optional] |
| **publishDirectory** | **kotlin.String** |  |  [optional] |
| **dockerContextPath** | **kotlin.String** |  |  [optional] |
| **dockerBuildStage** | **kotlin.String** |  |  [optional] |
| **herokuVersion** | **kotlin.String** |  |  [optional] |
| **isStaticSpa** | **kotlin.Boolean** |  |  [optional] |
| **railpackVersion** | **kotlin.String** |  |  [optional] |


<a id="BuildType"></a>
## Enum: buildType
| Name | Value |
| ---- | ----- |
| buildType | dockerfile, nixpacks, buildpacks, heroku, railpack, static |



