
# EdgeDomain

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **hostname** | **kotlin.String** |  |  [optional] |
| **functionSlug** | **kotlin.String** |  |  [optional] |
| **status** | [**inline**](#Status) |  |  [optional] |
| **tlsState** | [**inline**](#TlsState) |  |  [optional] |
| **verification** | [**EdgeDomainVerification**](EdgeDomainVerification.md) |  |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |


<a id="Status"></a>
## Enum: status
| Name | Value |
| ---- | ----- |
| status | pending, active, error |


<a id="TlsState"></a>
## Enum: tls_state
| Name | Value |
| ---- | ----- |
| tlsState | pending, provisioning, active, failed |



