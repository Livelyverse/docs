# Asset

It’s a general interface for asset basic functionality. Any asset (subject) implementations have to implement it. The AssetManager only register asset who has implemented IAssetEntity.

## Common Asset Entity Interface (IAssetEntity)

* **assetInitialize():** initialize asset by required data
* **assetSetSafeMode():** update asset safe mode status
* **assetSafeMode():** get the safe mode status of the asset
* **assetType():** get token type of asset
* **assetToken():** get token address of asset
* **assetName():** get asset name
* **assetVersion():** get asset version
* **assetAccessControl():** get ACL of asset
* **assetInitVersion():** get initialize version of asset
* **assetBalance():** get asset balance
* **assetInfo():** get asset information

\
