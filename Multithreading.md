# Multithreading
* Threads or thread-like abilities
  - Java contains threads, and they are created using special defined objects.
  
  - C# also contains the ability to create additional threads.
* How is multitasking accomplished?
  - Java uses several things to create a thread and then decide when and how it runs. The first thing to do is create a class using the interface Runnable, which forces the inclusion of a run() method, and within that mehod you will put the code you want to execute once the thread is started. The other thing to do is to create a class that extends Thread, and give it a Runnable object, which will then create a thread than can started on command.
  
  - C# allows you to use they System.Threading namespace to handle all threading realated tasks. An object of class Thread must simply be created and then given a method to run. That thread can then be started with the .Start() method and whatever method given in the creation of the Thread will be ran. Below is a simple example of creating a thread and starting it with a method included in the creation of the Thread. 
   
   static void Main()

        {

            Thread t = new Thread(new ThreadStart(MyThreadMethod));
            t.Start();           

            Console.Read();

        }

        static void MyThreadMethod()

        {

            Console.WriteLine("Hello World!");

        }
