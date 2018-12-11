[slide]
# Type Conversion
Because C# is statically-typed at compile time, after a variable is declared, it cannot be declared again or assigned a value of another type unless that type is implicitly convertible to the variable's type. However, you might sometimes need to copy a value into a variable or method parameter of another type. 

- Variables hold values of certain type
- Type can be changed (converted) to another type
    - Implicit type conversion (lossless): variable of bigger type (e.g. double) takes smaller value (e.g. float)
```csharp
float heightInMeters = 1.74f;
double maxHeight = heightInMeters; // Implicit conversion

```
- Explicit type conversion (lossy) – when precision can be lost:
```csharp
double size = 3.14;
int intSize = (int) size; // Explicit conversion -> 3
```
[/slide]

[slide]
# Problem: Elevator
- Calculate how many courses will be needed to elevate n persons by using an elevator of capacity of p persons

```csharp
persons = 17
capacity = 3

```

```csharp
6 courses
How? 5 courses /* 3 persons + 1 course /* 2 persons

```

- Sample solution:
```csharp
int n = int.Parse(Console.ReadLine());
int p = int.Parse(Console.ReadLine());
int courses = (int) Math.Ceiling((double)n / p);
Console.WriteLine(courses);

```
Check your solution here: 
[/slide]

