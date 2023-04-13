---
description: >-
  Policy is an operational access level that applies over Role entities and it
  is related to one of the scope entities.
---

# Policy

Policy is an ACL entity that limits the Role entity access level on the specific Scope. the Lively Guard will check the Role entity access level on the function call used by the policy code that is defined in the Policy entity and Function entity if the Role entity has included in the Policy entity and also Function entity must be a subset of the scope reference of it.

Each Policy entity can have a maximum 2^16 number of Role entities.

It also has some attributes such as a scope Id which shows the scope referred by it, unique name, ID, admin ID, activity status, alterability status, and policy code, Policy code is a number between 0 to 255 and these codes will be described as below:

**0:** (Unlock) Role can do any actions in referred scopes

**1-63:** (Soft Lock) Role can do soft limitations actions in referred scopes

**64-127:** (Medium lock) Limitations and accesses are at the medium level in referred scopes

**128-191:** (Restrict Lock) Limitations and accesses are at the restricted level in referred scopes

**192-254:** (Hard Lock) Limitations and accesses to do any actions are very low in referred scopes

**255:** (Lock) Limitations are at maximum level and the role can’t do any action in referred scopes
