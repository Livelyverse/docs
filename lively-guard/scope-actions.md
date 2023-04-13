# Scope Actions

\
**Universe Management Interface (IUniverseManagement)**
-------------------------------------------------------

* **universeUpdateActivityStatus():** update activity status of Universe entity
* **universeUpdateAlterabilityStatus():** update the alterability status of the Universe entity
* **universeUpdateAdmin():** update admin ID of Universe entity who is referred to specific Type or Role entity
* universeUpdateDomainLimit(): update the number of Domain (DApp) entities that can register in the universe entity.
* **universeCheckAdmin():** check admin of Universe entity by account address
* **universeHasFunction():** check Function ID exists in the Universe entity
* **universeHasContext():** check Context ID exists in Universe entity
* **universeHasRealm():** check Realm ID exists in the Universe entity
* **universeHasDomain():** check Domain ID exists in the Universe entity
* **universeGetDomains():** get registered domains ID from universe entity
* **universeGetInfo():** get universe entity information

Domain Management Interface (IDomainManagement)\



* **domainRegister():** register new Domains (DApp) entity in the Universe entity
* **domainUpdateActivityStatus():** update the activity status of the Domain entity
* **domainUpdateAlterabilityStatus():** update the alterability status of the Domain entity
* **domainUpdateAdmin():** update admin of Domain entity who is referred to specific Type or Role entity
* **domainMoveRealm():** move the Realm entity to another Context entity. A successful move occurs if the Realm entity hasn’t been referred by any agent
* **domainUpdateRealmLimit():** update the number of Realm (Service) entities that can register in the Domain entity.
* **domainRemove():** the Domain entity will be removed according to these conditions, firstly, it mustn't have any Realm entity, secondly, if it is referred by any Agent entity, the Domain entity will be removed softly, and also if it isn't referred by any Agent entity, the Domain entity will be removed from blockchain node (storage)
* **domainCheckId():** check Domain entity exists by ID
* **domainCheckName():** check Domain entity exists by Name
* **domainCheckAdmin():** check Domain entity admin by account address
* **domainHasFunction():** check Function ID exists in the Domain entity
* **domainasContext():** check Context ID exists in the Domain entity
* **domainHasRealm():** check Realm ID exists in the Domain entity
* **domainGetRealms():** get whole realms IDs in the Domain entity
* **domainGetInfo():** get Domain entity information

## Realm Management Interface (IRealmManagement

\


* **realmRegister():** register new Realms (Service) entity in the Domain entity
* **realmUpdateAdmin():** update admin of Realm entity who is referred to specific Type or Role entity
* **realmMoveContext():** move the Context entity to another Realm entity. A successful move occurs if the Context entity hasn’t been referred by any agent.
* **realmUpdateActivityStatus():** update activity status of Realm entity
* **realmUpdateAlterabilityStatus():** update the alterability status of Realm entity.
* **realmUpdateContextLimit():** update the number of Context (Contract) entities that can register in the Realm entity.
* **realmRemove():** the Realm entity will be removed according to these conditions, firstly, it mustn't have any Context entity, secondly, if it is referred by any Agent entity, the Realm entity will be removed softly, and also if it isn't referred by any Agent entity, the Realm entity will be removed from blockchain node (storage)
* **realmCheckId():** check Realm entity exists by ID
* **realmCheckName():** check Realm entity exists by Name
* **realmCheckAdmin():** check admin of Realm entity by account address
* **realmHasFunction():** check Function ID exists in the Realm entity
* **realmHasContext():** check Context ID exists in Realm entity
* **realmGetContexts():** get whole contexts IDs in Realm entity
* **realmGetInfo():** get Realm entity information\
  \
