## Methods
```sh
using System;

namespace MyApplication
{
  class Program
  {
    static int MyMethod(int x, int y)
    {
      return x + y;
    }

    static void Main(string[] args)
    {
      Console.WriteLine(MyMethod(5, 4));
    }
  }
}
```
* With method overloading, multiple methods can have the same name with different parameters (same operation, diff variable types)


## Classes
* A ``constructor`` is a special method that is used to initialize objects. The advantage of a constructor, is that it is called when an object of a class is created. It can be used to set initial values for fields.
* Acces modifiers:   
      *  ``public``	The code is accessible for all classes
      *  ``private``	The code is only accessible within the same class
      *  ``protected``	The code is accessible within the same class, or in a class that is inherited from that class. You will learn more about inheritance in a later chapter
      *  ``internal``	The code is only accessible within its own assembly, but not from another assembly. You will learn more about this in a later chapter

