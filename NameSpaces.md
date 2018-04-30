# Name spaces
* How are name spaces implemented?
  - Java
    * Java uses the term packages, when a new project is started it auto generates a package as well for you, Packages hold classes, classes hold code.
    * Essentially used to organize files or types to avoid conflicts.
    * Access can be restricted so that a class can only be acessiable from within its own package.
  - C#
    * C# actually uses the name namespace for its system, its system does pretty well just mirror Javas.
    * Namespaces are used to organize programs, both as an "internal" organization system for a program, and as an "external" organization system.
      
* How are name spaces used?
  - Java
    * You can map to a file system or package, by using a "." such as in someting like      system.security.cryptography.AsymmetricAlgorithm aa; or you can import the package like import system.security.Crypography; and simply call AsymmetricAlgorithm aa;.
  - C#
    * Much like Java, we can do System.Security.Cryptography.AsymmetricAlgorithm aa; or call "using" instead of the java import term and do using System.Security.Crypography; AsymmetricAlgorithm aa;.
    * Unlike Java we can create alernative names called aliases for these package calls. using myAlias = System.Security.Crypography;  myAlias.AsymmetricAlgorithm = aa;
