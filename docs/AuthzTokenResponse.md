
# AuthzTokenResponse

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **accessToken** | **kotlin.String** | JWT access token |  [optional] |
| **tokenType** | [**inline**](#TokenType) |  |  [optional] |
| **expiresIn** | **kotlin.Int** | Token lifetime in seconds |  [optional] |
| **refreshToken** | **kotlin.String** | Refresh token for obtaining new access tokens |  [optional] |
| **scope** | **kotlin.String** | Space-separated list of granted scopes |  [optional] |
| **idToken** | **kotlin.String** | OpenID Connect ID token (JWT) |  [optional] |


<a id="TokenType"></a>
## Enum: token_type
| Name | Value |
| ---- | ----- |
| tokenType | Bearer |



