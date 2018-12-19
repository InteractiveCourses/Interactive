[slide]
# Dictionary<K, V> – Add()

The key is hashed, and the value is put in a location depending on the hash value.

To retrieve the value, the same process is repeated (the key is hashed, and the value is retrieved from the location pointed by the hash).
[/slide]

[slide]
# Dictionary<K, V> – Remove()

The key is hashed, and if there's a value at the location pointed by the hash, it's removed.
[/slide]

[slide]
# Looping through dictionaries

```csharp
foreach (KeyValuePair<string, string> kvp in dict)
{
  Console.WriteLine(kvp.Key);
  Console.WriteLine(kvp.Value);
}
```
[/slide]

[slide]
# Phonebook - Dictionary Example

```csharp
var phonebook = new Dictionary<string, string>();

phonebook["John Smith"] = "+1-555-8976";
phonebook["Lisa Smith"] = "+1-555-1234";
phonebook["Sam Doe"] = "+1-555-5030";
phonebook["Giovani"] = "+359-899-555-592";
phonebook["Peter"] = "+359-2-981-9819";

phonebook.Remove("John Smith");

foreach (KeyValuePair<string, string> pair in phonebook)
{
  Console.WriteLine("{0} --> {1}", pair.Key, pair.Value);
}
```

[/slide]