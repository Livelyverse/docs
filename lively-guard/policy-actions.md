# Policy Actions

## Policy Management Interface (IPolicyManagement)

* **policyRegister():** register new Policies entity in Lively Guard
* **policyAddRoles():** adding the Role entity to the Policy entity. Note: Policy entity can't be included Role entity at that same time it is the admin of Policy
* **policyRemoveRoles():** removing the Role entity from the Policy entity
* **policyUpdateCodes():** update the policy code of the Policy entity
* **policyUpdateAdmin():** update admin of Policy entity who is referred to specific Type or Role entity
* **policyUpdateScope():** update Scope reference of Policy entity who is referred to specific Scope entity.
* **policyUpdateActivityStatus():** update the activity status of the Policy entity
* **policyUpdateAlterabilityStatus():** update the alterability status of the Policy entity
* **policyUpdateRoleLimit():** update the number of Role entities that can register in the Policy entity.
* **policyRemove():** the Policy entity will be removed from the blockchain node (storage) if it mustn't have any Role entity.
* **policyCheckId():** check Policy entity exists by I
* **policyCheckName():** check Policy entity exists by Name
* **policyCheckAdmin():** check admin of Policy entity by account address
* **policyCheckRole():** check Role entity has been included by the Policy entit
* **policyCheckAccess():** check specific Policy entity access to specific Function entity
* **policyCheckRoleAccess():** check specific Role entity access to specific Function entity
* **policyHasRole():** check Role entity exists in the Policy entity
* **policyGetInfoByRole():** get Policy entity information by is included specific Role entity
* **policyGetInfo():** get Policy entity information by ID
* **policyGetRoles():** get whole Role IDs in the Policy entity

\
