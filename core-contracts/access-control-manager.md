# Access Control Manager

Generally, the access control manager is considered one of the most important components system, and considering the extent of the Lively ecosystem, we decided to design an access control manager from scratch that can meet Lively needs.

The main idea of this design is based on a centralized structure on the blockchain platform, which is a decentralized and on-chain structure. so we have defined new concepts according to figure 1.

&#x20;

<figure><img src="../.gitbook/assets/lively-token-Page-11.drawio.svg" alt=""><figcaption><p>Lively ACL - figure 1</p></figcaption></figure>

Access Control List Manager (ACLM): it's the main contract to access control in the Lively system. it contains so many functions related to managing members, roles, types, groups, functions, contexts, realms, and domains.

Function: it's a basic element in ACLM that contains a function selector, status, and only a reference to one of Role, Type, and Group.

Context: it has a unique id in ACLM. it contains function selectors, states, and admin role. it's equivalent to a contract that will be registered to ACLM.

Realm: it defines a realm for a set of Contexts with a specific purpose. each Realm doesn't have any limitation to contain Context. it contains also a unique id, an admin role, status and etc.&#x20;

Domain:  it defines a domain for a set of Realms with a specific purpose. each Domain doesn't have any limitation to contain Realm. it contains also a unique id, an admin role, status and etc. ACLM can contain unlimited domains.

Member: it refers to an Account(smart contract address) entity or an EOA(External Of Account) entity.

Role: it contains a set of members with a clear definition of activity in the Lively system that defines in ACLM. it has a unique id that contains scope for reference to one of the functions, contexts, realms, and domains. it contains also security policy. the security policy is similar to the claim that contains some permissions.

Type: it defines a type of role to classify roles. it can contain many roles with different scopes and scopes of roles must conform with it. it has also a unique id and status.

Group: it contains a set of role types. it has a unique id and status. ACLM can contain unlimited groups with different scopes. it contains also many role types with different scopes and scopes of roles must conform with it.
