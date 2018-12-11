[slide]
# Strings

## What is a String?
A string is a sequence of characters stored in a certain address in memory. Remember the type char? In the variable of type char we can record only one character. Where it is necessary to process more than one character then strings come to our aid.

- Strings are represented by System.String objects in .NET Framework. The class **System.String** enables us to handle strings in C#. For declaring the strings we will continue using the keyword string, which is an alias in C# of the System.String class from .NET Framework. The work with string facilitates us in manipulating the text content: construction of texts, text search and many other operations.
- String objects contain an immutable (read-only) sequence of characters. The string class has an important feature – the character sequences stored in a variable of the class are never changing. After being assigned once, the content of the variable does not change directly – if we try to change the value, it will be saved to a new location in the dynamic memory and the variable will point to it. Since this is an important feature, it will be illustrated later.

## Let’s Begin!

[/slide]