[[ Inheritance]] = allow a class to Inherit attributes and methods from another class 
Helps with code reusability and extensibility 
class Child(Parent)

   multiple inheritance = inherit from more than one parent class  C(A,B)

   multilevel inheritance = inherit from a parent which inherits from another parent
    C(B) <--  B(A) <-- A

Ex 1: showing inheritance in animal hierarchy
`class Animal:`     `<--------- Parent class`
	`def __init__(self, name):` 
		`self.name = name`
		 `self.is_alive = True`
		 
	`def eat(self):`
		`print(f"{self.name} is eating")
		
	def sleep(self):
	 print(f"{self.name} is asleep") 
`class Dog(Animal):`     `<-------- here dog class gets inherited from Animal class`
	`def speak(self):` 
		`print("WOOF!")` 
`class Cat(Animal):`      `<--------- child class`
	`def speak(self):` 
		`print("MEOW!")`
 `class Mouse(Animal):`
	  `def speak(self):` 
		  `print("SQUEEK!")` 

`dog = Dog("Scooby")` 
`cat = Cat("Garfield")`
`mouse = Mouse("Mickey")`

Ex2: Multiple Inheritance

`class Prey:    <------- parent class`
	`def flee(self):` 
		`print("The animal is fleeing")` 
	
`class Predator:`
	`def hunt(self):` 
		`print("The animal is hunting")` 

`class Rabbit(Prey):  <----- child class`
	`pass` 
`class Hawk(Predator):` 
	`pass`
`class Fish(Prey, Predator):` 
	`pass`

`rabbit.flee()` 
`hawk.hunt()` 
`fish.flee()    <------fish inherited from both prey and predator class (multiple inheritancee)`
`fish.hunt()`

Ex 3  : Multi-level Inheritance

`class Animal:           <---------- Parent class`
	`def __init__(self, name):` 
		`self.name = name`
		
	``def eat(self):``
		 ``print(f"{self.name} is eating")`` 
		 
	``def sleep(self):`` 
		``print(f"{self.name} is sleeping")`` 
		
`class Prey(Animal):    <------ child1 class (Also a parent class to rabbit)`
	`def flee(self):` 
		`print(f"{self.name} is fleeing")` 
	
`class Predator(Animal):`
	`def hunt(self):` 
		`print(f"{self.name} is hunting")` 

`class Rabbit(Prey):  <------- child2 class (it inherits from animal and prey)`
	`pass` 
`class Hawk(Predator):` 
	`pass`
`class Fish(Prey, Predator):` 
	`pass`

`rabbit = Rabbit("Bugs")` 
`hawk = Hawk("Tony")` 
`fish = Fish("Nemo")`