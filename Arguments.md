Arguments ----->arguments are values passed to a function when it’s called. Parameters are the variables inside a function’s parentheses, and arguments provide values for those parameters.

1) Positional 
2) Default
3) keyword
4) Arbitrary

1)Positional Arguments-----> arguments are passed in the order they are defined in the function signature.

Ex: fun. prints full name where we use Positional Arguments-
`def create_name(first, last):` 
	`first = first.capitalize()` 
	`last = last.capitalize()`
	 `return first + " " + last` 
`full_name = create_name("spongebob", "squarepants")`
`print(full_name)`



2)Default Argument----> default value for certain parameters, default is used when that argument is omitted and it makes your functions flexible and also reduces the # of arguments

Ex: fun. prints the total price of product we use Default Argument to calculate 
`def net_price(list_price, discount=0, tax=0.05):`
	`return list_price * (1 - discount) * (1 - tax)` 
`print(net_price(500))        <-----here code uses default value as from parameter`
`print(net_price(500, 0.1))` 
`print(net_price(500, 0.1, 0))`



3)keyword argument----> an argument preceded by an identifier that matches the functions identifier helps with readability and the order of arguments doesn't matter

Ex: fun. prints phone num here we use keyword argument as order doesn't matter
`def get_phone(country, area, first, last):`
	`return f"{country}-{area}-{first}-{last}"` 
`phone_num = get_phone(country=1, area=123, last=7890,first=456) <---keyword` 
`print(phone_num)`




4)Arbitrary Argument----> functions to accept an unlimited number of arguments
'*'args - allows you to pass multiple non-keyword arguments. it returns as tuples.
 "**"kwargs** - allows you to to pass multiple keyword arguments. it returns as dictionaries
  * - refers unpacking operator.

Ex:
---- *ARGS Example 1 ---- 
`def add(*nums):` 
    `total = 0` 
    `for num in nums:` 
        `total += num`
    `return total` 
`print(add(1, 2, 3, 4))` 

---- *ARGS Example 2 ----
`def display_name(*args):`
	`print(f"Hello", end=" ")` 
	`for arg in args:`
	    `print(arg, end=" ")` 
`display_name("Dr.", "Spongebob", "Harold", "Squarepants", "III")` 

---- **KWARGS ---- 
`def print_address(**kwargs):`
	 `for value in kwargs.values():` 
		 `print(value, end=" ")` 
`print_address(street="123 Fake St.", pobox="P.O Box 777", city="Detroit", state="MI", zip="54321")` 
		 
		 
---- EXERCISE ---- 
`def shipping_label(*args, **kwargs):` 
	`for arg in args:` 
		`print(arg, end=" ")` 
	`print()` 
	`if "apt" in kwargs:` 
		`print(f"{kwargs.get('street')} {kwargs.get('apt')}")` 
	`elif "pobox" in kwargs:`
		 `print(f"{kwargs.get('street')}")` 
		 `print(f"{kwargs.get('pobox')}")`
	`else:`
		 `print(f"{kwargs.get('street')}")`
	 `print(f"{kwargs.get('city')}, {kwargs.get('state')} {kwargs.get('zip')}")`
	 
`shipping_label("Dr.", "Spongebob", "Squarepants", street="123 Fake St.", pobox="PO box 1001", city="Detroit", state="MI", zip="54321")`


ref:[[Functions]]


