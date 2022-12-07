---
id: ls08-null-safety
title: Null Safety in Dart
description: Null safety is a feature of the Dart programming language that prevents null reference exceptions by ensuring that variables cannot be null unless explicitly allowed. This is achieved through the use of nullable and non-nullable types, which allow developers to specify whether a variable can be null or not.
---

Null safety is a feature of the Dart programming language that prevents null reference exceptions by ensuring that variables cannot be null unless explicitly allowed. This is achieved through the use of nullable and non-nullable types, which allow developers to specify whether a variable can be null or not.

With null safety, Dart guarantees that all variables have a non-null value by default. If a variable needs to be nullable, it must be explicitly declared as such using the ? operator. This makes it easier to reason about the code and avoid null reference exceptions, which can be difficult to track down and fix.

Additionally, null safety provides support for the ?? operator, which allows developers to specify a default value to use if a nullable variable is null. This simplifies code and makes it more readable, as it eliminates the need for null check statements.

Overall, null safety is a useful feature of Dart that helps improve the reliability and safety of code. It allows developers to explicitly declare whether a variable can be null or not, and provides support for handling null values in a safe and concise manner.

In summary, null safety is a feature of the Dart programming language that prevents null reference exceptions by ensuring that variables cannot be null unless explicitly allowed. This is achieved through the use of nullable and non-nullable types, which allow developers to specify whether a variable can be null or not. Null safety also provides support for the ?? operator, which allows developers to specify a default value to use if a nullable variable is null. Overall, null safety is a useful feature of Dart that helps improve the reliability and safety of code.

## Projects

### 1. Basic Null Safety

Create a simple program that declares and initializes a few variables, including some that are nullable and some that are non-nullable. 
     
### 2. Null coalescing operator (??)

Write a function that accepts optional `String` parameter and returns the value of the parameter if it is not null, otherwise it returns the string "Default value" using the null coalescing operator.

### 3. late

Write a program by using late modifier and assign values that and print final variable.

## Remember things

- When possible, try to create non-nullable variables, which are guaranteed not to be null at compile time.
- If you know a nullable expression will not be null, you can use the ! operator to assign it to a non-nullable variable.

## Resources

- [Dart Null Safety](https://dart.dev/null-safety)
- [Understanding Null Safety](https://dart.dev/null-safety/understanding-null-safety)
- [Sound Null Safety](https://dart.dev/null-safety#:~:text=Null%20safety%20prevents%20errors%20that,can%20be%20difficult%20to%20debug.)
- [Practice courses](https://codewithandrea.com/videos/dart-null-safety-ultimate-guide-non-nullable-types/)
