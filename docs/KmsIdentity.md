
# KmsIdentity

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **authMethod** | [**inline**](#AuthMethod) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="AuthMethod"></a>
## Enum: authMethod
| Name | Value |
| ---- | ----- |
| authMethod | universal-auth, token-auth, kubernetes-auth, gcp-auth, aws-iam-auth, azure-auth, oidc-auth, jwt-auth, ldap-auth, tls-cert-auth, alicloud-auth, oci-auth |



