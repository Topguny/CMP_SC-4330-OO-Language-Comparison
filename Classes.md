# Classes
* Defining
  - Java
  
    public class MyClass{<br/>
      //stuff<br/>
    }
    
  - C#
  
    public class Customer{<br/>
    // Fields, properties, methods and events go here...<br/>
    }
  - Java and C# both declare/define their classes very similarly if not identically.
* Creating new instances
  - Java
    
    MyClass Math = new MyClass();
    
  - C#
    
    Customer object1 = new Customer();
    
  - Again creating a new instance an object of a class is very similar between the two languages.
* Constructing/initializing
  - Java
  
    public class MyClass{<br/> 
      String name;<br/>
      public MyClass(String name){<br/>
        this.name = name;<br/>
      }<br/>
   }
    
  - C#
  
    public class Customer{<br/> 
      String name;<br/>
      public Customer(String name){<br/>
        this.name = name;<br/>
      }<br/>
    }
  
  - Again C# and Java are almost identical in terms of constructors.
  
* Destructing/de-initializing
  - Java
    * Garbage collection in Java handles the destrcuting of everything, things live as long as there's a reference that points to them. Some things do allow for the use of ".close" or ".dispose" but there are meant for freeing resources from uncessary things or to stop certain services from running. 
  - C#
    * Much like Java C# has built in garbage collection so you never really need to worry about this. But you can make your own deconstructor if you want to. 

    class Customer{<br/>
      ~Customer(){  // destructor<br/>
        // cleanup statements...<br/>
      }<br/>
    }
    
    * The deconstructor implicitly calls finalize on the base class of the object. The code above gets implicility translated into the following code.
    
    protected override void Finalize(){<br/>
      try{<br/>
        // Cleanup statements...<br/>
      }<br/>
      finally{<br/>
        base.Finalize();<br/>
      }<br/>
    }
