
# CommercePaymentRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **type** | [**inline**](#Type) |  |  [optional] |
| **token** | **kotlin.String** | Payment processor token (e.g., Stripe token) |  [optional] |
| **paymentMethodId** | **kotlin.String** |  |  [optional] |
| **amount** | **kotlin.Int** | Amount in cents (optional, defaults to order total) |  [optional] |


<a id="Type"></a>
## Enum: type
| Name | Value |
| ---- | ----- |
| type | card, paypal, stripe, bitcoin, ethereum, balance |



