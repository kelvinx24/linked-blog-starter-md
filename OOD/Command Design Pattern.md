Problem: Want to a way to add new commands and limit the growth of methods/class

Solution: Make each command a class following the same interface

1) Make an interace with 1 method: execute().
2) For each command, implement a class that implements that interface
3) in the [[Model-View-Controller (MVC)#Controller|controller]] , depending on the input, create the corresponding command object
4) after processing that input, call execute on command