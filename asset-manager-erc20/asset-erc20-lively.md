# Asset ERC20 (Lively)

It’s an interface for the Lively ERC20 asset. ERC20 asset (subject) has to implement it to support the Lively token functionalities.

## ERC20 Asset Interface (IAssetERC20)

\


* tokenLock(): calls lockToken() of Lively token with requested data by the authorized account

\


* tokenTransfer(): calls transfer() of Lively token with requested data by the authorized account

\


* tokenBatchTransfer(): calls batchTransfer() of Lively token with requested data by the authorized account

\


* tokenTransferFrom(): calls transferFrom() of Lively token with requested data by the authorized account

\


* tokenBatchTransferFrom(): calls batchTransferFrom() of Lively token with requested data by the authorized account

\


* tokenApprove(): calls approve() of Lively token with requested data by the authorized account

\


* tokenIncreaseAllowance(): calls increaseAllowance() of Lively token with requested data by the authorized account

\


* tokenDecreaseAllowance(): calls decreaseAllowance() of Lively token with requested data by the authorized account

\
