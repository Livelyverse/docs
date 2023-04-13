# Profile Agent Actions

## Profile Type Management Interface (IProfileTypeManagement)

* **profileTypeRegister():** register new Types (Departement) entity in Lively Guard
* **profileTypeUpdateAdmin():** update admin of Type entity who is referred to specific Type or Role entity or itself.
* **profileTypeUpdateScope():** update Scope reference of Type entity who is referred to specific Scope entity.
* **profileTypeUpdateActivityStatus():** update activity status of Type entity
* **profileTypeUpdateAlterabilityStatus():** update alterability status of Type entity
* **profileTypeUpdateRoleLimit():** update the number of Role entities that can register in the Type entity.
* **profileTypeRemove():** the Type entity will be removed from the blockchain node (storage) if it mustn't have any Role entity.
* **profileTypeCheckId():** check Type entity exists by ID
* **profileTypeCheckName():** check Type entity exists by Name
* **profileTypeCheckAdmin():** check admin of Type entity by account address
* **profileTypeHasAccount():** check the account address of the member exists in the Type entity
* **profileTypeHasRole():** check Role entity ID exists in the Type entity
* **profileTypeGetRoles():** get whole Role IDs in the Type entity
* **profileTypeGetInfo():** get Type entity information

## Profile Role Management Interface (IProfileRoleManagement)

* **profileRoleRegister():** register new Role entity in Type entity
* **profileRoleGrantMembers():** granting the Member entity to the Role entity
* **profileRoleRevokeMembers():** revoking the Member entity from the Role entity
* **profileRoleUpdateAdmin():** update admin of Role entity who is referred to specific Type or Role entity or itself.
* **profileRoleUpdateScope():** update Scope reference of Role entity who is referred to specific Scope entity.
* **profileRoleUpdateActivityStatus():** update the activity status of the Role entity
* **profileRoleUpdateAlterabilityStatus():** update the alterability status of the Role entity
* **profileRoleUpdateMemberLimit():** update the number of Member entities that can register in the Role entity.
* **profileRoleRemove():** the Role entity will be removed from the blockchain node (storage) if it mustn't have any Member entity.
* **profileRoleCheckId():** check Role entity exists by ID
* **profileRoleCheckName():** check Role entity exists by Name
* **profileRoleCheckAdmin():** check admin of Type entity by account address
* **profileRoleHasAccount():** check the account address of the member that exists in the Role entity
* **profileRoleGetInfo():** get Role entity information

## Profile Member Management Interface (IProfileMemberManagement)

* profileMemberRegister(): register a new Member entity in the Role entity of the Type entity, in such a way it can register in only one Role of each Type entity.
* profileMemberUpdateTypeLimit(): update the number of Type entities that Member entity can join those.
* profileMemberUpdateRegisterLimit(): update register limitations of Member entity which is related to actions member can do in the specific Profile entity.
* profileMemberUpdateCallLimit(): update the number of call functions that the Member entity can do.
* profileMemberUpdateActivityStatus(): update activity status of Member entity
* profileMemberUpdateAlterabilityStatus(): update alterability status of Member entity
* profileMemberUpdateAdmin(): update admin of Member entity who is referred to specific Type or Role entity.
* profileMemberRemove(): remove the Member entity from the blockchain node (storage)
* profileMemberCheckId(): check Member entity exists by ID
* profileMemberCheckAccount(): check Member entity exists by account address
* profileMemberCheckAdmin(): check admin of Member entity by account address
* profileMemberHasType(): check Member entity exists in Type entity

\


* profileMemberGetTypes(): get whole Type IDs in the Member entity

\


* profileMemberGetInfo(): get Member entity information

\


\


\
