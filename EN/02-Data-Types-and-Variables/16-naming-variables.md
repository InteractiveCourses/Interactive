[slide]
# Naming Variables
- Variable names
    - Always refer to the naming conventions of a programming language – for C# use camelCase
    - Preferred form: [Noun] or [Adjective] + [Noun]
    - Should explain the purpose of the variable (Always ask yourself "What this variable contains?")

```csharp
Good variable names
firstName, report, config, usersList, fontSize, maxSpeed

Bad variable names
foo, bar, p, p1, p2, populate, LastName, last_name, LAST_NAME
```

[/slide]



[slide]
# Problem: Refactor Volume of Pyramid
- You are given a working code that finds the volume of a prism: 
    - Fix naming, span and multi-purpose variables
```csharp
double dul, sh, V = 0;
Console.Write("Length: ");
dul = double.Parse(Console.ReadLine());
Console.Write("Width: ");
sh = double.Parse(Console.ReadLine());
Console.Write("Height: ");
V = double.Parse(Console.ReadLine());
V = (dul * sh * V) / 3;
Console.WriteLine("Pyramid Volume: {0:F2}", V);
```

Check your solution here: 

[/slide]



