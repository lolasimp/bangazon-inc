# Planet and Spaceships

## Setup

```
mkdir -p ~/workspace/csharp/exercises/lists && cd $_
dotnet new console
dotnet restore
```

## Reference

* [C# Lists](https://msdn.microsoft.com/en-us/library/6sh2ey19(v=vs.110).aspx)
* [Interactive C# Lists](http://www.learncs.org/en/Lists)

## Exercise

In the `Main` method, place the following code

```cs
List<string> planetList = new List<string>(){"Mercury", "Mars"};
```

1. `Add()` Jupiter and Saturn at the end of the list.
1. Create another `List` that contains that last two planet of our solar system.
1. Combine the two lists by using `AddRange()`.
1. Use `Insert()` to add Earth, and Venus in the correct order.
1. Use `Add()` again to add Pluto to the end of the list.
1. Now that all the planets are in the list, slice the list using `GetRange()` in order to extract the rocky planets into a new list called `rockyPlanets`.
1. Being good amateur astronomers, we know that Pluto is now a dwarf planet, so use the `Remove()` method to eliminate it from the end of `planetList`.

## Iterating over planets

> **Ref:** [List of Solar System probes](https://en.wikipedia.org/wiki/List_of_Solar_System_probes)

1. Create another dictionary that will hold the name of a spacecraft that we have launched, and a list of names of the planets that it has visited. Remember that `List` is a Type just like native types (such as `string`, `int`, & `bool`) and your custom types (such as `Movie`, `Dog`, and `Food`). They can be passed to anything, like a dictionary, as a Type.
1. Iterate over your list of planets from above, and inside that loop, iterate over the dictionary. Write to the console, for each planet, which satellites have visited which planet.

```sh
Mars: Viking, Opportunity, Curiosity
Venus: Mariner, Venera

etc...
```
