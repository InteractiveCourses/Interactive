[slide]
# Extracting Substrings
For now we know how to check whether a substring occurs in a text and which are the occurrence positions. But how can we extract a substrings of a string in a separate variable? 
The solution of this problem is the method **Substring(…)**. By using it, we can **extract** a part of the string (substring) by a given **starting position** in the text and its **length**. If the length is omitted, a portion from the text will be extracted, starting from the initial position to the string’s end.
- Extracting substrings
    - str.Substring(int startIndex, int length)


```csharp
string filename = @"C:\Pics\Rila2005.jpg";
string name = filename.Substring(8, 8);
// name is Rila2005

```
    - str.Substring(int startIndex)

```csharp
string filename = @"C:\Pics\Summer2009.jpg";
string nameAndExtension = filename.Substring(8);
// nameAndExtension is Summer2009.jpg

```
## Try it yourself!


[/slide]


