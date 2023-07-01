<h2>C# Interface</h2>

Interface in C# is a blueprint of a class. It is like abstract class because all the methods which are declared inside the interface are abstract methods. It cannot have method body and cannot be instantiated.

It is used to achieve multiple inheritance which can't be achieved by class. It is used to achieve fully abstraction because it cannot have method body.

Its implementation must be provided by class or struct. The class or struct which implements the interface, must provide the implementation of all the methods declared inside the interface.



 Note:
Interface members must be implemented with the public modifier; otherwise, the compiler will give compile-time errors.


Modifiers in Interfaces

C# 8.0 allows private, protected, internal, public, virtual, abstract, sealed, static, extern, and partial modifiers in an interface.

The default access level for all interface members is public.
An interface member whose declaration includes a body is a virtual member unless the sealed or private modifier is used.
A private or sealed function member of an interface must have implementation body.
Interfaces may declare static members which can be accessed by interface name.



<h2>Difference between Abstract Class and Interface in C#</h2>


| Abstract Class                                                             | Interface Class                                                                                 |
|----------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|
| The special class which cannot be instantiated is known as abstract class. | The interface enables us to determine the functionality or functions but cannot implement that. |
| Abstract classes have static members.                                      | Interface does not have static members.                                                         |
| They have a constructor.                                                   | They don’t have a constructor.                                                                  |
| Here the performance is fast.                                              | Here the performance is slow.                                                                   |
| It includes methods, fields, constants, etc.                               | It only includes methods .                                                                      |
| Abstract class can be fully, partially or not implemented.                 | Interfaces can be fully implemented.                                                            |

