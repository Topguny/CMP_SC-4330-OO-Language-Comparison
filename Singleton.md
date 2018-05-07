# Singleton
* How is a singleton implemented?
  - Java
  The most straightforward way to creating a singleton in Java is to create a private constructer and a field to hold its result, with a static accessor method, commonly getInstance(), that is public.
  - C#
  Below is an example of a singleton implementation in C#, and is simply one of many options to create a singleton in C#. It shares similarities with Java, due to the creation of a private constructer, with a get method to actually access the instance.  
  public class Singleton  
{  
   private static Singleton instance;  

   private Singleton() {}

   public static Singleton Instance  
   {  
      get 
      {  
         if (instance == null)  
         {  
            instance = new Singleton();  
         }  
         return instance;  
      }  
   }  

* Can it be made thread-safe?
  - Java
  Java singletons can be made thread safe a number of ways including creating the instance variable at the time of loading the class, synchronizing the getInstance mehod, and using a sychronized block inside the if loop and volatile variable.
  - C#
  C# can also create thread safe singletons, and just like Java has several methods of creation with different advantages and drawbacks. A common approach is to declare an object within the class and then use that object with the lock keyword to prevent more than one function from accessing the instance at once.
  
* Can the singleton instance be lazily instantiated?
  - Java
  Java can lazily instanciate a singleton, which causes the singleton instance to not actually be created until its fetch method, like getInstance() is called.
  
  public class ClassicSingleton {

   private static ClassicSingleton instance = null;  
   private ClassicSingleton() {  
      // Exists only to defeat instantiation.  
   }

   public static ClassicSingleton getInstance() {  
      if(instance == null) {  
         instance = new ClassicSingleton();  
      }  
      return instance;  
   }  
}
  - C#
  C# allows for a singleton to be lazily instantiated and have the singleton created upton the actual call of the get method, in this case it matches Java perfectly, outside of some differences in naming schemes.
  
