# Classes
* Defining
  - Java
    public class MyClass{
      //stuff
    }
  - C#
* Creating new instances
  - Java
    MyClass Math = new MyClass();
  - C#
* Constructing/initializing
  - Java
    public class MyClass{
      String name;
      public MyClass(String name){
        this.name = name;
      }
    }
  - C#
* Destructing/de-initializing
  - Java
    * Garbage collection in Java handles the destrcuting of everything, things live as long as there's a reference that points to them. Some things do allow for the use of ".close" or ".dispose" but there are meant for freeing resources from uncessary things or to stop certain services from running. 
  - C#
