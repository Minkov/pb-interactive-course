[slide]
# Welcome to SoftUni
[image src="http://link-to-image" /]
[/slide]

[slide]
# Video
[youtube-video videoId=0f7c9RIZGaE /]
[/slide]

[slide]
# Hello World!
[code-task title="" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
public class Program {         
    public static void Main()
    {
        System.Console.WriteLine("Hello World!");
    }
}
```
[/code-editor]
[task-description]
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Explanation
Let's go through the program line by line.
* `class Program{...}`
The above statement creates a class named - Program. C# is an object-oriented programming language, creating a class is mandatory for the program's execution.
 
* `static void Main(){...}`

Main() is a method of class Program. The execution of every C# program starts from the Main() method.
We'll learn more about methods in the later lectures.
 
* `System.Console.WriteLine("Hello World!");`

For now, remember this is the piece of code that prints Hello World! to the output screen. You'll learn more about how it works in the later lectures.
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
[task-description]Write a program that reads a name from the Console and greets the person.[/task-description]
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
# Explanation
[/slide]
