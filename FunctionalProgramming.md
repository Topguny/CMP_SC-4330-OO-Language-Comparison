# Functional programming
* Does the language support functional programming?
  - Java
    While Java is not a functional langauage, it supports functional programming in a limited way in the form of lambda expressions. Lambda expressions allow for functions to exist outside of the class and object structure normally present in Java. Lambda expressions were added in Java 8, and did not exist prior to that release. Lambda's are often used in conjunction with interfaces.   
final Array<Integer> a = array(1, 2, 3);  
final Array<Integer> b = a.map({int i => i + 42});  
arrayShow(intShow).println(b); // {43,44,45}
  
  
  - C#
  Once again, C# and Java show their similarity because C# also supports functional programing in the form of lambda expressions, however C# takes it a step further and actually supports a large set of functional tools. Generics, functions as return values for other functions, more true to functional closures, as well as LINQ. There are also signs that Microsoft plans on taking things a step further and implementing structual typing in the next large patch to C#. C# when created started off as an OO language, but over time it has been picking up more and more functional type aspects.
