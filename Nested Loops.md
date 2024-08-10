nested loop = a loop within another loop(outer loop ,inner loop )
				outer loop:
				      inner loop:

Ex: printing patterns (right triangle)

`num = int(input("Enter the no. of rows: "))`  
  
`for i in range(1,num+1):`  
    `for j in range(1,i+1):`  
        `print("$",end = " ")`  
    `print()`

ex : reverse right triangle
`num = int(input("Enter the no. of rows: "))`  
`for i in range(num+1,0,-1):`  
    `for j in range(i-1,0,-1):`  
        `print("*",end = " ")`  
    `print()`

Reference : [[Python loops]]  [[For loops]] [[While loops]]