# Infinite For Loop
[slide]
# Definition
An infinite loop is a piece of coding that lacks an exit condition so the loop repeats indefinitely. Infinite loop is **rarely needed** and should be **avoided**.
[/slide]

[slide]
# Video
[youtube-video videoId=Hxbz656Euyw /]
[/slide]

[slide]
# Example
```cs
for (int i = 1 ; i > 0; i++)
{
    Console.WriteLine("Iteration {0}", i);
}

We can also create an infinite loop by replacing the condition with a blank. For example:
```csharp
for ( ; ; )
{
	// body of for loop
}
```

or 

```csharp
for (initialization ; ; iterator)
{
	// body of for loop
}
```
[/slide]

[slide]
# Summary
[/slide]
