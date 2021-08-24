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
