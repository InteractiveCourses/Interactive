[slide]
# Working with Arrays of Elements
## What are Arrays?
- In programming, **array** is a **sequence of elements**
    - Elements are **numbered** from **0** to **Length-1**
    - Elements are of the **same type** (e.g. integers)
    - Arrays have **fixed size** (**Array.Length**) – cannot be resized

[/slide]

[slide]
# Working with Arrays
Before we can use an element of a given array, it has to be **initialized** or to have a **default value**. In some programming languages there are no default values and then if we try to access an element, which is not initialized, this may cause an error. In **C#** all variables, including the elements of arrays have a **default initial value**. This value is either **0** for the numeral types or its equivalent for the non-primitive types (for example **null** for a reference type and **false** for the bool type).

- **Allocating** an array of 10 integers:

```csharp
int[] numbers = new int[10];
```
- **Assigning values** to the array elements. Each element can be accessed through the **name of the array** and the **element’s index** (consecutive number) placed in the brackets. We can access given elements of the array both for **reading** and for **writing**, which means we can **treat** elements as variables.
```csharp
for (int i = 0; i < numbers.Length; i++)
    numbers[i] = 1;

```
- **Accessing** array elements by index. 
```csharp
numbers[5] = numbers[2] + numbers[7];
numbers[10] = 1; // IndexOutOfRangeException

```


[/slide]

[slide]
# Days of Week – Example

- The days of week can be stored in **array of strings**:
```csharp
string[] days = {
  "Monday",
  "Tuesday",
  "Wednesday",
  "Thursday",
  "Friday",
  "Saturday",
  "Sunday"
};


```

[/slide]

[slide]
# Problem: Day of Week

- Enter a **day number** [1…7] and print the **day name** (in English) or "**Invalid day!**"

[image src=https://github.com/InteractiveCourses/Interactive/blob/master/assets/ProblemDayOfWeek.png alt="ProblemDayOfWeek" /]

Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/172#0]https://judge.softuni.bg/Contests/Practice/Index/172#0[/anchor]

# Try it yourself!

[code-task title="Try it yourself!" executionStrategy="csharp-dot-net-core-code" requiresInput]

[code-editor language=csharp]
```
using System;

namespace App
{
    class Program
    {
        static void Main(string[] args)
        {
		    // enter your code here
		    
		}
	}
}
```
[/code-editor]

[task-description]
Enter a day number [1…7] and print the day name (in English) or "Invalid day!"
[/task-description]

[code-io /]
[/code-task]


[/slide]
[slide]
# Solution: Day of Week
```csharp
string[] days = { "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday" };
int day = int.Parse(Console.ReadLine());

if (day >= 1 && day <= 7)
   Console.WriteLine(days[day - 1]);
else
   Console.WriteLine("Invalid day!");
```

[/slide]


