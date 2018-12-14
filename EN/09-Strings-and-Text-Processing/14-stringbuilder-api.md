[slide]
# Building and Modifying Strings
Strings in C# are immutable. This means that any adjustments applied to an existing string do not change it but return a new string. For example, using methods like **Replace(…)**, **ToUpper(…)**, **Trim(…)** do not change the string, which they are called for. They allocate **a new area in the memory** where the new content is saved. This behavior has many advantages but in some cases can cause **performance problems**. We can see this when trying to **concatenate strings in a loop**. The problem is directly related to the strings handling and dynamic memory, which is used to store them. 
**StringBuilder** is a class that serves to **build and change strings**. It overcomes the performance problems that arise when concatenating strings of type string. The class is built in the form of an **array of characters** and what we need to know about it is that the information in it can be freely changed. Changes that are required in the variables of type StringBuilder, are carried out in the same area of memory (buffer), which **saves time and resources**. Changing the content does not create a new object but simply changes the current.

## StringBuilder: How It Works?
Unlike the already familiar for us strings, the objects of the StringBuilder class are **not immutable**, namely edit operations do not require creating a new object in the memory. This reduces the unnecessary transfer of data in memory when performing basic operations such as string concatenation.
**StringBuilder** keeps a **buffer** with a certain capacity (16 characters by default). The buffer is implemented as an array of characters that is provided to the developer by a user-friendly interface – methods that quickly and easily add and edit elements of the string. At any moment part of the characters in the buffer are used and the rest stay in reserve. This allows the addition to **work very quickly**. Other operations also operate faster than the class string, because the changes **do not create a new object**.

- StringBuilder keeps a buffer memory, allocated in advance
    - Most operations use the buffer memory and do not allocate new objects. Once the **internal buffer** of the StringBuilder is full, it automatically is doubled (the internal buffer is resized to increase its capacity while its content is kept unchanged). Resizing is a slow operation but is happens **rarely** so the total performance is good.

[/slide]

[slide]
# Changing the Contents of a String
- Use the **System.Text.StringBuilder** class for modifiable strings of characters:
```csharp
public static string ReverseString(string s)
{
    StringBuilder sb = new StringBuilder();
    for (int i = s.Length - 1; i >= 0; i--)
    {
        sb.Append(s[i]);
    }    

    return sb.ToString();
}

```
- Use **StringBuilder** if you need to keep adding characters to a string


[/slide]





[slide]
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
Test your code.
[/task-description]

[code-io /]
[/code-task]


[/slide]


