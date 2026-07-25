
# FrameworkDocType

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** |  |  |
| **fields** | [**kotlin.collections.List&lt;FrameworkDocField&gt;**](FrameworkDocField.md) |  |  |
| **module** | **kotlin.String** |  |  [optional] |
| **isSingle** | **kotlin.Boolean** | Exactly one document exists |  [optional] |
| **isSubmittable** | **kotlin.Boolean** | Has the submit/cancel lifecycle |  [optional] |
| **autoname** | **kotlin.String** | \&quot;\&quot; or hash → random id; \&quot;field:x\&quot;; \&quot;prompt\&quot;; or a series pattern e.g. \&quot;INV-.YYYY.-.#####\&quot; |  [optional] |
| **titleField** | **kotlin.String** |  |  [optional] |
| **permissions** | [**kotlin.collections.List&lt;FrameworkDocPerm&gt;**](FrameworkDocPerm.md) |  |  [optional] |
| **createdAt** | **kotlin.Long** |  |  [optional] |
| **updatedAt** | **kotlin.Long** |  |  [optional] |



