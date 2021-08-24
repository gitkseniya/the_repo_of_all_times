### Syntax

* ``Console.Write("Hello World!")`` or ``Console.WriteLine("Hello World!")``
* Comments: ``//`` or ``/* this is a multi-line comment */``
* Variables:
  *   ``int``  ||   ``double`` (15 decimals) = 10.877777D (D at the end not req)   ||    ``char`` (single quotes)  ||   ``string`` (double quotes)  ||   ``bool``     || ``long`` (super-large nums) || ``float`` (6-7 decimals) = 5.75F
  *   type variableName = value;  
      *   string name = "John";     
         Console.WriteLine(name);
      *   const int myNum = 15; // can't overwrite this value
      *    float f1 = 35e3F;    
           double d1 = 12E4D;   
           Console.WriteLine(f1) = 35000;     
           Console.WriteLine(d1) = 120000;    
* Type casting
  * Implicit - smaller type to larger (char -> int -> long -> float -> double)
  * Explicit - larger type to smaller (double -> float -> long -> int -> char)
  * Built-in conversion tools: Convert.ToBoolean, Convert.ToDouble, Convert.ToString, Convert.ToInt32 (int) and Convert.ToInt64 (long)

### User Input
* ``Console.ReadLine()``
* Convert user input:
  * Console.WriteLine("Enter your age:");   
    int age = Convert.ToInt32(Console.ReadLine());   
    Console.WriteLine("Your age is: " + age);     
    
 
### Operators
* % modulus
* ++ // add 1
* -- // substract 1
* +=n // add n
* <<= 3 // n * 2 to the power of 3

### Math
* Math.Max(5, 10)
* Math.Min(x,y)
* Math.Sqrt(64)
* Math.Abs(-14.7) // returns the absolute (positive) value of x (14.7)
* Math.Round()

### String
* txt.Length
* ToUpper() // all caps
* ToLower() // all lowcase
* string.Concat(x, y)
* string name = $"My full name is: {firstName} {lastName}";
* Console.WriteLine(myString[0]);  // Outputs "H" from "Hello"
* Console.WriteLine(myString.IndexOf("e"));  // Outputs "1" from "Hello"
* Console.WriteLine(name.Substring(name.IndexOf("D"))) // name = "Jane Doe" => Doe
* string txt = "We are the so-called \"Vikings\" from the north."; // to read double quotes within double qoutes
* string txt = "It\'s alright."; // to read single quotes within double qoutes
* string txt = "The character \\ is called backslash."; // => The character \ is called backslash.
* ``new line`` string txt = "Hello\nWorld!";
* ``tab`` string txt = "Hello\tWorld!"
* ``backspace`` string txt = "Hel\blo World!";

### Boolean
* Console.WriteLine(isCSharpFun);   // Outputs True
* Console.WriteLine(10 > 9); // returns True, because 10 is higher than 9

### If Else
* Conditional statements:
  * ``if`` execute if a specified condition is true
  * ``else`` to specify a block of code to be executed, if the same condition is false
  * ``else if`` to specify a new condition to test, if the first condition is false
  * ``switch`` to specify many alternative blocks of code to be executed
  * int x = 20;   
    int y = 18;    
    if (x > y)    // note the ()
    {  
      Console.WriteLine("x is greater than y");    
    }.   
   * ``ternary operator``string result = (time < 18) ``?`` "Good day." ``:`` "Good evening."; // if else
 
 ### Switch
 Case by case
 ```sh
 using System; 

namespace MyApplication   
{  
  class Program  
  {   
    static void Main(string[] args)    
    {   
      int day = 4;   
      switch (day)   
      { 
        case 1:  
          Console.WriteLine("Monday");  
          break;  
        case 2:  
          Console.WriteLine("Tuesday");  
          break;  
        case 3:  
          Console.WriteLine("Wednesday");  
          break;  
        case 4:  
          Console.WriteLine("Thursday");  
          break;  
        case 5:  
          Console.WriteLine("Friday");  
          break;  
        case 6:  
          Console.WriteLine("Saturday");  
          break;  
        case 7:  
          Console.WriteLine("Sunday");  
          break;  
          
          default:   
          Console.WriteLine("Looking forward to the Weekend.");  
          break;   
      }    
    }
  }
}
```
// outputs Thursday since input is 4. ``break`` When a match is found, and the job is done, it's time for a break. There is no need for more testing.  
// ``default`` sets output if conditions haven't been met

### While Loop
* ``while`` In the example below, the code in the loop will run, over and over again, as long as a variable (i) is less than 5:
```sh
int i = 0;   
while (i < 5)   
{  
  Console.WriteLine(i);   
  i++;   
}  
```
* ``do/while`` This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.
* ``for`` (int i = 0; i < 11; i++)  // (executed before code; condition; executed after) 
* ``foreach`` (string i in {"Volvo", "BMW", "Ford", "Mazda"}) 
* ``break`` statement can also be used to jump out of a loop
* ``continue`` breaks one iteration (in the loop), if a specified condition occurs, and continues with the next iteration in the loop. 

### Arrays
