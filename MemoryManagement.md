# Memory management
* How is it handled?
  - Java's memory is handled by the JVM, which controls all memory allocation and deletion.
  
  - C# much like Java has an algorithm to handle memory management and allocation.
  
* How does it work?
  - Java uses a heap to store all objects, but there is also space allocated for Java methods, thread stacks, and native handles. The heap is seperated into two different sections (generations) called the nursery and the old space. All new objects are put into the nursury, and only transfered into the old space after a set amount of time have passed. The JVM also sees a differnce between object size and handles them differently based off of size, these sizes change dependent on the current use case.
  
  - C# also uses a heap to manage its allocated memory and it uses a fairly complex alogrithm to manage the memory. As objects are created they are placed into a generation, and a memory pointer is moved. That generation has a set size, and will eventually fill up, causing a new generation to be created and start filling the objects in the same way.
  
* Garbage collection?
  - Java use a mark and sweep collection method for getting rid of objects. As the name depicts, a sweep is ran through the entire memory and any object that can be consider dead or no longer in use is marked so. The sweep also marks open spaces between objects as places ready to have new objects inserted into them.
  
  - C# has a garbage collector can check if an item is still in use, and get rid of it if it is deemed no longer in use. The collecter uses a series of roots to mark the different memory locations being used and starts sorting through the memory. All items are at first considered garbage and only if a root can be found to match will the collecter keep the item. Once the item is removed the memory space is marked as free again in the register.
 
* Automatic reference counting?
  - Java does not use automatic reference counting as it is considered error prone.
  
  - C# does not use automatic reference counting for the same reasons Java does not.
