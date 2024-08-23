# SOLID

## Single Responsibility
**S**ingle responsibility: every object should be responsible for one focused purpose

## Open / Closed
**O**pen/closed: everything can be open to extension but closed to modification - adding on to existing features by using interfaces

- Client looks at interface => interface is updated with new methods or a new implementation

## Liskov Substitution
**L**iskov substitution: if a type S is a subtype of a type T, then objects of type S can be used anywhere objects of type T can - interfaces and abstraction

![[word-image-7.png]]

![[word-image-8.png]]

## Interface Segregation
**I**nterface segregation: no client should be forced to depend on methods it doesn't use - break up interfaces if methods are not used in all classes, aka throws exception

![[word-image-12.png]]


![[word-image-13.png]]

## Dependency Inversion
**D**ependency inversion: abstractions should not depend on details; rather the reverse - high-level class only knows about interface rather than an instance of the interface

- Client => High-Level => Low-Level
- Higher up should not be affected by lower - Client and high-level should not be affected by low-level

![[solid-dependency-inversion-coffee-machine-18.png]]

![[solid-dependency-inversion-coffee-machine-19.png]]

#Java #Principles

## Additional OOD Principles
### Principle of Least Knowledge
**Talk only to immediate friends** - limit the number of classes coupled to one class
and how it interacts with those classes

EX)
![[274fig01.png.jpg]]

Only invoke methods that belong to:
- The object itself
- objects passed in as a parameter to a method
- objects created from the method itself aka new Blank()
- Any components/fields of the object

EX)
![[275fig01.png.jpg]]

**NOTE**: Principle may result in more wrappers being written to handle method calls to other components