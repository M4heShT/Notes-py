
functions ---> a block of  reusable code 
	    place  ( ) after the function name to invoke it

return ----> statement used to end a function and send 
			results back to the caller

--------- EXAMPLE 1 --------- 
`def display_invoice(username, amount, due_date):   <------ here we use positional                                                   arguments if we change position of                                               arguments the  value changes accordingly`
    `print(f"Hello {username}")` 
    `print(f"Your bill of ${amount:.2f} is due: {due_date}")` 
`display_invoice("BroCode", 42.50, "01/02")` 
`display_invoice("JoeSchmo", 100.99, "02/03")`

--------- EXAMPLE 2 ---------
`def create_name(first, last):` 
	`first = first.capitalize()` 
	`last = last.capitalize()`
	 `return first + " " + last` 
`full_name = create_name("spongebob", "squarepants")`
`print(full_name)`














