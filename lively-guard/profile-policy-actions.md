# Profile Policy Actions

## Profile Policy Management Interface (IProfilePolicyManagement)

* **profilePolicyRegister():** register a new Policy entity in the Profile entity
* **profilePolicyAddRoles():** adding the Role entity to the Policy entity. Note: Policy entity can't be included Role entity at that same time it is the admin of Policy
* **profilePolicyRemoveRoles():** removing the Role entity from the Policy entity
* **profilePolicyUpdateCodes():** update the policy code of the Policy entity
* **profilePolicyUpdateAdmin():** update admin of Policy entity who is referred to specific Type or Role entity.
* **profilePolicyUpdateScope():** update Scope reference of Policy entity who is referred to specific Scope entity.
* **profilePolicyUpdateActivityStatus():** update activity status of Policy entity
* **profilePolicyUpdateAlterabilityStatus():** update the alterability status of the Policy entity
* **profilePolicyUpdateRoleLimit():** update the number of Role entities that can register in the Policy entity.
* **profilePolicyRemove():** the Policy entity will be removed from the blockchain node (storage) if it mustn't have any Role entity.
* **profilePolicyCheckId():** check Policy entity exists by ID
* **profilePolicyCheckName():** check Policy entity exists by Name
* **profilePolicyCheckAdmin():** check admin of Policy entity by account address
* **profilePolicyCheckRole():** check Role entity has been included by the Policy entity
* **profilePolicyCheckAccess():** check specific Policy entity access to specific Function entity
* **profilePolicyCheckRoleAccess():** check specific Role entity access to specific Function entity
* **profilePolicyHasRole():** check Role entity exists in the Policy entity
* **profilePolicyGetInfoByRole():** get Policy entity information by is included specific Role entity
* **profilePolicyGetInfo():** get Policy entity information by ID
* **profilePolicyGetRoles():** get whole Role IDs in the Policy entity

\
