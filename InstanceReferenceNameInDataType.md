# Instance reference name in data type (class)
* this? self?
  - Java
    * Within an instance method or a constructor, this is a reference to the current object — the object whose method or constructor is being called. You can refer to any member of the current object from within an instance method or a constructor by using this.
    
    public class Point {  
      public int x = 0;  
      public int y = 0;  
      //constructor  
      public Point(int x, int y) {  
          this.x = x;  
          this.y = y;  
      }  
    }
    
  - C#
