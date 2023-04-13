# Authorize Actions

## ACL General Interface (IACLGenerals)



* **isAgentExist():** check the Agent ID (which is one of the Type, Role, or Member entities) that exists in the Lively Guard
* **isScopeExist():** check the Scope ID (which is one of the Function, Context, Realm, Domain, or Universe entities) that exists in the Lively Guard
* **isPolicyExist():** check the Policy ID that exists in the Lively Guard
* **isProfileExist():** check the Profile ID that exists in the Lively Guard
* **scopeBaseInfo():** get Scope basic information by Scope ID in the Lively Guard
* **agentBaseInfo():** get Agent basic information by Agent ID in the Lively Guard
* **checkScopesCompatibility():** check scope compatibility between two scope IDs. It means two scopes have been put on a common path into the Scope hierarchy of the Lively Guard.

## ACL Interface (IACL)



* **hasAccess():** check authorization by the Function ID and message sender in the Lively Guard
* **hasMemberAccess():** check authorization by the Function and Member ID in the Lively Guard
* **hasCSAccess():** check authorization by the contract address and Function selector ID in the Lively Guard
* **hasAccountAccess():** check authorization by the contract address, Function selector ID, and account address in the Lively Guard

\


\
