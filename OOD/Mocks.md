Fake components used for testing
- Usually for inputs 

EX : 
A theoretical mock class based on a calculator program
```
public class mockModel implements model {
	final StringBuilder log
	add(int n1, int n2) {
	log.append(n1, n2)}
}
```

Then, you would initialize mockModel and pass it into the controller =>
check log after controller executes


Problem: A component of my system with an interface does not have the interface needed to help with testing

Solution Make a fake component and use that for testing

1) What are we testing for? (ex: controller passes inputs to model w/o change) 
2) Can we test for that with the current component?
3) Create a Mock class that implements the component's interface.
4) For each method implemented, decide how to get the desired testing info to the test (ex: print inputs to console)
5) When testing, pass in the Mock instead of real component
