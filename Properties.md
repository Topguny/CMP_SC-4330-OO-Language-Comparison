# Properties
  - Java
    * Properties in java are kinda managed as key/value pairs, you do build your own. But generally you ask for getName, and it returns the value.
  - C#
    * C# kinda treat properties as the same, a set of key/value pairs.
* Getters and setters…write your own or built in?
  - Java
    * Java you build your own getters and setters.
    
    public class Employee{  
      private string name;  
      public string getName(){  
        return name;  
      }  
    }
    
  - C#
    * C# lets you do it the exact way java does it, but since c# 1.1 they have implemented many ways to do. Such as:
    
    public class Foo{  
    private string bar;  
    public string Bar{  
        get { return bar; }  
        set { bar = value; }  
    }  
    }

    public class Foo{  
      public string Bar { get; set; }  
    }  
    
    public class Foo{  
      private string bar;  
      public string Bar{  
        get{ return bar; }  
      }  
    }
    
    public class Foo{  
      public string Bar { get; private set; }
    }
    
* Backing variables?
  - Java
  - C#
* Computed properties?
  - Java
  - C#
