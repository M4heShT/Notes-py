recursion = a function that calls itself from within 
helps to visualize a complex problem into basic steps 
problems can be solved more easily iteratively or recursively 

iterative = faster, complex
recursive = slower, simpler

---- EXAMPLE 1 ---- 
ITERATIVE 
`def walk(steps):` 
	`for step in range(1, steps+1):` 
		`print(f"You take step #{step}")`
		
RECURSIVE 
`def walk(steps):` 
	`if steps == 0:`
		 `return walk(steps - 1)`
		  `print(f"You take step #{steps}")` 
		  
`walk(100)`