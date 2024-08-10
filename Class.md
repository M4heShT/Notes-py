**Object** ---> A bundle of related attributes(variables) and methods(functions)

you need a Class to create many objects

[[Class]] ----> (blueprint) used to design the structure and layout of an object

Ex:   creating the car(object)
`class Car:`    `<---- class object`
	`def __init__(self, model, year, color, for_sale):`  `<---- constructor`
		`self.model = model`
		 `self.year = year`
		  `self.color = color` 
		  `self.for_sale = for_sale` 
	`def drive(self):`  `<-----class methods(functions)`
		`print("You drive the car")'`
		 `print(f"You drive the {self.model}")`
		  `print(f"You drive the {self.color}{self.model}")`
	 `def stop(self):` 
		 `print("You stop the car")`
		  `print(f"You stop the {self.model}")` 
		  `print(f"You stop the {self.color} {self.model}")` 
	`def describe(self):`
		 `print(f"{self.year} {self.color} {self.model}")` 

`car1 = Car("Mustang", 2024, "red", False)`
`car2 = Car("Corvette", 2025, "blue", True)` 
`car3 = Car("Charger", 2026, "yellow", True)`

`print(car1.model)` 
`print(car1.year)`
`print(car1.color)` 
`print(car1.for_sale)` 

`car1.drive()` 
`car1.stop()` 
`car3.describe()`

##### Class variables & Instance variables
*Class variables = Shared among all instances of a class 
Defined outside the constructor 
Allow you to share data among all objects created from that class

*Instance variables = used only in instances of a class 
Defined inside the constructor 
in instance variable, each object has its own version with class variable

Ex:
`class Student:` 
	`class_year = 2025` `<------class variable`
	`num_students = 0`
	
	`def __init__(self, name, age):`
		 `self.name = name`  <----- instance variables
		 `self.age = age` 
		 `Student.num_students += 1`
		 
`student1 = Student("Spongebob", 30)` 
`student2 = Student("Patrick", 35)` 
`student3 = Student("Squidward", 55)` 
`student4 = Student("Sandy", 27)`

`print(f"My graduating class of {Student.class_year} has {Student.num_students} students")` 
`print(student1.name)`
`print(student2.name)`
`print(student3.name)` 
`print(student4.name)`