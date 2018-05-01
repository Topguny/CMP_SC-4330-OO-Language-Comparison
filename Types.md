# Types
* What types does the language support?
  - Java
    * Primitive Data types, are literals. Meaning they are not objects of a class, but rather the source code representation of a fixed value.
    
    ![alt text](https://github.com/Topguny/CMP_SC-4330-OO-Language-Comparison/blob/master/typesJava.PNG?raw=true)
    
    * There is also objects for each of the data types, primitive data types are lower case like integer, while the object is capitilized like Integer. This object acts as a wrapper for the primitive types, and is what allows you to convert an integer to a string or any of the functions meant to be used to convert.
  - C#
    * C# has several types of data, the first being ValueTypes, which are similar to primitive types in how they are directly given a value. 
    
    ![alt text](https://github.com/Topguny/CMP_SC-4330-OO-Language-Comparison/blob/master/typesC%23.PNG?raw=true)
    
* Are both reference and value types supported?
  - Java
    * Kinda, Java makes things complicated. All data is passed by value, but objects are sometimes passed by reference via a pointer. Some cases of this are Field access, Method invocation, the cast operator, the string concatenation operator, the instanceof operator, the reference equality operator and the conditional operator.
  - C#
* Can new value types be created?
  - Java
    * Yes in the sense that you can make a new object like we talked about above, essentially making a new wrapper class to hold your own data type in.
  - C#
