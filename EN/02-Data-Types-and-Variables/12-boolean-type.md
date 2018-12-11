[slide]
# Boolean Type
Boolean type is declared with the keyword bool. It has two possible values: true and false. Its default value is false. It is used most often to store the calculation result of logical expressions

```csharp
int a = 1;
int b = 2;
bool greaterAB = (a > b);
Console.WriteLine(greaterAB);  // False
bool equalA1 = (a == 1);
Console.WriteLine(equalA1);    // True
```

[/slide]

[slide]
# Problem: Special Numbers
- A number is special when its sum of digits is 5, 7 or 11
    - For all numbers 1…n print the number and if it is special
```csharp
        1 -> False  8 -> False  15 -> False
        2 -> False  9 -> False  16 -> True
        3 -> False  10 -> False 17 -> False
20 ->   4 -> False  11 -> False 18 -> False
        5 -> True   12 -> False 19 -> False
        6 -> False  13 -> False 20 -> False
        7 -> True   14 -> True
```
Check your solution here: 


[/slide]



[slide]
# Solution: Special Numbers
```csharp
int n = int.Parse(Console.ReadLine());
for (int num = 1; num <= n; num++)
{
  int sumOfDigits = 0;
  int digits = num;
  while (digits > 0)
  {
    sumOfDigits += digits % 10;
    digits = digits / 10;
  }
  bool special = (sumOfDigits == 5) || …; // TODO: finish this
  Console.WriteLine("{0} -> {1}", num, special);
}

```
Check your solution here: 
[/slide]

