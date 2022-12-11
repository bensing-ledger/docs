# How The Bensing Ledger Works

This documentation is language-agnostic design for the ledger.  This ledger is a mechanism manage fund transfers between parties in a marketplace scenario.  The ledger tracks the deposit of cash, transfers of cash between marketplace participants, and the withdrawal of fund.

## Use Cases

- Deposit Funds
- Send Funds
- Withdraw Funds

Examples of how these use cases look in a ledger can be found at [Bensing Ledger - Example](https://docs.google.com/spreadsheets/d/1G1NLvnJIlmE6_xCFI6UCidd1r7ob65sbjNE-bZrV_-I/edit?usp=sharing)

### 1.0 Deposit Funds

A user deposits funds from an outside cash source into the ledger

#### 1.1.0 - Deposit Into Wallet

A user deposits funds from an outside cash source into their corresponding wallet within the ledger.  The wallet is a liability account associated to one, and only one, user.

Definitions

* **Cash Account** - The place where all cash funds are tracked for the ledger.
* **Wallet Account** - The place where we track all the money a user can use. 
  * It is a liability account linked to one, and only one user. 

##### Primary Path

Required Input Data

* User Account
* Quantity of Money Deposit
* Currency Type of Money

System Generated Data

* Ledger Transaction Identifier

Sequence

1) A debit is recorded in the ledgers cash account
2) A credit is recorded in the users wallet account

##### Secondary Paths (TODO)

###### Deposit Money is equal-to or less than zero (0). (TODO)

###### Deposit currency is not the same currency as the Users wallet. (TODO)


---


### 2.0 Transfer Funds (TODO)

#### 2.1.0 - Transfer Between Wallets (TODO)


___


### 3.0 Withdraw Funds (TODO)

#### 3.1.0 - Withdraw Funds from Wallet (TODO)

---

