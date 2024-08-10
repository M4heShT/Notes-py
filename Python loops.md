In python there are different kinds of Loops available but most familiar are 
[[While loops]]  and  [[For loops]]  both are used for different purposes 

ex : reverse right triangle
`num = int(input("Enter the no. of rows: "))`  
`for i in range(num+1,0,-1):`  
    `for j in range(i-1,0,-1):`  
        `print("*",end = " ")`  
    `print()`
    
Ex: simple for loop

`n = int(input("enter the value:))`

`for i in range(1,n):`
     `i += 1`
     `print("i")`