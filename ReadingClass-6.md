<h1>C# Inheritance</h1>

In C#, inheritance is a process in which one object acquires all the properties and behaviors of its parent object automatically. In such way, you can reuse, extend or modify the attributes and behaviors which is defined in other class.

In C#, the class which inherits the members of another class is called derived class and the class whose members are inherited is called base class. The derived class is the specialized class for the base class.

<hr>

<h1>C# Abstract</h1>
Abstract classes are the way to achieve abstraction in C#. Abstraction in C# is the process to hide the internal details and showing functionality only. Abstraction can be achieved by two ways:

1- Abstract class

2- Interface

 Abstract Method: A method that is declared abstract, has no “body” and is declared inside the abstract class only.
 An abstract method must be implemented in all non-abstract classes using the override keyword. After overriding, the abstract method is in the non-Abstract class.
 We can derive this class in another class, and again we can override the same abstract method with it.

 Abstract Class: This is the way to achieve the abstraction in C#. An Abstract class is never intended to be instantiated directly.
 An abstract class can also be created without any abstract methods, We can mark a class abstract even if doesn’t have any abstract method.
 The Abstract classes are typically used to define a base class in the class hierarchy. Or in other words, an abstract class is an incomplete class or a special class we can’t be instantiated.
 The purpose of an abstract class is to provide a blueprint for derived classes and set some rules that the derived classes must implement when they inherit an abstract class.
 We can use an abstract class as a base class and all derived classes must implement abstract definitions. 
 
 <hr>

<h1>Polymorphism</h1> In C# allows objects of derived classes to be treated as objects of the base class, providing flexibility and code reusability. 
It involves runtime polymorphism, where the appropriate method implementation is determined based on the actual type of the object. 
Method overriding through virtual methods enables derived classes to provide their own implementation while still adhering to the base class contract. 

- Method overriding is used to provide a new implementation of a method in a derived class, replacing the inherited implementation from the base class.
  
- Method overloading is used to create multiple methods with the same name but different parameters within a class, enabling different ways of invoking the method based on the input arguments.
