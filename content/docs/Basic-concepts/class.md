---
linkTitle: "Class"
title: Class concept
weight: 1
---

A class is a user-defined data type. It consists of data members and member functions, which can be accessed and used by creating an instance of that class. It represents the set of properties or methods that are common to all objects of one type. A class is like a blueprint for an object. \
Imagine we have a Class called "GameCharacter." Within the vast world of gaming, there can be a multitude of different characters, each with unique names, appearances, and abilities.\
However, despite their individuality, they often share certain common characteristics and behaviors that define what it means to be a "GameCharacter."In this scenario, "GameCharacter" is the Class, and the shared attributes and behaviors are its properties. These properties could include fundamental aspects such as "Health Points," "Attack Power," "Movement Speed," and "Special Abilities." \
Regardless of whether a GameCharacter is a heroic knight, a cunning rogue, or a powerful wizard, they all possess these core properties



|ㅤㅤㅤㅤㅤGameCharacterㅤㅤㅤㅤㅤ |
|:--:|
|int  healthPoints <br/> int attackPower <br/> int movementSpeed  |
| + attack( ) <br/> +defend( ) <br/> +move( ) |

### Example: Bank Account Class

Let's consider the concept of a class using the example of a `BankAccount`.

#### Class Concept:

A class is like a blueprint or template for creating objects. In our example, the `BankAccount` class represents the blueprint for creating individual bank account objects.

- **Attributes**:
  - Attributes are characteristics or properties that describe the objects created from the class. For instance, in the case of a bank account, attributes could include `account_number`, `balance`, and `account_holder`.

- **Methods**:
  - Methods are functions that define the behavior of the objects created from the class. In the context of a bank account, methods could include operations like `deposit` and `withdraw`, which specify how money can be added to or withdrawn from an account.

### Bank Account Class:

Imagine we have a `BankAccount` class. This class doesn't represent a specific bank account; rather, it outlines what attributes and methods bank account objects will have.

For instance, the `BankAccount` class may have:
- Attributes such as `account_number`, `balance`, and `account_holder`.
- Methods such as `deposit` and `withdraw` to perform actions on a bank account.

This class acts as a blueprint for creating individual bank account objects. Each bank account object created from this class will have its own unique set of attributes (e.g., account number, balance) and can perform operations defined by the methods (e.g., depositing or withdrawing money).

