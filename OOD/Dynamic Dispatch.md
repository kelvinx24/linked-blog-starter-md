Important Topic for Fundies

Dynamic dispatch is the act of calling a method on non-concrete object.

Involves subclasses

For example, take the an two classes, Person and Other, that implements the interface IAT. When a method is called on an object IAT, the program automatically knows which class's method to call, depending on what IAT actually is.

This feature is helpful when we have to call methods on an interface.

[[Java]]

## Double Dynamic Dispatch
When you do not know the exact object type of one or both objects, so you call a method within the unknown object to identify it

Do not know obj1 => call method / dispatch to identify obj1 => obj1 identified - can now manipulate fields within obj1 => call method / dispatch to identify obj2

EX) 
return obj.sameShape(obj1);
public boolean sameShape(IShape that) { return that.sameCircle(this); } - obj1 is a circle

public boolean sameCircle(Circle obj1) { return that.radius == this.radius; } - will be called if obj2 is a circle, but sameSquare or sameTriangle could be called if obj2 was not a circle