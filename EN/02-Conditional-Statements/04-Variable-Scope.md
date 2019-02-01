[slide]
# Variable scope

The scope of a variable determines its visibility to the rest of a program.
```csharp
string currentDay = Console.ReadLine(); 
if (currentDay == "Monday") 
{
    double salary = double.Parse(Console.ReadLine());
}
Console.WriteLine(salary); //Compile time error
```

The ***variable salary*** exists only in the ***if*** code block and can't be used anywhere else.
[/slide]