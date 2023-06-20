
<h2> Classes </h2>

1. In C#, classes are the fundamental building blocks of object-oriented programming, 
encapsulating data and behavior. They define the structure and behavior of objects, 
allowing you to create and manipulate instances of those objects in your program.

2. Classes in C# provide a blueprint for creating objects with shared characteristics and behaviors, 
allowing for code reusability and modular design. They encapsulate data through properties and define methods to perform operations,
enabling developers to organize and manage complex code structures efficiently.


<h2>Constructors</h2>
in C# are special methods within a class that are automatically invoked when an instance of the class is created. 
They initialize the object's state by assigning initial values to its fields or properties, 
allowing for proper object initialization. 
Constructors can be overloaded, providing flexibility to create objects with different sets of initial values or configurations.


<h2>Properties</h2>



<p>Properties in C# provide a way to encapsulate fields within a class and control their access and modification. 
They allow for the definition of getter and setter methods, which enable the retrieval and assignment of values to the underlying fields.
Properties provide a level of abstraction and help maintain the integrity of the object's state by enforcing validation and business logic.
They can also be used to expose read-only or write-only access to data, depending on the requirements of the class.</p>

<hr>


<h3>Static Constructor</h3>
A constructor declared using static modifier is a static constructor.
A static constructor is use to initialize static data or to perform a particular action that need to be performed only once in life cycle of class. 
Static constructor is first block of code to execute in class. Static constructor executes one and only one time in life cycle of class. It is called automatically.
Static constructor does not take any parameters. It has no access specifiers. It is not called directly.

<h3>Instance Constructor</h3>
Instance constructor is used to initialize instance data. Instance constructor is called every time when object of class is created. It is called explicitly.
Instance constructor takes parameters. It has access specifiers.


<hr>

<h2>Stack and Heap</h2>
Understanding both the stack and the heap allows for rethinking previous projects to achieve more efficient memory usage.
Strategies such as optimizing stack allocation, minimizing object creation,
utilizing value types, properly releasing resources, managing object lifecycles, 
using memory-efficient data structures,
and implementing lazy loading can significantly optimize memory utilization.

By considering these approaches, projects can effectively reduce memory allocations, utilize stack memory where appropriate, optimize overall memory management, and reduce potential memory leaks. Timely deallocation of objects, proper resource disposal, and selection of memory-efficient data structures help in reducing memory consumption.

Incorporating memory profiling tools enables the identification of memory-intensive areas, large allocations, and potential memory leaks. By addressing these issues, projects can further improve memory efficiency and overall application performance.
