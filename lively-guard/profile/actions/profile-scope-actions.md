# Profile Scope Actions

## Profile Universe Management Interface (IProfileUniverseManagement)

* **profileUniverseUpdateActivityStatus():** update activity status of Universe entity
* **profileUniverseUpdateAlterabilityStatus():** update alterability status of universe entity
* **profileUniverseUpdateAdmin():** update admin ID of Universe entity who is referred to specific Type or Role entity
* **profileUniverseUpdateDomainLimit():** update the number of Domain (DApp) entities that can register in the Universe entity.
* **profileUniverseCheckAdmin():** check admin of Universe entity by account address
* **profileUniverseHasFunction():** check Function ID exists in the Universe entity
* **profileUniverseHasContext():** check Context ID exists in Universe entity
* **profileUniverseHasRealm():** check Realm ID exists in the Universe entity
* **profileUniverseHasDomain():** check Domain ID exists in the Universe entity
* **profileUniverseGetDomains():** get registered domains ID from universe entity
* **profileUniverseGetInfo():** get universe entity information

## Profile Domain Management Interface (IProfileDomianManagement)



* **profileDomainRegister():** register new Domains (DApps) entity in universe entity
* **profileDomainUpdateActivityStatus():** update the activity status of the Domain entity
* **profileDomainUpdateAlterabilityStatus():** update the alterability status of the Domain entity
* **profileDomainUpdateAdmin():** update admin of Domain entity who is referred to specific Type or Role entity
* **profileDomainMoveRealm():** move the Realm entity to another Context entity. A successful move occurs if the Realm entity hasn’t been referred by any agent.
* **profileDomainUpdateRealmLimit():** update the number of Realm (Service) entities that can register in the Domain entity.
* **profileDomainRemove():** the Domain entity will be removed according to these conditions, firstly, it mustn't have any Realm entity, secondly, if it is referred by any Agent entity, the Domain entity will be removed softly, and also if it isn't referred by any Agent entity, the Domain entity will be removed from blockchain node (storage)
* **profileDomainCheckId():** check Domain entity exists by ID
* **profileDomainCheckName():** check Domain entity exists by Name
* **profileDomainCheckAdmin():** check Domain entity admin by account address
* **profileDomainHasFunction():** check Function ID exists in the Domain entity
* **profileDomainHasContext():** check Context ID exists in the Domain entity
* **profileDomainHasRealm():** check Realm ID exists in the Domain entity
* **profileDomainGetRealms():** get whole realms IDs in the Domain entity
* **profileDomainGetInfo():** get Domain entity information

## Profile Realm Management Interface (IProfileRealmManagement)



* **profileRealmRegister():** register new Realms (Services) entity in the Domain entity.
* **profileRealmUpdateAdmin():** update admin of Realm entity who is referred to specific Type or Role entity.
* **profileRealmMoveContext():** move the Context entity to another Realm entity. A successful move occurs if the Context entity hasn’t been referred by any agent.
* **profileRealmUpdateActivityStatus():** update activity status of Realm entity
* **profileRealmUpdateAlterabilityStatus():** update the alterability status of the Realm entity
* **profileRealmUpdateContextLimit():** update the number of Contexts (Contract) entities that can register in the Realm entity.
* **profileRealmRemove():** the Realm entity will be removed according to these conditions, firstly, it mustn't have any Context entity, secondly, if it is referred by any Agent entity, the Realm entity will be removed softly, and also if it isn't referred by any Agent entity, the Realm entity will be removed from blockchain node (storage)
* **profileRealmCheckId():** check Realm entity exists by ID
* **profileRealmCheckName():** check Realm entity exists by Name
* **profileRealmCheckAdmin():** check admin of Realm entity by account address
* **profileRealmHasFunction():** check Function ID exists in the Realm entity
* **profileRealmHasContext():** check Context ID exists in the Realm entity
* **profileRealmGetContexts():** get whole contexts IDs in the Realm entity
* **profileRealmGetInfo():** get the Realm entity information

## Profile Context Management Interface (IProfileContextManagement)

* **profileContextRegister():** register new Context (Contract) entity in Realm entity
* **profileContextUpdateActivityStatus():** update activity status of Context entity
* **profileContextUpdateAlterabilityStatus():** update alterability status of Context entity
* **profileContextUpdateAdmin():** update admin of Context entity who is referred to specific Type or Role entity
* **profileContextUpdateFunctionLimit():** update the number of Function entities that can register in the Context entity.
* **profileContextRemove():** the Context entity will be removed according to these conditions, firstly, it mustn't have any Function entity, secondly, if it is referred by any Agent entity, the Context entity will be removed softly, and also if it isn't referred by any Agent entity, the Context entity will be removed from blockchain node (storage)
* **profileContextCheckId():** check the Context entity exists by ID
* **profileContextCheckAccount():** check the Context entity exists by contract address
* **profileContextCheckAdmin():** check admin of the Context entity by account address
* **profileContextHasFunction():** check Function ID exists in the Context entity
* **profileContextHasSelector():** check function selector ID exists in the Context entity
* **profileContextGetFunctions():** get whole Functions IDs in Context entity
* **profileContextGetInfo():** get the Context entity information

## Profile Function Management Interface (IProfileFunctionManagement)



* **profileFunctionRegister():** register new Function entity in Context entity
* **profileFunctionUpdateAdmin():** update admin of Function entity who is referred to specific Type or Role entity
* **profileFunctionUpdateAgent():** update agent of Function entity who is referred to specific Type or Role entity
* **profileFunctionUpdateActivityStatus():** update activity status of Function entity
* **profileFunctionUpdateAlterabilityStatus():** update alterability status of Function entity
* **profileFunctionUpdatePolicyCode():** update policy code of Function entity
* **profileFunctionRemove():** the Function entity will be removed if it is referred by any Agent entity, the Function entity will be removed softly, and also if it isn't referred by any Agent entity, the Function entity will be removed from blockchain node (storage)
* **profileFunctionCheckId():** check Function entity exists by ID
* **profileFunctionCheckSelector():** check Function entity exists by function selector ID
* **profileFunctionCheckAdmin():** check admin of Function entity by account address
* **profileFunctionCheckAgent():** check agent of Function entity by account address
* **profileFunctionGetInfo():** get Function entity Information

\


\


