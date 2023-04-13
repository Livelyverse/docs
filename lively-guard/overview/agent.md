---
description: >-
  Agent is the subject who can make actions in Scope. It contains Type
  (Department), Role, and Member entities.
---

# Agent

## Type (Department)

Type is an agent type entity that logically corresponds to the department in an organization or corporation. When the ACL of the organization department is assigned to Lively Guard, a Type entity must be created that is equivalent to it.

Each Type entity can have a maximum 2^16 number of Role entities.

It also has some attributes such as ID, a unique name, admin ID, activity status, alterability status, and Scope ID which defines its operation zone.

## Role

Role is an agent type entity that logically corresponds to the organization department role which contains members. When a department role is assigned to Lively Guard, a Role entity must be created that is equivalent to it.

Each Role entity can have a maximum 2^24 number of Member entities.

It also has some attributes such as ID, a unique name, admin ID, activity status, alterability status, and Scope ID which defines its operation zone

## Member

Member is an agent type entity that logically corresponds to the department role member or smart contract. When a member of a role is assigned to Lively Guard, a Member entity must be created that is equivalent to it. Member entity has a unique role in each department (type) and also, and they can have different roles in different departments.

Each Member entity can join to a maximum 2^16 Type entity and also it has a unique address that is equivalent to EOA or smart contract address. It also has some attributes such as ID, name, admin ID, limits, activity status, and alterability status.
