[slide]
# Associative Arrays (Maps, Dictionaries)

- Associative arrays are arrays indexed by keys
    - Not by the numbers 0, 1, 2, …
- Hold a set of pairs {key -> value}

Traditional array:

| 0 | 1  | 2  | 3   | 4  |
|---|----|----|-----|----|
| 8 | -3 | 12 | 408 | 33 |

Associative array:

| key        | value       |
|------------|-------------|
| John Smith | +1-555-8976 |
| Lisa Smith | +1-555-1234 |
| Sam Doe    | +1-555-5030 |

[/slide]

[slide]
# Dictionary<K, V>, SortedDictionary<K, V>

Have property `Count` – the number of key-value pairs.

`Keys` – a set of unique keys:

```csharp
Dictionary<string, int> dict = new Dictionary<string, int>();
foreach (var key in dict.Keys)
{
  Console.WriteLine(key);
}
```

`Values` – a collection of all values:

```csharp
foreach (var value in dict.Values)
{
  Console.WriteLine(value);
}

Basic operations – `Add()`, `Remove()`, `Clear()`.
[/slide]

[slide]
# Dictionary<K, V>, SortedDictionary<K, V> (2)

Boolean methods:

- `ContainsKey()` – checks if a key is present in the dictionary (fast)
- `ContainsValue()` – checks if a value is present in the dictionary (slow)
- `TryGetValue()` – check if a key is present in the dictionary and ouputs the value, or returns the default value of the type.
[/slide]