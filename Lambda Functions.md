Lambda function = A small anonymous function for a one time use (throw away function) 
They take any number of arguments, but have only 1 expression 
Helps keep the namespace clean and is useful with higher-order functions : 'sort()', 'map()', 'filter()', 'reduce()'
lambda parameters: expression


Ex:
`double = lambda x :  x * 2`
`add = lambda x ,y : x + y`
`max_value = lambda x, y : x if x > y else y`
`min_value = lambda x, y : x if x < y else y`
`full_name = lambda first, last: first + " "+ last` 
`is_even = lambda x : "odd" if x % 2 == 0 else "even"`
`age_check = lambda age : "Kick-in "if age >= 18 else "Kick-out"`

`print(double(2))`
`print(add(2, 3))`
`print(max_value(6, 5))`
`print(max_value(4, 5))`
`print(age_check(12))`   
`print(is_even(4))`


1) map(function, collection) = Applies a given function to all items in a collection

ex:
`celsius_temps = [0.0, 10.0, 20.0, 30.0, 40.0, 50.0] 
`fahrenheit_temps = list(map(lambda temp: (temp * 9/5) + 32, celsius_temps))

`print(fahrenheit_temps)`


2) filter(condition, collection) = return all elements that pass a condition

ex:

`grades = [91, 32, 83, 54, 72, 63, 47]`

`passing_grades = filter(lambda grade : grade >= 60 , grades)`

`for grade in passing_grades:`
	`print(grade)`


3) reduce(function, collection) = Reduces elements in a collection to a single value 
For loop is better in most cases 
Reduce is better for a functional approach + readability 

ex:
`from functools import reduce` 

`prices = [19.99, 1.00, 5.75, 12.99, 10.99]`
`total = reduce(lambda x, y: x + y, prices)` 

`print(f"${total}")`

4) SORTING IN PYTHON .sort() or sorted() 
Lists[], Tuples(), Dictionaries{"":""}, Objects

ex:
--------- LISTS --------- 
`fruits = ["banana", "orange", "apple", "coconut"]` 

`fruits.sort()` 
`fruits.sort(reverse=True)` 

`print(fruits)`
 
--------- TUPLES ---------
`fruits = ("banana", "orange", "apple", "coconut")` 

`fruits = tuple(sorted(fruits))` 
`fruits = tuple(sorted(fruits, reverse=True))` 

`print(fruits)`

--------- DICTIONARIES --------- 
`fruits = { "banana": 105,`
		`"apple": 72,` 
		`"orange": 73,`
		`"coconut": 354 }`
		
`fruits = dict(sorted(fruits.items()))` 
`fruits = dict(sorted(fruits.items(), key=lambda item: item[0], reverse=True))` 
`fruits = dict(sorted(fruits.items(), key=lambda item: item[1])) fruits = dict(sorted(fruits.items(), key=lambda item: item[1], reverse=True))` 

`print(fruits)`


--------- OBJECTS --------- 
`class Fruit:` 
	`def __init__(self, name, calories):` 
		`self.name = name` 
		`self.calories = calories` 
		
	def __repr__(self):`
		 `return f"{self.name}: {self.calories}"
		 
`fruits = [Fruit("banana", 105),` 
		`Fruit("apple", 72),`
		`Fruit("orange", 73),` 
		`Fruit("coconut", 354)]` 

`fruits = sorted(fruits, key=lambda fruit: fruit.name)`
`fruits = sorted(fruits, key=lambda fruit: fruit.name, reverse=True)` 
`fruits = sorted(fruits, key=lambda fruit: fruit.calories)`
`fruits = sorted(fruits, key=lambda fruit: fruit.calories, reverse=True)` 

`print(fruits)`












ref:[[Functions]]


