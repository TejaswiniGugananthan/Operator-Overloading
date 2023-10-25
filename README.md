# Operator-Overloading

## Aim:
 To write a C# program to pass values through constructors(default and parameterized) and also overload equal operators by checking whether objects are equal using operator overloading. 
 
 ## Algorithm:
step 1: Create a class for operator overloading.

step 2: Get inputs for length,breadth and height of the box from the user and then calculate the volume in overloading function.

step 3: After that return a new object for the calculated volume.

step 4: Then create a new object to store the return object.

step 5: After that print the calculated volume.
 
 
 ## Program:
 Name: G.TEJASWINI
 
 Reg no: 212222230157

 ```python
using System;
namespace ConsoleApp8
{
    class example
    {
        public int length;
        public example()
        {
            length = 10;
        }
        public example(int i)
        {
            length = i;
        }
        public static bool operator ==(example obj1, example obj2)
        {
            return obj1.Equals(obj2);
        }
        public static bool operator !=(example obj1, example obj2)
        {
            return !obj1.Equals(obj2);
        }
        public static void Main()
        {
            example e1 = new example();
            example e2 = new example(20);
            example e3 = new example();
            example e4 = e3;
            if (e3 == e4)
            {
                Console.WriteLine("Equal");
            }
            else if (e3 != e4)
            {
                Console.WriteLine("Not equal");
            }
        }
    }
}
```
 
 # Output:
 
 ![Screenshot (39)](https://github.com/TejaswiniGugananthan/Operator-Overloading/assets/121222763/e9325897-d327-4eaa-ae3b-f2eece3af6f7)

 ## Result:
 Thus the C# program to find the volume of a box using operator overloading is implemented successfully.
