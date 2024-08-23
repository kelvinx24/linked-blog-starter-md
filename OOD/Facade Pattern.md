**The Facade Pattern** provides a unified interface to a set of interfaces in a subsystem. Facade defines a higher-level interface that makes the subsystem easier to use.

- When you need to simplify and unify a large interface or complex set of interfaces, use a facade
- A facade decouples a client from a complex subsystem
- Implementing a facade requires that we compose the facade with its subsystem and use delegation to perform the work of the facade.

Diagram:
![[272fig01.png.jpg]]

EX)
![[277fig01.png.jpg]]