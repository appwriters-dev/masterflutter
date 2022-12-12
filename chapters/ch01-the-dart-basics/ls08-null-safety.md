---
id: ls08-null-safety
title: Null Safety in Dart
description: Null safety is a Dart programming language feature that prevents null reference exceptions by preventing variables from being null unless explicitly allowed. This is accomplished by using nullable and non-nullable types, which allow developers to specify whether or not a variable can be null.
---

Null safety is a Dart programming language feature that prevents null reference exceptions by preventing variables from being null unless explicitly allowed. This is accomplished by using nullable and non-nullable types, which allow developers to specify whether or not a variable can be null.

Dart's null safety ensures that by default, all variables have a non-null value. If a variable must be nullable, the? operator must be used to explicitly declare it as such. This makes reasoning about the code easier and helps to avoid null reference exceptions, which can be difficult to track down and fix.

Furthermore, null safety supports the?? operator, which allows developers to specify a default value to use if a nullable variable is null. This simplifies and improves code readability by eliminating the need for null check statements.

Overall, null safety is a useful Dart feature that helps improve code reliability and safety. It enables developers to explicitly declare whether a variable can be null or not, and it supports dealing with null values in a safe and concise manner.

Null safety is a Dart programming language feature that prevents null reference exceptions by ensuring that variables cannot be null unless explicitly permitted. This is accomplished by using nullable and non-nullable types, which allow developers to specify whether or not a variable can be null. Null safety also supports the?? operator, which allows developers to specify a default value that will be used if a nullable variable is null. Overall, null safety is a useful Dart feature that helps improve code reliability and safety.

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

- [Null Safety](https://dart.dev/null-safety)
- [Understanding Null Safety](https://dart.dev/null-safety/understanding-null-safety)
- [Null Safety Codelab](https://dart.dev/codelabs/null-safety)
- [Null Safety Ultimate Guide](https://codewithandrea.com/videos/dart-null-safety-ultimate-guide-non-nullable-types/)
