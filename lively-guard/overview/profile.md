---
description: >-
  Profile is an ACL entity that provides profiles for business owners or
  customers that would like to have authorization service from the Lively Guard.
  It has Scopes, Agents, and Policies sections.
---

# Profile

**Profile** is an ACL entity to provide ACL(authorization) service to business owners or customers. When a customer requests ACL service from the Lively Guard, after the registration process, the Profile entity is created for the customer to keep ACL info.

Each Profile entity contains three sections Scope, Agent, and Policy whose definitions same as those already have been defined except for the Member entity which will be defined in this section. It has also a unique name, ID, admin ID, owner address, registration limits, profile limits,

activity status and alterability status.

## ProfileMember

ProfileMember is an Agent type entity that logically corresponds to the department role member or smart contract. When a member of a role is assigned to a profile, a ProfieMember entity must be created that is equivalent to it. ProfileMember entity has a unique role in each department (type) and also, and they can have different roles in different departments.

Each ProfileMember entity can join to a maximum 2^16 Type entity and also it has a unique address that is equivalent to EOA or smart contract address. It also has some attributes such as ID, name, admin ID, call limit, register limit, activity status, and alterability status.

\
