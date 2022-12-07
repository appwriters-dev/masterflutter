---
id: ls08-null-safety
title: Null Safety in Dart
---

Null safety helps us write more stable programs. So it's important to understand null safety in
Dart. The Dart programming language includes sound null safety. Null safety guards against errors
caused by unintentional access to variables set to null. If a method expects an integer but receives
null, your app generates a runtime error. This type of error, known as a null dereference error, can
be difficult to troubleshoot.

By flagging when any non-nullable variable hasn't been initialized with a non-null value or is being
assigned a null, sound null safety converts potential runtime errors into edit-time analysis errors.
This enables you to correct these issues before deploying your app.

## Projects

### 1. Basic Null Safety

Create a simple program that declares and initializes a few variables, including some that are nullable and some that are non-nullable. 
     
### 2. Null coalescing operator (??)

Write a function that accepts optional `String` parameter and returns the value of the parameter if it is not null, otherwise it returns the string "Default value" using the null coalescing operator.

### 3. late

Write a program by using late modifier and assign values that and print final variable.

## Remember things : 

- When possible, try to create non-nullable variables, which are guaranteed not to be null at compile time.
- If you know a nullable expression will not be null, you can use the ! operator to assign it to a non-nullable variable.

## Resources

- [Dart Null Safety](https://dart.dev/null-safety)
- [Understanding Null Safety](https://dart.dev/null-safety/understanding-null-safety)
- [Sound Null Safety](https://dart.dev/null-safety#:~:text=Null%20safety%20prevents%20errors%20that,can%20be%20difficult%20to%20debug.)
- [Practice courses](https://codewithandrea.com/videos/dart-null-safety-ultimate-guide-non-nullable-types/)
