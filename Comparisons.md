# Comparisons of references and values
* How are values compared? (i.e. comparing two strings)
  -Java
  
  In Java there are two different ways to compare objects, by reference and by value. By reference directly compares the two objects to see if they are the same, objects using the == operater to compare them. 
  
  Int a = 1;
  Int b = 1;
  
  if(a == b)
  {
    This is not entered, because a and b are different objects.
  }
  
  For the case of comparing two objects by value, the equals method can be used to compare the values of two objects.
  
  if(a.equals(b))
  {
    This is entered because the values of the two objects are identical, even if they are not the same object.
  }
  
  -C#
  
  In C# there are two ways to compare objects, by reference and by value. By reference directly compares the two objects to see if they are the same, objects, meaning that even if they share the same value, they may still be two seperate and thusly different objects.
  
  Test a = 1;
  Test b = 1;
  
   bool areEqual = System.Object.ReferenceEquals(a, b); (This would be False)
   a = b;
   bool areEqual = System.Object.ReferenceEquals(a, b); (This would be True)
   
   The other way to compare to items is by value, where we simple compare of the two values stored inside an object and see if they are equal.
   
   int a = 1;
   int b = 1;
   
   if (a == b)
   {
      Console.WriteLine("Both a and b are the same.");
   }
