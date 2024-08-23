Problem: I want to enhance existing features w/ the following requirements
1) No editing existing classes
2) New enhanced classes must function like the existing ones
3) Features can be composed 

# Decorator Pattern
Class is the existing interface(implements) and also has an object of the existing interface (composition)

All following extends this new decorator class

# Strategy
Problem:  I want to switch the algorithm a class uses at runtime

Solution:
1) Determine type of the algorithm - Functions
	- EX: Fn<Int, String>
2) Make an interface w/ 1 function: that function has the algorithm's type signature
3) For every implementation of algorithm implement this interface with a class


