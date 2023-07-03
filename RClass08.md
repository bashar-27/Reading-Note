<h1>Collections And Enums</h1>

<hr>

<h2>1. Collections</h2>
<p>Specialized classes for storing and retrieving data are known as collection classes.
  These classes are designed to handle stacks, queues, lists, and hash tables. They typically implement common interfaces.

The primary functions of collection classes include dynamically allocating memory for elements and facilitating access to items based on their index. 
These classes allow for the creation of collections comprising objects derived from the Object class, which serves as the base class for all data types in C#.</p>

<h3>Kinds of Collections</h3>
Many common collections are provided by .NET. Each type of collection is designed for a specific purpose.

Some of the common collection classes are described in this section:

* System.Collections.Generic classes

* System.Collections.Concurrent classes

* System.Collections classes

  <hr>

  <h2>2. Enums</h2>
  <p>An enumeration is a collection of named integer constants. It is defined using the "enum" keyword.

    In C#, enumerations are value types, meaning they hold their own values and cannot inherit or be inherited from.

    To declare an enumeration, you use the following syntax:
  <code>
  enum <enum_name>
{
   // Enumeration list
}</code>


Example:
   <code>enum Colors { Red, Green, Blue, Yellow };
</code> 
In this example, the "Colors" enumeration consists of four symbols: "Red", "Green", "Blue", and "Yellow". By default, the value of "Red" is 0, "Green" is 1, "Blue" is 2, and "Yellow" is 3.

You can use this enumeration to represent different colors in your program. For example, you can declare a variable of type "Colors" and assign one of the enumerated values to it:
<code> Colors selectedColor = Colors.Blue;
 </code>

 In this case, the variable "selectedColor" is assigned the value "Blue" from the "Colors" enumeration.

 <h3>The System.Enum type and enum constraint</h3>
The System.Enum type is the abstract base class of all enumeration types. It provides a number of methods to get information about an enumeration type and its values.
For more information and examples, see the System.Enum API reference page.

You can use System.Enum in a base class constraint (that is known as the enum constraint) to specify that a type parameter is an enumeration type.
Any enumeration type also satisfies the struct constraint, which is used to specify that a type parameter is a non-nullable value type.
</p>
