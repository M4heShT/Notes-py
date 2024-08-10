dictionary = a collection of {key: value} pairs ordered and changeable. No duplicates 



`capitals = {"USA": "Washington D.C.", "India": "New Delhi", "China": "Beijing", "Russia": "Moscow"}` 

`print(dir(capitals))             -----> shows possible fn can do in dict()`
 `print(help(capitals))       -------> shows details of each fun.`
`print(capitals.get("India"))    ------> prints the value in given dict of resp. key if doesn't have any key-value pair it returns none.`

`if capitals.get("Russia"):` 
	`print("That capital exists")` 
`else:` 
	`print("That capital doesn't exist")          ------> this if-else loops checks if value in given dict`

`capitals.update({"Germany": "Berlin"})    -----> it updates the dict`
`capitals.update({"USA": "Detroit"})`
`capitals.pop("China")     -------> it remove the key-value from dict`
`capitals.popitem()        ---------> it remove the last/recently added item from dict`
`capitals.clear()           -----------> it clears the whole dict`

`keys = capitals.keys()      ------> it prints only keys from dict`
`for key in capitals.keys():  ------>it iterates the keys from dict`
`print(key)` 

`values = capitals.values()    ------------->  it prints only keys from dict`
`for value in capitals.values():   ------>it iterates the values from dict`
`print(value)` 

`items = capitals.items()   ----------> it prints the key-value pair in 2d tuple/collection`
`for key, value in capitals.items():    ------>it iterates both key and values pairs from dict`
`print(f"{key}: {value}")`



ref : [[Collections]]