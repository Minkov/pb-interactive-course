[slide]
# Welcome to SoftUni
[image src="http://link-to-image" /]
[/slide]

[slide]
# Video
[youtube-video videoId=0f7c9RIZGaE /]
[/slide]

[slide]
# Task
[code-task title="Hello" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp] 
```
using System;
public class App
{
    public static void Main()
    {
        string name = Console.ReadLine();
        // Write your code here
    }
}
```
[/code-editor]
[task-description]Write a program that reads a name from the Console and greets the user.[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution
```
using System;
public class App
{
    public static void Main()
    {
        string name = Console.ReadLine();
        Console.WriteLine("Hello " + name + "!");
    }
}
```
[/slide]

[slide]

[/slide]