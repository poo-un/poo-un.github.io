---
linkTitle: "Object"
title: Object concept
weight: 2
---
## Object Concept

In object-oriented programming (OOP), an object is an instance of a class. It represents a real-world entity with its own set of properties (attributes) and behaviors (methods). Objects are the building blocks of OOP and are used to model and interact with the system.

### Example: Bank Account Class

Let's say we have a class called `BankAccount`. This class represents a bank account, and it has methods to perform banking operations like depositing money and withdrawing money.

#### Object Concept:

In our example, an object is an instance of the `BankAccount` class. Each individual bank account created from the `BankAccount` class is an object.

- **Attributes**:
  - Each bank account object has its own set of attributes that describe its specific state. For instance, each bank account object might have attributes like `account_number`, `balance`, and `account_holder`.

- **Methods**:
  - Objects have access to the methods defined by their class. These methods define the behavior or actions that objects can perform. For example, each bank account object can use methods like `deposit` and `withdraw` to manage its funds.

### Example:

Suppose we create two bank account objects from the `BankAccount` class:

1. **Account 1**:
   - `account_number`: 123456
   - `balance`: $500
   - `account_holder`: John Doe

2. **Account 2**:
   - `account_number`: 789012
   - `balance`: $1000
   - `account_holder`: Jane Smith

Each bank account object represents a distinct bank account with its own unique attributes and behaviors. For example, account 1 and account 2 have different account numbers, balances, and account holders. They can each independently use the `deposit` and `withdraw` methods to manage their funds.
