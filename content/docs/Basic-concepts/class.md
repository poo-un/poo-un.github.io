---
linkTitle: "Classes"
title: Class concept
weight: 1
---

A class is a user-defined data type. It consists of data members and member functions, which can be accessed and used by creating an instance of that class. It represents the set of properties or methods that are common to all objects of one type. A class is like a blueprint for an object. \
Imagine we have a <font color="#007bff">Class</font> called <font color="#007bff">`GameCharacter`</font>. Within the vast world of gaming, there can be a multitude of different characters, each with unique names, appearances, and abilities.\
However, despite their individuality, they often share certain common characteristics and behaviors that define what it means to be a <font color="#007bff">`GameCharacter`</font>. In this scenario, <font color="#007bff">`GameCharacter`</font> is the <font color="#007bff">Class</font>, and the shared <font color="#FFA600">attributes</font> and behaviors are its properties. These properties could include fundamental aspects such as <font color="#FFA600">`Health Points`</font>, <font color="#FFA600">`Attack Power`</font>, <font color="#FFA600">`Movement Speed`</font>, and <font color="#FFA600">`Special Abilities`</font>. \
Regardless of whether a <font color="#007bff">`GameCharacter`</font> is a heroic knight, a cunning rogue, or a powerful wizard, they all possess these core properties

Methods such as <font color="#FF75A0">`attack()`</font>, <font color="#FF75A0">`defend()`</font>, and <font color="#FF75A0">`move()`</font> allow <font color="#007bff">`GameCharacters`</font> to interact dynamically with the game world, performing offensive, defensive, and movement actions respectively.

|ㅤㅤㅤㅤㅤ<font color="#007bff">GameCharacter</font>ㅤㅤㅤㅤㅤ|
|:--:|
|<font color="#FFA600">int</font> healthPoints <br/> <font color="#FFA600">int</font> attackPower <br/> <font color="#FFA600">int</font> movementSpeed|
| + <font color="#FF75A0">attack</font>( ) <br/> + <font color="#FF75A0">defend</font>( ) <br/> + <font color="#FF75A0">move</font>( )|


Let's explain this concept with an example:

## Bank Account Class

Let's consider the concept of a class using the example of a `BankAccount`.

A <font color="#007bff">class</font> is like a blueprint or template for creating objects. In our example, the <font color="#007bff">`BankAccount`</font> class represents the blueprint for creating individual bank account objects.

- **Attributes**:
  - <font color="#FFA600">Attributes</font> are characteristics or properties that describe the objects created from the class. For instance, in the case of a <font color="#007bff">`BankAccount`</font>, attributes could include <font color="#FFA600">`account_number`</font>, <font color="#FFA600">`balance`</font>, and <font color="#FFA600">`account_holder`</font>.

- **Methods**:
  - <font color="#F2613F">Methods</font> are functions that define the behavior of the objects created from the class. In the context of a <font color="#007bff">`BankAccount`</font>, methods could include operations like <font color="#F2613F">`deposit`</font> and <font color="#F2613F">`withdraw`</font>, which specify how money can be added to or withdrawn from an account.

|ㅤㅤㅤㅤㅤ<font color="#007bff">BankAccount</font>ㅤㅤㅤㅤㅤ|
|:--:|
| <font color="#FFA600">int</font> account_number <br/> <font color="#FFA600">int</font> balance <br/> <font color="#FFA600">string</font> account_holder |
| + <font color="#F2613F">deposit</font>(amount) <br/> + <font color="#F2613F">withdraw</font>(amount) |


This <font color="#007bff">class</font> blueprint, highlighted in <font color="#007bff">blue</font>, defines the structure for creating <font color="#007bff">`BankAccount`</font> objects. Each object instantiated from this class inherits <font color="#FFA600">attributes</font> styled in <font color="#FFA600">yellow</font>, such as <font color="#FFA600">`account number`</font>, <font color="#FFA600">`balance`</font>, and <font color="#FFA600">`account holder`</font>. Additionally, the <font color="#F2613F">methods</font> highlighted in <font color="#F2613F">red</font>, such as <font color="#F2613F">`deposit()`</font> and <font color="#F2613F">`withdraw()`</font>, enable the objects to perform operations like adding or withdrawing money. 