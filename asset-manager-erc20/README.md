# Asset Manager ERC20

Asset management is very important when distributing tokens according to the tokenomics.

the AssetManagerERC20 can manage distributed tokens safe and secure by asset entity contracts that are compatible, and bind to specific ERC20 token. It substitutes external of accounts (EOA) with smart contracts in the tokens distribution process.

## ERC20 Asset Manager Interface (IAssetManagerERC20)

* **createAsset():** creates ERC20 asset entity that the subject (asset) contract has registered in the asset manager
* **registerAsset():** registers ERC20 asset entity that it’s already created
* **removeAsset():** removes ERC20 asset entity from assetManager
* **registerToken():** registers new ERC20 token along with its subject (asset) implementation and system admin signature
* **updateToken():** updates subject (asset) implementation or system admin signature that is related to ERC20 token address
* **setSafeModeAssets():** updates safe mode status of asset entity
* **getSafeModeAsset():** gets safe mode status of asset entity
* **getAllTokens():** gets all registered ERC20 token addresses in the asset manager
* **getTokenInfo():** gets subject (asset) implementation address and system admin signature that are related to ERC20 token
* **isAssetExists():** checks asset entity exists by Address
* **isTokenExists():** checks erc20 token exists by Address
* **predictAddress():** calculate address by create2 feature

\


\
