[slide]
# Floating-Point Division & Abnormalities
## Floating-Point Division
- Integral division and floating-point division are different:
```csharp
Console.WriteLine(10 / 4);    // 2 (integral division)
Console.WriteLine(10 / 4.0);  // 2.5 (real division)
Console.WriteLine(10 / 0.0);  // Infinity
Console.WriteLine(-10 / 0.0); // -Infinity
Console.WriteLine(0 / 0.0);   // NaN (not a number)
Console.WriteLine(8 % 2.5);   // 0.5 (3 * 2.5 + 0.5 = 8)
int d = 0;             // Integral division works differently
Console.WriteLine(10 / d); // DivideByZeroException
```

## Floating-Point Calculations – Abnormalities
- Sometimes floating-point numbers work incorrectly!
```csharp
Console.WriteLine(100000000000000.0 + 0.3);
// Result: 100000000000000 (loss of precision)
double a = 1.0f, b = 0.33f, sum = 1.33;
Console.WriteLine("a+b={0} sum={1} equal={2}",
  a+b, sum, (a+b == sum));
// a+b=1.33000001311302 sum=1.33 equal=False
double one = 0;
for (int i = 0; i < 10000; i++) one += 0.0001;
Console.WriteLine(one); // 0.999999999999906
```

[/slide]

