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

### 1. Use ? non-nullable operator
    Write a program which containing fullName,address and phoneNumber with non-nullable iniliazation and add values for given parameter inside build context or init method and then print parameter.
     
### 2. Use ! operator
     Write a program which have multiple parameter like above project 1 and guarented that values are not null by using ! operator ,and print that parameter .

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
