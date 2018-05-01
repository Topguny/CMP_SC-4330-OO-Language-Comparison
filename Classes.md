# Classes
* Defining
  - Java
  
    public class MyClass{<br/>
      //stuff<br/>
    }
    
  - C#
* Creating new instances
  - Java
    
    MyClass Math = new MyClass();
    
  - C#
* Constructing/initializing
  - Java
  
    public class MyClass{<br/> 
      String name;<br/>
      public MyClass(String name){<br/>  
        this.name = name;<br/>
      }<br/>
    }
    
  - C#
* Destructing/de-initializing
  - Java
    * Garbage collection in Java handles the destrcuting of everything, things live as long as there's a reference that points to them. Some things do allow for the use of ".close" or ".dispose" but there are meant for freeing resources from uncessary things or to stop certain services from running. 
  - C#
