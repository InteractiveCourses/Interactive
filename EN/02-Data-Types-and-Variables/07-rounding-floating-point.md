[slide]
# Rounding Floating-Point Numbers
There are different methods to do rounding
- Math.Round(3.45) – round to integer number (mathematically)
- Math.Round(2.3455, 3) – round with precision
- Math.Ceiling() – round up to the nearest integer
- Math.Floor() – round down to the nearest integer

```csharp
double a = 2.3455;
Console.WriteLine(Math.Round(a));    // result: 2
Console.WriteLine(Math.Round(a, 3)); // result: 2.346
Console.WriteLine(Math.Ceiling(a));  // result: 3
Console.WriteLine(Math.Floor(a));    // result: 2
```

[/slide]

[slide]
# Problem: Circle Area (12 Digits Precision)
- Write program to enter a radius r (real number) and prints the area of the circle with exactly 12 digits after the decimal point:
```csharp
2.5 -> 19.634954084936
1.2 -> 4.523893421169
```

- Sample solution:
```csharp
double r = double.Parse(Console.ReadLine());
Console.WriteLine("{0:f12}", Math.PI * r * r);

```

Check your solution here: 


[/slide]