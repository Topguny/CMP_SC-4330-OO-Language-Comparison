# Inheritance / Extension
* Both Java and C# implicitly inherent from an object class for all objects/classes that are made allowing them to have access to basic methods.
* Java
  - Inheritance and Extension go hand in hand in Java, as a sub-class can inherit  fields and methods from its superclass. And how you declare a class a sub-class of another class or a superclass is by using the keyword "extends". A key thing to remember is a class in Java only supports single Inheritance and not multiple.
  
  public class Pet{  
  //stuff  
  }
  
  public class Dog extends Pet{ //this is where a dog gets ineheritance from pet by extending from it   
    
  }
  
* C#
  - Much like Java C# only supports single inheritance, it also follows very similar guidelines for inheritance/extension. Unlike Java, C# use the ":" to show extension, instead of a keyword like java. 
  
  public class Pet{  
  //stuff  
  }
  
  public class Dog : Pet{ // ":" show us that dog extends pet  
    
  }
