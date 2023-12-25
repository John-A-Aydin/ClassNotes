### Procedural
More explicit

### Descriptive
- Pseudo-Prolog
	- Ex. Database contains
		- Facts (Data definitions and properties)
			- eat(bear, fox) (bear eats fox) 
			- eat(fox, squirrel)
			- eat(bear, fish)
			- eat(bear, deer)
			- animal(fox)
			- animal(deer)
			- plant(grass)
			- eat(deer, grass)
		- Rules
			- prey(x) if animal(x) and eat(z, x)
			- carnivore(x) if animal(x) and eat(x, z) and animal(z)
			- foodchain(x, y) (The data for eats() can be looked at as a tree or graph )
				- solve this recursively
				- if eat(y,x)
				- if eat(y, z) and foodchain(x, y) *Recursive call to function iterating to next node*
				- We can traverse the graph in either direction or both simultaneously to arrive at the correct answer
				- The way we traverse the graph is related to how the data is structured or what we're querying. 
				- Ex. If the query is ancestor(x, y) we want to take a top down approach
				- 