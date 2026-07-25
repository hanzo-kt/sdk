
# DoLoadBalancerCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Friendly name; must match ^[a-z0-9]([a-z0-9-]{0,38}[a-z0-9])?$ |  |
| **region** | **kotlin.String** | DO region slug |  |
| **type** | **kotlin.String** | empty → DO default (REGIONAL) |  [optional] |
| **propertySize** | **kotlin.String** | DO size slug |  [optional] |
| **forwardingRules** | [**kotlin.collections.List&lt;DoForwardingRule&gt;**](DoForwardingRule.md) | empty → default http 80→80 |  [optional] |



