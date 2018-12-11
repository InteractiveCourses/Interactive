[slide]
# Variable Scope and Lifetime
- Scope shows from where you can access a variable
- Lifetime shows how long a variable stays in memory
TODO: picture code
[/slide]

[slide]
# Variable Span
- Variable span is how long before a variable is called
- Always declare a variable as late as possible (e.g. shorter span)
TODO: picture code
[/slide]

[slide]
# Variable Span2
- Variable span is how long before a variable is called
- Always declare a variable as late as possible (e.g. shorter span)
TODO: picture code
[/slide]




[slide]
# Problem: Refactor Special Numbers
```csharp
int kolkko = int.Parse(Console.ReadLine());
int obshto = 0; int takova = 0; bool toe = false;
for (int ch = 1; ch <= kolkko; ch++)
{
    takova = ch;
    while (ch > 0)
    {
        obshto += ch % 10;
        ch = ch / 10;
    }
    toe = (obshto == 5) || (obshto == 7) || (obshto == 11);
    Console.WriteLine($"{takova} -> {toe}");
    obshto = 0; ch = takova;
}
```



Check your solution here: 

[/slide]



