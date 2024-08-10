OOP's -----> Object Oriented Programming
object ---> A bundle of related attributes(variables) and methods(functions)

you need a [[Class]] to create many objects

[[Class]] ----> (blueprint) used to design the structure and layout of an object

In this we have, 1)Inheritance 2)Encapsulation 3)Polymorphism 4)Abstraction 

class variables = Shared among all instances of a class 
Defined outside the constructor 
Allow you to share data among all objects created from that class

Instance variables = used only in instances of a class 
Defined inside the constructor 
in instance variable, each object has its own version with class variable

[[ Inheritance]] = allow a class to Inherit attributes and methods from another class 
Helps with code reusability and extensibility 
class Child(Parent)

   multiple inheritance = inherit from more than one parent class  C(A,B)

   multilevel inheritance = inherit from a parent which inherits from another parent
    C(B) <--  B(A) <-- A
    


[[Abstract class]]: A class that cannot be instantiated on its own; Meant to be subclassed. 
They can contain abstract methods, which are declared but have no implementation. 
Abstract classes(Abstraction) benefits: 
1. Prevents instantiation of the class itself 
2. Requires children to use inherited abstract methods

[[super() ]]= Function used in a child class to call methods from a parent class (superclass).
Allows you to extend the functionality of the inherited methods


[[Polymorphism ]]= Greek word that means to "have many forms or faces" 
Poly = Many 
Morphe = Form 

TWO WAYS TO ACHIEVE POLYMORPHISM 
1. Inheritance = An object could be treated of the same type as a parent class 
2. "Duck typing" = Object must have necessary attributes/methods


   "*Duck typing"* = Another way to achieve polymorphism besides Inheritance 
   Object must have the minimum necessary attributes/methods
    "If it looks like a duck and quacks like a duck, it must be a duck."

[[Aggregation]] = Represents a relationship where one object (the whole) contains references to one or more INDEPENDENT objects (the parts)

Aggregation = A relationship where one object contains references to other INDEPENDENT objects "has-a" relationship

[[Composition ]]= The composed object directly owns its components, which cannot exist independently "owns-a" relationship

[[Nested class ]]= A class defined within another class 
class Outer:  
	class Inner: 
Benefits: Allows you to logically group classes that are closely related 
Encapsulates private details that aren't relevant outside of the outer class
Keeps the namespace clean; reduces the possibility of naming conflicts

[[@Static methods]] = A method that belong to a class rather than any object from that class (instance) Usually used for general utility functions
Instance methods - Best for operations on instances of the class (objects)
Static methods - Best for utility functions that do not need access to class data

[[@Class methods]] = Allow operations related to the class itself Take (cls) as the first parameter, which represents the class itself. 
Instance methods = Best for operations on instances of the class (objects)
Static methods = Best for utility functions that do not need access to class data 
Class methods = Best for class-level data or require access to the class itself

[[__Magic methods__ ]]= Dunder methods (double underscore) __init__, __str__, __eq__ 
They are automatically called by many of Python's built-in operations
 They allow developers to define or customize the behavior of objects

[[@property]] = Decorator used to define a method as a property (it can be accessed like an attribute)
Benefit: Add additional logic when read, write, or delete attributes 
Gives you getter, setter, and deleter method


[[@Decorator ]]= A function that extends the behavior of another function w/o modifying the base function
Pass the base function as an argument to the decorator