
# PlatformCreateDomainInput

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **host** | **kotlin.String** |  |  |
| **domainType** | [**inline**](#DomainType) |  |  |
| **port** | **kotlin.Int** |  |  [optional] |
| **https** | **kotlin.Boolean** |  |  [optional] |
| **path** | **kotlin.String** |  |  [optional] |
| **applicationId** | **kotlin.String** |  |  [optional] |
| **composeId** | **kotlin.String** |  |  [optional] |
| **serviceName** | **kotlin.String** |  |  [optional] |
| **certificateType** | [**inline**](#CertificateType) |  |  [optional] |


<a id="DomainType"></a>
## Enum: domainType
| Name | Value |
| ---- | ----- |
| domainType | application, compose |


<a id="CertificateType"></a>
## Enum: certificateType
| Name | Value |
| ---- | ----- |
| certificateType | none, letsencrypt, custom |



