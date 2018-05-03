# Reflection
* What reflection abilities are supported?
  - Java
    * find out what methods are defined within a class
  
    Method methlist[]  = cls.getDeclaredMethods();
  
    * find out about the constructors of a class
  
    Constructor ctorlist[] = cls.getDeclaredConstructors();
  
    * find out which data fields are defined in a class
  
    Field fieldlist[] = cls.getDeclaredFields();
  
    * invoke a method of a specified name
  
    Class cls = Class.forName("method2");  
    Class partypes[] = new Class[2];  
    partypes[0] = Integer.TYPE;  
    partypes[1] = Integer.TYPE;  
    Method meth = cls.getMethod("add", partypes);  
    method2 methobj = new method2();  
    Object arglist[] = new Object[2];  
    arglist[0] = new Integer(37);  
    arglist[1] = new Integer(47);  
    Object retobj = meth.invoke(methobj, arglist);
  
    * creating new objects
  
    Class cls = Class.forName("constructor2");  
    Class partypes[] = new Class[2];  
    partypes[0] = Integer.TYPE;  
    partypes[1] = Integer.TYPE;  
    Constructor ct = cls.getConstructor(partypes);  
    Object arglist[] = new Object[2];  
    arglist[0] = new Integer(37);  
    arglist[1] = new Integer(47);  
    Object retobj = ct.newInstance(arglist);  
  
    * change the values of data fields in objects
  
    Class cls = Class.forName("field2");  
    Field fld = cls.getField("d");  
    field2 f2obj = new field2();  
    fld.setDouble(f2obj, 12.34);   
            
    * create and manipulate arrays
  
    Class cls = Class.forName("java.lang.String");  
    Object arr = Array.newInstance(cls, 10);  
    Array.set(arr, 5, "this is a test");  
    String s = (String)Array.get(arr, 5);  
  
  - C#
* How is reflection used?
 - Java
    * It allows an executing Java program to examine or "introspect" upon itself, and manipulate internal properties of the program. To use reflection in java you must import java.lang.reflect.* which gives you access to all of the methods for reflection.
 - C#
