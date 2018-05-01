# Types
* What types does the language support?
  - Java
    * Primitive Data types, are literals. Meaning they are not objects of a class, but rather the source code representation of a fixed value.
    
    ![alt text](https://github.com/Topguny/CMP_SC-4330-OO-Language-Comparison/blob/master/typesJava.PNG?raw=true)
    
    * There is also objects for each of the data types. Primitive types are lower case like integer, while the object is capitilized like Integer. This object acts as a wrapper for the primitive types, and is what allows you to convert an integer to a string or any of the functions meant to be used to convert.
  - C#
    * ValueTypes:which are similar to primitive types in how they are directly given a value. 
    
    ![alt text](https://github.com/Topguny/CMP_SC-4330-OO-Language-Comparison/blob/master/typesC%23.PNG?raw=true)
    
    * Reference Taype: The reference types do not contain the actual data stored in a variable, but they contain a reference to the variables.
    * Object Type: The Object Type is the ultimate base class for all data types in C# Common Type System (CTS). Object is an alias for System.Object class. By converting a valuetype to an object type, it is called boxing. And converting it back is unboxing. This is kinda mesh of Java and its object class for primitive types, and swift.
    * Dynamic Type: You can store any type of value in the dynamic data type variable. Type checking for these types of variables takes place at run-time.
    * String Type: The String Type allows you to assign any string values to a variable. The string type is an alias for the System.String class. It is derived from object type.
    
* Are both reference and value types supported?
  - Java
    * Kinda, Java makes things complicated. All data is passed by value, but objects are sometimes passed by reference via a pointer. Some cases of this are Field access, Method invocation, the cast operator, the string concatenation operator, the instanceof operator, the reference equality operator and the conditional operator.
  - C#
    * C# is similar to Java in the sense that valuetypes/primitie data types are passed by value, but when passed to a method it ispass by reference.
* Can new value types be created?
  - Java
    * Yes in the sense that you can make a new object like we talked about above, essentially making a new wrapper class to hold your own data type in.
  - C#
    * Much like Java you have to make your own class, you can also use structs to do this in a similar way.
