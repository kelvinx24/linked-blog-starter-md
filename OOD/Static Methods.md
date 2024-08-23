_Static_ describes things that happen or are determined at compile time, and _dynamic_ describes things that happen or are determined at run time

in Java in particular, static means that some member—a field, method, or nested class—is part of its class

## When to Use
- Fields: one variable for the whole class rather than one per
object
	- Should be rare except for constants
- Methods: a method associated with the class that does not
depend on an instance
	- Factory methods are a common case
	- Implementation does not rely on representation of the obeject
- Classes: helper classes with strong associations
	- An iterator class nested in a collection class
	- class does not rely on the representation of outer class

Can be called via:
<class-name>.<the thing you want>


#Java 