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

\
