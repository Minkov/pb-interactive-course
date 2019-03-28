# Introduction
[slide]
# Welcome to SoftUni
[image src="https://interactive-platform.serveo.net/platform/assets/icons/logo.svg" /]
[youtube-video videoId=WD33ii01kXI /]
[/slide]

[slide]
# Video
[youtube-video videoId=rtczBseiAac /]
[/slide]

[slide]
# Hello World!
[code-task title="Hello World" executionStrategy="csharp-dot-net-core-code"]
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
This is a simple program, written in C#, that prints "Hello World!" as an output.
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Explanation
Let's go through the program line by line.
- ***class Program{...}***

The above statement creates a class named - Program. C# is an object-oriented programming language, creating a class is mandatory for the program's execution.
 
- ***static void Main(){...}***

Main() is a method of class Program. The execution of every C# program starts from the Main() method.

We'll learn more about methods in the later lectures.
 
- ***System.Console.WriteLine("Hello World!");***

For now, remember this is the piece of code that prints "Hello World!" to the output screen. 

You'll learn more about how it works in the later lectures.
[/slide]

[slide]
# Task
[code-task title="Greeting" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp] 
```
using System;
public class Program
{
    public static void Main()
    {
        string name = Console.ReadLine();
        // Write your code here
    }
}
```
[/code-editor]
[task-description]Write a program that reads a name from the Console and greets the person in the following format: "Hello {name}!". 

Hint: You can use "+" sign to join to strings.
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution

[code-task title="Greeting" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
    public static void Main()
    {
        string name = Console.ReadLine();
        Console.WriteLine("Hello " + name + "!");
    }
}
```
[/code-editor]
[task-description]
Write a program that reads a name from the Console and greets the person in the following format: "Hello {name}!". 

Hint: You can use "+" sign to join to strings.
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Explanation - Namespaces
You see that above the class there is ***using System;***

System is a Namespace. Namespaces are used in C# to organize and provide a level of separation of codes. 

They can be considered as a container which consists of other namespaces, classes, etc.

So after we are using the System Namespace, we can just type ***Console.WriteLine()***. That is because Console is a member of the System Namespace.

You will learn more about Namespaces in the following lectures.
[/slide]

[slide]
# Explanation - Concatenation

When we read the input from the console and store it in the variable ***name***, we print a line on the console as a result.
We are using a method of the class Console, just like ***ReadLine()***, but now printing, rather than reading - ***PrintLine()***.

The line consist of the text "Hello " which is concatenated with the value of the variable ***name*** and "!". 

When we are using "+" sign between 2 parts of text, called strings, we are concatenating them, not adding them together.

We are going to learn about strings and different data types in the following sections.
[/slide]
