[slide]
# Problem: Short Words Sorted

Read a **text**, extract its **words**, find all **short words** (less than 5 characters) and print them **alphabetically**, in **lower case**.

- Use the following separators: . , : ; ( ) [ ] " ' / \ ! ? (space)
- Use case-insensitive matching; remove duplicated words

Input: In SoftUni you can study Java, C#, PHP and JavaScript. JAVA and c# developers graduate in 2-3 years. Go in!
Output: 2-3, and, c#, can, go, in, java, php, you

Check your solution here:
[code-task title="Working with collections" executionStrategy="csharp-code" requiresInput]
[code-editor language=csharp]
```csharp
using System;
using System.Collections.Generic; // needed for List<T>
using System.Linq;  // needed for Select(), OrderBy(), etc.

class Program
{
  static void Main(string[] args)
  {
    char[] separators = new char[] 
{'.',',',':',';','(',')','[',']','\\','\"','\'','/','!','?',' '};
    string sentence = Console.ReadLine().ToLower();
    string[] words = sentence.Split(separators);
    // var result = ...
  }
}
```
[/code-editor]
[task-description]Read a **text**, extract its **words**, find all **short words** (less than 5 characters) and print them **alphabetically**, in **lower case**.[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Short Words Sorted

[code-task title="Working with collections" executionStrategy="csharp-code" requiresInput]
[code-editor language=csharp]
```csharp
using System;
using System.Collections.Generic; // needed for List<T>
using System.Linq;  // needed for Select(), OrderBy(), etc.

class Program
{
  static void Main(string[] args)
  {
    char[] separators = new char[] 
{'.',',',':',';','(',')','[',']','\\','\"','\'','/','!','?',' '};
    string sentence = Console.ReadLine().ToLower();
    string[] words = sentence.Split(separators);
    var result = words
        .Where(w => w != "")
        .Where(w => w.Length < 5)
        .OrderBy(w => w)
        .Distinct();
    Console.WriteLine(string.Join(", ", result));
  }
}
```
[/code-editor]
[task-description]Read a **text**, extract its **words**, find all **short words** (less than 5 characters) and print them **alphabetically**, in **lower case**.[/task-description]
[code-io /]
[/code-task]
[/slide]
