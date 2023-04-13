# Lively Token ERC20 (LIV)

## ERC20 Interface (IERC20)

* **transfer():** Transfers the number of tokens to the destination address.
* **transferFrom():** Transfers the number of tokens from the source address to the destination address. The transferFrom method is used for a withdraw workflow, allowing contracts to transfer tokens on your behalf. This can be used for example to allow a contract to transfer tokens on your behalf and/or to charge fees in sub-currencies.
* **approve():** Allows spender to withdraw from your account multiple times, up to the value amount.
* **allowance():** Returns the amount which the spender is still allowed to withdraw from the owner
* **name():** Returns the name of the token
* **symbol():** Returns the symbol of the token
* **decimals():** Returns the number of decimals the token uses
* **totalSupply():** Returns the total token supply.
* **balanceOf():** Returns the account balance of another account with the address

## ERC20 Extra Interface (IERC20Extra)

* **increaseAllowance():** Atomically increases the allowance granted to the spender by the caller.
* **decreaseAllowance():** Atomically decreases the allowance granted to the spender by the caller.
* **burn():** Destroys amount tokens from the caller.
* **mint():** Creates amount tokens and assigns them to account, increasing the total supply
* **batchTransfer():** Batch transfers the number of tokens to the destination addresses.
* **batchTransferFrom():** Batch transfers the number of tokens from the source addresses to the destination addresses.
* **updateTaxRate():** Update the tax rate percentage in the token
* **updateTaxWhitelist():** Update the tax whitelist in the token whose addresses exclude from the tax
* **permit():** Sets value as the allowance of spender over owner's tokens, given owner's signed approval.
* **taxRate():** Get the tax rate percentage from the token
* **taxTreasury():** Get the tax treasury address
* **taxWhitelist():** Get the tax whitelist addresses from the token
* **nonce():** Returns the current nonce for the owner. This value must be included whenever a signature is generated for the permit.

## ERC20 Lock Interface (IERC20Lock)

* **lockToken():** Locks the number of tokens for a period of time from the specific source address. It returns a lock ID that could be tracked and it’s put in the custody of the new owner (account address). After release time, the locked tokens withdraw to the new account address.
* **unlockToken():** Unlocks the number of tokens under release time by lock ID and returns it to the source address.
* **claimToken():** Claims (release) the number of tokens after release time to withdraw to the new account address. It can only call by the new owner.
* **lockInfo():** Get the Lock information by ID
* **totalBalanceOf():** Get adding the result of the account balance and account lock balance by account address
* **lockBalanceOf():** Get account lock balance by account address

## ERC20 Pause Interface (IERC20Pause)

* **pause():** suspends (freeze) an account address in the token
* **unpause():** unsuspends (unfreeze) an account address in the token
* **pauseAll():** suspends Token contract
* **unpauseAll():** unsuspends Token contract
* **isPaused():** checks the account address that suspends in the token
* **isPausedAll():** checks token that is suspended
* **pausedAccounts():** returns suspended accounts

\


\


\
