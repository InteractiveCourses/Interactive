[slide]
# Problem: Get Folder Size
- You are given a folder named “TestFolder”. Get the size of all files in the folder, which are **NOT directories**. Print the result on the console in **Megabytes**.


```csharp
Output
5.16173839569092
```


Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/322#5]https://judge.softuni.bg/Contests/Practice/Index/322#5[/anchor]

[/slide]

[slide]
# Solution: Get Folder Size
```csharp
string[] files = Directory.GetFiles("TestFolder");
double sum = 0;

foreach (string file in files)   
{
	FileInfo fileInfo = new FileInfo(file);
 	sum += fileInfo.Length;
}

sum = sum / 1024 / 1024;

File.WriteAllText("оutput.txt", sum.ToString());
```

Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/322#5]https://judge.softuni.bg/Contests/Practice/Index/322#5[/anchor]
[/slide]

[slide]
# Try it yourself!

[code-task title="Problem: Get Folder Size" executionStrategy="csharp-dot-net-core-code" requiresInput]

[code-editor language=csharp]
```
using System;

namespace App
{
    class Program
    {
        static void Main(string[] args)
        {
		    // enter your code here
		    
		}
	}
}
```
[/code-editor]

[task-description]
You are given a folder named “TestFolder”. Get the size of all files in the folder, which are NOT directories. Print the result on the console in Megabytes. 
[/task-description]

[code-io /]
[/code-task]
[/slide]