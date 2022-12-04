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

## Resources

- [Dart Null Safety](https://dart.dev/null-safety)
- [Understanding Null Safety](https://dart.dev/null-safety/understanding-null-safety)
- [Sound Null Safety](https://dart.dev/null-safety#:~:text=Null%20safety%20prevents%20errors%20that,can%20be%20difficult%20to%20debug.)
