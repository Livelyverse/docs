# Agent Actions

## Type Management Interface (ITypeManagement)



* **typeRegister():** register new Types (Departement) entity in Lively Guard
* **typeUpdateAdmin():** update admin of Type entity who is referred to specific Type or Role entity or itself.
* **typeUpdateScope():** update Scope reference of Type entity who is referred to specific Scope entity.
* **typeUpdateActivityStatus():** update activity status of Type entity
* **typeUpdateAlterabilityStatus():** update alterability status of Type entity
* t**ypeUpdateRoleLimit():** update the number of Role entities that can register in the Type entity.
* **typeRemove():** the Type entity will be removed from the blockchain node (storage) if it mustn't have any Role entity.
* **typeCheckId():** check Type entity exists by ID
* **typeCheckName():** check Type entity exists by Name
* **typeCheckAdmin():** check admin of Type entity by account address
* **typeHasAccount():** check the account address of the member that exists in the Type entity
* **typeHasRole():** check Role entity ID exists in the Type entity
* **typeGetRoles():** get whole Role IDs in the Type entity
* **typeGetInfo():** get information of Type entity

## Role Management Interface (IRoleManagement)

* **roleRegister():** register new Role entity in Type entity
* **roleGrantMembers():** granting the Member entity to the Role entity
* **roleRevokeMembers():** revoking the Member entity from the Role entity
* **roleUpdateAdmin():** update admin of Role entity who is referred to specific Type or Role entity or itself.
* **roleUpdateScope():** update Scope reference of Role entity who is referred to specific Scope entity.
* **roleUpdateActivityStatus():** update the activity status of the Role entity
* **roleUpdateAlterabilityStatus():** update the alterability status of the Role entity
* **roleUpdateMemberLimit():** update the number of Member entities that can register in the Role entity.
* **roleRemove():** the Role entity will be removed from the blockchain node (storage) if it mustn't have any Member entity.
* **roleCheckId():** check Role entity exists by ID
* **roleCheckName():** check Role entity exists by Name
* **roleCheckAdmin():** check admin of Type entity by account address
* **roleHasAccount():** check the account address of the member that exists in the Role entity
* **roleGetInfo():** get information of Role entity

\
Member Management Interface (IMemberManagement)
-----------------------------------------------

* **memberRegister():** register new Members entity in the Role entity of the Type entity, in such a way it can register in only one Role of each Type entity.
* **memberUpdateActivityStatus():** update activity status of Member entity
* **memberUpdateAlterabilityStatus():** update alterability status of Member entity
* **memberUpdateAdmin():** update admin of Member entity who is referred to specific Type or Role entity.
* **memberUpdateGeneralLimit():** update general limitations of Member entity which is related to actions member can do in the Lively Guard
* **memberRemove():** remove the Member entity from the blockchain node (storage)
* **memberCheckId():** check Member entity exists by ID
* **memberCheckAccount():** check Member entity exists by account address
* **memberCheckAdmin():** check admin of Member entity by account address
* **memberHasType():** check Member entity exists in Type entity
* **memberGetTypes():** get whole Type IDs in the Member entity
* **memberGetInfo():** get Member entity information

\


\
