# Unexpected Object Reference Behavior in C#

This repository demonstrates a common C# pitfall related to object references.  When assigning an object to a new variable, it's crucial to understand that you are not creating a copy of the object; rather, you are creating a second reference to the same object in memory.  Modifications made through one reference are reflected in all others.

The `bug.cs` file shows a simple example where altering an object's property through one reference also modifies it through another reference. The solution in `bugSolution.cs` demonstrates how to create a deep copy if you need independent object instances.

This example is helpful in understanding the importance of differentiating between value types and reference types in C# and how to manage them effectively to prevent unexpected behavior.