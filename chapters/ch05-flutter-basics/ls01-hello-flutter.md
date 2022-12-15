---
id: ls01-hello-flutter
title: Hello Flutter
---

In this first lesson we will learn to get started with Flutter framework.

## Projects

### 1. Hello Flutter

Head over to [Dartpad](https://dartpad.dev/) and create a New Pad and choose Flutter. Clear everything in the editor and paste the following code.

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(
    Center(
      child: Text(
        'Hello, Flutter!',
        style: TextStyle(color: Color(0xffffffff)),
        textDirection: TextDirection.ltr,
      ),
    ),
  );
}
```

### 2. Install Flutter

Head over to [Flutter Installation guide](https://flutter.dev/docs/get-started/install), choose your operating system, and follow the instructions to install Flutter on your machine. Use `flutter doctor` command to verify that everything is setup correctly.

### 3. Install Visual Studio Code and Flutter Extension

Head over to [Visual Studio Code](https://code.visualstudio.com/) and download the latest version of Visual Studio Code for your operating system. If you already have Visual Studio Code installed, install the Flutter extension from the [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=Dart-Code.flutter).

### 4. Hello Again Flutter

Create new Flutter project in Visual Studio Code. Open the `main.dart` file and replace the code with the following code. Now run the code in web and desktop (also on mobile if you have Android or iOS setup)

```dart
import 'package:flutter/material.dart';

void main() {
  runApp(
    Center(
      child: Text(
        'Hello, Flutter!',
        style: TextStyle(color: Color(0xffffffff)),
        textDirection: TextDirection.ltr,
      ),
    ),
  );
}
```

## Resources

- [Flutter](https://flutter.dev/)
- [Dartpad](https://dartpad.dev/)
- [Flutter Installation guide](https://flutter.dev/docs/get-started/install)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=Dart-Code.flutter)
- [Flutter doctor](https://flutter.dev/docs/reference/flutter-cli#flutter-doctor)
