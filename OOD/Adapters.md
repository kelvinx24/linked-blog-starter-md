Problem: I want to link 2 libraries together but I can't modify any code

## Class Adapter Pattern
![[ClassAdapter 2.svg]]
The adaptee is extended (inherited) and the target is implemented

Positives
- Get all of IAdaptee for free - don't have to rewrite
- Reuse the same obj as both a IAdaptee and ITarget (with one name) - can be casted

Cons
- Exposes all of IAdaptee
	- Unecessary methods have to throw exceptions
	- EX: ListToStackAdapter has getIndex() from List even though not needed

## Object Adapter Pattern
![[ObjectAdapter.svg]]
The adaptee is passed into the adapter (composition) and the target is implemented

Pros:
- Converting from adaptee to target is easy - quick conversion
- Pick and choose methods to add from non-ITarget interfaces

Cons:
- No methods are free: all need an implementation
- To have object that can used in both libraries, I need 2 aliases - can't cast