for = execute a block of code for fixed no. of times and can iterate over range, strings, sequences, etc. 

Ex: simple for loop

`n = int(input("enter the value:))`

`for i in range(1,n):`
     `i += 1`
     `print("i")`


ex: countdown timer program

`import time`  
  
`my_time = int(input("Enter the time in seconds:"))`  
  
`for t in range(my_time,0,-1):`  
    `seconds = t % 60`  
    `minutes = int(t/60) %60`  
    `hours = int(t/3600)`  
    `print(f"{hours}:{minutes:02}:{seconds:02}")`  
    `time.sleep(1)`  
`print("Time's up kiddos just fuck up & sleep!")`



reference : [[Python loops]]
