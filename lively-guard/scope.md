---
description: >-
  Scope is the operational zone that corresponds to system functionality
  entities. It includes Universe, Domain, Realm, Context, and Function entities.
---

# Scope

## **Universe**

Universe is a scope type entity. The Lively Guard defines only one universe entity by default. It base scope of all other fundamental Types and Roles. It also includes all Domain (DApp) entities that will be defined in the ACL.

Universe can include the maximum number of 2^16 Domain (Dapp) entities. It also has some attributes such as unique name, ID, admin ID, activity status, and alterability status.

## Domain (DApp):

Domain is a scope type entity that logically corresponds to Dapp which includes smart contracts and services. When the ACL of Dapp is assigned to Lively Guard, a Domain entity must be created that is equivalent to Dapp.

Each Domain entity can include a maximum number of 2^16 Realm (Service) entities. It also has some attributes such as a unique name, ID, admin ID, activity status, and alterability status.

## Realm (Service)

Realm is a scope type entity that logically corresponds to the service of Dapp which includes smart contracts. When ACL of Service is assigned to Lively Guard, a Realm entity must be created that is equivalent to Dapp’s Service.

Each Realm could have a maximum number of 2^32 Context entities. It also has some attributes such as unique name, ID, admin ID, activity status, and alterability status.

## Context (Smart Contract)

Context is a scope type entity that logically corresponds to Smart Contracts of Dapp which includes functions. When ACL of Smart Contract would be assigned to Lively Guard, a Context entity must be created that is equivalent to Smart Contract of Dapp

Each context entity has a unique address which is equivalent to deployed smart contract address and could have 256 Function entities. It also has some attributes such as name, ID, admin ID, activity status, and alterability status.

## Function

Function is a scope type entity that logically corresponds to the function of a Smart Contract. When the ACL of the Smart Contract function is assigned to Lively Guard, a Function entity must be created that is equivalent to the function of the Smart Contract.

Each Function entity has an Agent ID which allows a specific Type or Role can call it. It has a unique selector ID which equals the function selector in the smart contract and also has some attributes such as name, ID, admin ID, activity status, alterability status, and policy code which is related to ACL policy management.
