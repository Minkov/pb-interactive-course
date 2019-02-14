# For Definition

[slide]

# Definition
The **for** keyword is used to create for loop in C#. The syntax for **for loop** is:
```csharp
for (initialization; condition; iterator)
{
	// body of for loop
}
```

## Initialization
Executed at first and only once. Here, the variable is usually declared and initialized

## Condition
Boolean expression, i.e. it returns either ***true*** or ***false***.
    - If the condition is evaluated to true the statements inside the for loop are executed, then, the iterator statement is executed which usually changes the value of the initialized variable and finally the condition is evaluated again.
    - If the condition is evaluated to false, the for loop ***terminates***.

## Iterator
Executed at each iteration, after the loop's body has been executed. It is most commonly used to update the value of the counter-variable.

## The Body of the Loop
The body of the loop contains a block with source code. The loop variables, declared in the initialization block of the loop are available in it. The body is executed at each iteration.
[/slide]

[slide]
# Video
[youtube-video videoId=Hxbz656Euyw /]
[/slide]

[slide]
# For Loop Example
```csharp
for (int i = 1; i <= 5; i += 1)
{
    Console.WriteLine(i);
}
```

When we run the program, the output will be:
```
1
2
3
4
5
```
[/slide]

[slide]
# Explanation
In this program:
- initialization statement is int i = 1
- condition statement is i <= 5
- iterator statement is i += 1
    - The iterator statement could be anything that updates the initialized variable, but the actual result will be different. For example:
        - i += 2;
        - i += 3;
        - i += 5; 
[/slide]

[slide]
# Summary
[/slide]