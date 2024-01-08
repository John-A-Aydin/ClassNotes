A new style of concurrent programming
- Used in GUI-based applications, some types of internet servers

Instead of having all of these [[Threads|threads]] lets just use one and get rid of these dang locks
- Dev has very little control over what happens at any given time

### The Event Loop

- Wait for something (event)
	- Ex. Update of state is React
- When it does, check what type of event it is
- Do the small amount of work that type of event requires

#### select() API
- Check whether there is any open I/O

### Approaches

- Async API
	- requires frequent checks to see if its done
- Interrupt
	- Uses UNIX signals
	- Need to remember why 