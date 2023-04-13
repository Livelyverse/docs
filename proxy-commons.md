---
description: It’s common interface of proxy used in all contracts.
---

# Proxy Commons

## Proxy Interface (IProxy)

* **upgradeTo():** Upgrade the implementation of the proxy
* **setSafeModeStatus():** Update the safe mode status of the proxy
* **setUpdatabilityStatus():** Set the update ability status of the proxy
* **setLocalAdmin():** Update the local administration address of the proxy
* **setAccessControlManager():** Update the ACL address of the proxy
* **withdrawBalance():** Withdraw the whole amount of the balance of the proxy
* **contractName():** Get the contract name of the proxy
* **contractVersion():** Get the contract version of the proxy
* **accessControlManager():** Get the ACL address of the proxy
* **subjectAddress():** Get the implementation contract address of the proxy
* **safeModeStatus():** Get the safe mode status of the proxy
* **updatabilityStatus():** Get the update ability status of the proxy
* **localAdmin():** Get the local administrator address of the proxy
* **domainSeparator():** Returns the domain separator used in the encoding of the signature, as defined by EIP712
* **initVersion():** Get the initialized version of the proxy

\


\
