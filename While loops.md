While = executes some code while some conditions remains True

Ex: while python code

`name = input("Enter Ur Name: ")`

`while name = "" :`
       `print("you didn't type Ur name")`     
       `name = input("Enter Ur Name: ") <---- this line of code ensures`that
                                 `while loop didn'tstruck in infinity loop`      
  `print("Hello, {name}")  <----- here, we exit the while loop` 
	                        `while the condition not True`



Ex: compound interest calculator  
  
`principle = 0  -----> amount u bought` 
`rate = 0   -----> interest rate` 
`time = 0  ----> for how many years` 
  
`while principle <=0 :`  
    `principle = float(input("Enter the Principle Amount: "))`  
    `if principle <=0 :`  
        `print("Principle Amount can't be less than or equal to zero!")`  
  
`while rate <=0 :`  
    `rate = float(input("Enter the Interest Rate: "))`  
    `if rate <=0 :`  
        `print("Interest Rate can't be less than or equal to zero!")`  
  
`while time <=0 :`  
    `time = int(input("Enter the Time in years: "))`  
    `if time <=0 :`  
        `print("Time can't be less than or equal to zero!")`  
  
`total = principle * pow((1 + rate/100 ),time)`  
`print(f"Balance after {time} years: ${total:.2f} ")`


compound interest formula ----> principle * pow((1 + rate/100 ),time)   

reference : [[Python loops]]