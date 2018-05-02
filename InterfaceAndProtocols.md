# Interfaces / protocols
* What does the language support?
  - Java
    * Java supports Interfaces. Interfaces are blueprints of classes
  - C#
    * C# also uses Interfaces and is defined as containing "definitions for a group of related functionalities that a class or a struct can implement."
* What abilities does it have?
  - Java
    * Ability to achieve total abstraction
    * Achieve multiple inheritance
    * Used for loose coupling.
  - C#
    * Much like Java classes do not support multiple inheritance, but interfaces do.
    * Also if you want to simulate inheritance in structs, you must you an interface.
* How is it used?
  - Java
    * First you must create your interface, then you use the keyword "implements" followed by the interface on a class to use it.
    
    interface in{  
    //what you want it to do  
    }
    
    class testClass implements in{  
    //what ever you want it to do  
    }
    
  - C#
    * using interfaces in C# is similar to Java but not identical, like Java you must first make it. But instead of impelements, you use a ":" to show inheritance.

    interface IEquatable<T>{  
        //whatever you want to do  
    }
  
    public class Car : IEquatable<Car>{  
        //whatever you want to do.  
    }
