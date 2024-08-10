if  = do some code which executes if the condition is True 
     else = execute the different code which may be the condition false 
elif = if more than two condition is there int he function then elif comes into play 
it is also called control flow statements


Ex:  age program 

`age = int(input("Enter your age (>0):"))`

`if age <= 0 :`
    `print("Age not valid should be greater than 0")`
`else :`
    `print("You are {age} years old!")`


Ex: weight calculator program
`weight = float(input("Enter your weight : "))`  
`unit = input("Kilograms or Pounds? (K or L) : ")`

`if unit == "K":`  
    `weight = weight * 2.205`  
    `unit = 'Lbs.'`  
    `print(f"your weight is : {weight} {unit}")`  
`elif unit == "L":`  
     `weight = weight / 2.205`  
    `unit = 'Kgs'`  
    `print(f"Your weight is : {weight} {unit}")`  
 `else:`  
    `print(f'{unit} is not valid!')`


Ex: temperature calculator program

`temp = float(input("Enter your Temperature: "))`
`unit = input("Enter the Temperature in Celcius or Fahrenheit (C/F) : ")`

`if unit == "C":`
	`temp = (9 * temp/5 + 32)`
	 `print(f"Ur Temp in Fahrenheit is :{temp}^F")`
`elif  unit == "F":`
	`temp = ((temp-32)*5/9)`
	 `print(f"Ur Temp in Fahrenheit is :{temp}^C")`
`else:`  
    `print(f'{unit} is not valid measurement!')`



