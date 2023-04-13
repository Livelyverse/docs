# Profile Authorize Actions

## Profile ACL General Interface (IProfileACLGenerals)

* **profileIsAgentExist():** check the Agent ID (which is one of the Type, Role, Member entities) that exists in the Profile entity
* **profileIsScopeExist():** check the Scope ID (which is one of the Function, Context, Realm, Domain, Universe entities) that exists in the Profile entity
* **profileIsPolicyExist():** check the Policy ID that exists in the Profile entity
* **profileScopeBaseInfo():** get Scope basic information by Scope ID in the Profile entity
* **profileAgentBaseInfo():** get Agent basic information by Agent ID in the Profile entity
* **profileCheckScopesCompatibility():** check scope compatibility between two scope IDs. It means two scopes have been put on a common path into the Scope hierarchy of the Profile entity.

## Profile ACL Interface (IProfileACL)

* **profileHasAccess():** check authorization by the Function ID and message sender in the Profile entity
* **profileHasMemberAccess():** check authorization by the Function and Member ID in the Profile entity
* **profileHasCSAccess():** check authorization by the contract address and Function selector ID in the Profile entity
* **profileHasAccountAccess():** check authorization by the contract address, Function selector ID, and account address in the Profile entity

\


\
\
