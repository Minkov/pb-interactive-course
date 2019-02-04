# Variables

[slide]
# Definition
A variable is a symbolic name given to a memory location. 
Variables are used to store data in a computer program.
You can imagine the variable as a box with a content. Like in the real world, the box can be empty or store a value. 
There are different types of variables, as we are going to learn in the next section.
[/slide]

[slide]
# Video
[youtube-video videoId=Hxbz656Euyw /]
[/slide]

[slide]
# Declaring Variables
In C# we declare variables, using the following format:
```
{data type} {variable name} = {value};
```
- The data type can be any primitive data type or, as we are going to learn in future lectures and courses, we can define our own custom data types.
- the variable name should make sense 

Variables in C# must be declared before they can be used. This means, the name and type of variable must be known before they can be assigned a value. 

[/slide]

[slide]
# Best Practices

1. Choose a variable name that make sense. For example, name, age, subject makes more sense than n, a and s.
2. Use camelCase notation (starts with lowercase letter) for naming local variables. For example, numberOfStudents, age, etc.
3. Use PascalCase or CamelCase (starts with uppercase letter) for naming public member variables. For example, FirstName, Price, etc.
4. Use a leading underscore (_) followed by camelCase notation for naming private member variables. For example, _bankBalance, _emailAddress, etc.
You can learn more about naming conventions in C# [here](https://docs.microsoft.com/en-us/dotnet/standard/design-guidelines/naming-guidelines).

[/slide]


[slide]
# Summary
Variable = Box
[/slide]