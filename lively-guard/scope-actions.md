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



* domainRegister(): register new Domains (DApp) entity in the Universe entity
* domainUpdateActivityStatus(): update the activity status of the Domain entity
* domainUpdateAlterabilityStatus(): update the alterability status of the Domain entity
* domainUpdateAdmin(): update admin of Domain entity who is referred to specific Type or Role entity
* domainMoveRealm(): move the Realm entity to another Context entity. A successful move occurs if the Realm entity hasn’t been referred by any agent
