
# NotifyWeb3AuthRequest

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **address** | **kotlin.String** | Ethereum wallet address |  |
| **nonce** | **kotlin.String** | Nonce obtained from /v1/iam/auth/web3-nonce |  |
| **signature** | **kotlin.String** | Wallet signature |  |
| **createAt** | **kotlin.Int** | Timestamp when signature was created |  [optional] |
| **typedData** | **kotlin.String** | The message that was signed |  [optional] |
| **walletType** | [**inline**](#WalletType) | Type of wallet used |  [optional] |


<a id="WalletType"></a>
## Enum: walletType
| Name | Value |
| ---- | ----- |
| walletType | MetaMask, WalletConnect, Coinbase, Rainbow |



