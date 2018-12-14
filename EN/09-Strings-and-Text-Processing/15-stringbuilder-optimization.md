[slide]
# StringBuilder Optimization

- Given the code below try to **optimize** it to go under 10 secs. 
    - Do **not** change the loop nor the Convert.ToString() method

```c#
string result = "";
Stopwatch st = new Stopwatch();
st.Start();
for(int i = 0; i < 50000; i++)
    {
        result += (Convert.ToString(i,2) + "\n");
    }
    
    st.Stop();
    Console.WriteLine(st.Elapsed);
```
 

[/slide]



[slide]
# Try it yourself!

[code-task title="Try it yourself!" executionStrategy="csharp-dot-net-core-code" requiresInput]

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
Test your code.
[/task-description]

[code-io /]
[/code-task]


[/slide]


