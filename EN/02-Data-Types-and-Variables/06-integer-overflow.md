<<<<<<< HEAD:EN/02-Data-Types-and-Variables/06-integer-overflow.md
[slide]
# Beware of Integer Overflow!
- Integers have range (minimal and maximal value)
- Integers could overflow -> this leads to incorrect values
```csharp
byte counter = 0;
for (int i = 0; i < 260; i++)
{
  counter++;
  Console.WriteLine(counter);
}

```

```csharp
1
2
…
255
0
1
```
[/slide]

[slide]
# Problem: Centuries to Minutes
- Write program to enter an integer number of centuries and convert it to years, days, hours and minutes

```csharp
Centures = 1
1 centuries = 100 years = 36524 days = 876576 hours = 52594560 minutes
```csharp

```csharp
Centures = 5
5 centuries = 500 years = 182621 days = 4382904 hours = 262974240 minutes
```
Check your solution here:

[/slide]

[slide]
# Solution: Centuries to Minutes
```csharp
Console.Write("Centuries = ");
int centuries = int.Parse(Console.ReadLine());
int years = centuries * 100;
int days = (int) (years * 365.2422); 
int hours = 24 * days;
int minutes = 60 * hours;
Console.WriteLine("{0} centuries = {1} years = {2} days = {3} hours = {4} minutes", centuries, years, days, hours, minutes);

```
Check your solution here: 

[/slide]
=======
[slide]
# Beware of Integer Overflow!
- Integers have range (minimal and maximal value)
- Integers could overflow -> this leads to incorrect values
```csharp
byte counter = 0;
for (int i = 0; i < 260; i++)
{
  counter++;
  Console.WriteLine(counter);
}

```

```csharp
1
2
…
255
0
1
```
[/slide]

[slide]
# Problem: Centuries to Minutes
- Write program to enter an integer number of centuries and convert it to years, days, hours and minutes

```csharp
Centures = 1
1 centuries = 100 years = 36524 days = 876576 hours = 52594560 minutes
```csharp

```csharp
Centures = 5
5 centuries = 500 years = 182621 days = 4382904 hours = 262974240 minutes
```
Check your solution here:

[/slide]

[slide]
# Solution: Centuries to Minutes
```csharp
Console.Write("Centuries = ");
int centuries = int.Parse(Console.ReadLine());
int years = centuries * 100;
int days = (int) (years * 365.2422); 
int hours = 24 * days;
int minutes = 60 * hours;
Console.WriteLine("{0} centuries = {1} years = {2} days = {3} hours = {4} minutes", centuries, years, days, hours, minutes);

```
Check your solution here: 

[/slide]
>>>>>>> 7ec58516592b9ae83b26abd3b22d745f595eddea:EN/02-Data-Types-and-Variables/06-integer-overflow.md
