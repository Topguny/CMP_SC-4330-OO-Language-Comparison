# Errors and exception handling
* Exceptions
  - Java
  
    In Java exceptions, can be classified under two different categories, checked exceptions and run time exceptions. Checked exceptions are errors that the compiler finds in the code that will be force the program to break or stop, and prevent the program from finishing compiling. Run time exceptions are errors that occur during the execution of the code and may happen sometimes and not others. A try catch block can be used to gather information on these run time exceptions, by putting code inside a try block that commonly may cause an exception and then performing the code inside the catch block if an exception is thrown.

try { <br/>
       //Code that you expect could throw an exception goes here <br/>
    }<br/>
catch (Exception ex)<br/>
    {<br/>
    
    }


All exception classes are subtypes of the java.lang.Exception class, and this can be used to define what kind of exception you expect to catch. This allows the programmer to define different catch blocks for different kinds of exceptions that are thrown.
    
    
    
  - C#
  
    C# handles exceptions almost identically to Java, because it also used try catch blocks to handle exceptions thrown by the program.
    
    try<br/>
{<br/>
    // Code that you expect could throw an exception goes here.<br/>
}<br/>
catch (SomeSpecificException ex)<br/>
{<br/>
    // Code to handle the exception goes here.<br/>
    // Only catch exceptions that you know how to handle.<br/>
    // Never catch base class System.Exception without<br/>
    // rethrowing it at the end of the catch block.<br/>
}
