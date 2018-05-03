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
    * Use "Assembly" to define and load assemblies, load modules that are listed in the assembly manifest, and locate a type from this assembly and create an instance of it.
    * Use "Module" to discover information such as the assembly that contains the module and the classes in the module. You can also get all global methods or other specific, nonglobal methods defined on the module.
    * Use "ConstructorInfo" to discover information such as the name, parameters, access modifiers (such as public or private), and implementation details (such as abstract or virtual) of a constructor. Use the GetConstructors or GetConstructor method of a Type to invoke a specific constructor.
    * Use "MethodInfo" to discover information such as the name, return type, parameters, access modifiers (such as public or private), and implementation details (such as abstract or virtual) of a method. Use the GetMethods or GetMethod method of a Type to invoke a specific method.
    * Use "FieldInfo" to discover information such as the name, access modifiers (such as public or private) and implementation details (such as static) of a field, and to get or set field values.
    * Use "EventInfo" to discover information such as the name, event-handler data type, custom attributes, declaring type, and reflected type of an event, and to add or remove event handlers.
    * Use "PropertyInfo" to discover information such as the name, data type, declaring type, reflected type, and read-only or writable status of a property, and to get or set property values.
    * Use "ParameterInfo" to discover information such as a parameter's name, data type, whether a parameter is an input or output parameter, and the position of the parameter in a method signature.
    * Use "CustomAttributeData" to discover information about custom attributes when you are working in the reflection-only context of an application domain. CustomAttributeData allows you to examine attributes without creating instances of them.
* How is reflection used?
  - Java
    * It allows an executing Java program to examine or "introspect" upon itself, and manipulate internal properties of the program. To use reflection in java you must import java.lang.reflect.* which gives you access to all of the methods for reflection.
  - C#
    * You can use reflection to dynamically create an instance of a type, bind the type to an existing object, or get the type from an existing object and invoke its methods or access its fields and properties. If you are using attributes in your code, reflection enables you to access them. Much like Java C# requires you to inlcude the system for reflection, "using System.Reflection;".
