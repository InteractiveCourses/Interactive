[slide]
# Decimal Floating-Point Type
- There is a special decimal floating-point real number type in C#:
    - decimal (±1,0 × 10-28 to ±7,9 × 1028)
        - 128-bits, precision of 28-29 digits
    - Used for financial calculations
    - Almost no round-off errors
    - Almost no loss of precision
- The default value of decimal type is:
    - 0.0M (M is the suffix for decimal numbers)

[/slide]

[slide]
# Problem: Exact Sum of Real Numbers
- Write program to enter n numbers and print their exact sum:
```csharp
2
1000000000000000000
5

```
1000000000000000005
```

```
Check your solution here: 

[/slide]

[slide]
# Solution: Exact Sum of Real Numbers
- This code works but makes mistakes sometimes:

```csharp
int n = int.Parse(Console.ReadLine());
double sum = 0;
for (int i = 0; i < n; i++)
  sum += double.Parse(Console.ReadLine());
Console.WriteLine(sum);

```
- Change double with decimal and check the differences

Check your solution here: 

[/slide]


