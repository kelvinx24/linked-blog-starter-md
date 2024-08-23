#Java  allows omitting the parameter(s) on types and constructors:

EX: 
```
BinTree tree = new BinTree();
List l = new ArrayList();
```

**DONT USE**

## CONSEQUENCES
- Rampant type-casting
- Class cast [[Exceptions]] when casting goes wrong
- Unchecks casts lead to [[Exceptions]] later