[slide]
# Real Number Types
- Floating-point types:
    - Represent real numbers, e.g. 1.25, -0.38
    - Have range and precision depending on the memory used
    - Sometimes behave abnormally in the calculations
    - May hold very small and very big values like 0.00000000000001 and 10000000000000000000000000000000000.0

[/slide]

[slide]
# Floating-Point Numbers
- Floating-point types are:
    - float (±1.5 × 10−45 to ±3.4 × 1038)
        - 32-bits, precision of 7 digits
    - double (±5.0 × 10−324 to ±1.7 × 10308)
        - 64-bits, precision of 15-16 digits
- The default value of floating-point types:
    - Is 0.0F for the float type
    - Is 0.0D for the double type

[/slide]

[slide]
# PI Precision – Example
- Difference in precision when using float and double:

```csharp
float floatPI = 3.141592653589793238f;
double doublePI = 3.141592653589793238;
Console.WriteLine("Float PI is: {0}", floatPI);
Console.WriteLine("Double PI is: {0}", doublePI);

```
- NOTE: The "f" suffix in the first statement!
    - Real numbers are by default interpreted as double!
    - One should explicitly convert them to float
[/slide]