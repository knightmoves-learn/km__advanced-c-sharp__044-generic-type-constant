# 044 Generic Type Constant 

## Lecture

NO VIDEO ON YOUTUBE CURRENTLY
[![# Null Coalescing Operator)](https://img.youtube.com/vi/v1dbW26xRQQ/0.jpg)](https://www.youtube.com/watch?v=v1dbW26xRQQ)

## Instructions

- In `HomeEnergyApi/Models/IUserRepository.cs`
  - Create a new default interface method on `IUserRepository` named `UserIsAdmin()` with a return type of `bool` and taking one argument of type `string`
    - `UserIsAdmin()` should return true if the provided string is equal to `"Admin"` or false otherwise
- In `HomeEnergyApi/Controllers/AuthenticationControllerV2.cs`
  - Modify the `Register()` method so that...
    - `Ok("Admin registered successfully.")` is returned in the case of `userRepository.UserIsAdmin()` returns true with the user's `Role` as the passed argument
    - `Ok("User is registered successfully.")` is returned otherwise

## Additional Information

- Do not remove or modify anything in `HomeEnergyApi.Tests`
- Some Models may have changed for this lesson from the last, as always all code in the lesson repository is available to view
- Along with `using` statements being added, any packages needed for the assignment have been pre-installed for you, however in the future you may need to add these yourself

## Building toward CSTA Standards:

## Resources
- https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/generics/constraints-on-type-parameters

Copyright &copy; 2025 Knight Moves. All Rights Reserved.
