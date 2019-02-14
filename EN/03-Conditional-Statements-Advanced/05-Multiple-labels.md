[slide]
# Using Multiple Labels
sing multiple labels is appropriate, when we want to ***execute the same structure in more than one case***. 
Let’s look at the following example:
[/slide]
[slide]
# Example
[code-task title="Example" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
class Program
{
    static void Main(string[] args)
    {
        string animal = Console.ReadLine();
        switch (animal)
        {
            case "dog":
            case "cat":
                Console.WriteLine("mammal");
                break;
            case "crocodile":
            case "tortoise":
            case "snake":
                Console.WriteLine("reptile");
                break;
            default:
                Console.WriteLine("unknown");
                break;
        }
    }
}
```
[/code-editor]
[task-description]
[/task-description]
[code-io /]
[/code-task]
[/slide]