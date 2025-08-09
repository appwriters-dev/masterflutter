---
id: ls03-hive
title: Hive
description: In this lesson, we will learn how to use Hive to store data.
---

## What is Hive?

Hive is a lightweight and blazing fast key-value database written in pure Dart. It is a good alternative to SQLite for storing structured data.

To use Hive, you need to add the `hive` and `hive_flutter` packages to your `pubspec.yaml` file:

```yaml
dependencies:
  hive: ^2.0.0
  hive_flutter: ^1.0.0
```

You will also need to add `hive_generator` and `build_runner` to your `dev_dependencies`:

```yaml
dev_dependencies:
  hive_generator: ^1.0.0
  build_runner: ^2.0.0
```

## Projects

### 1. Simple To-Do App with Hive

Re-create the to-do app from the previous lesson, but this time use Hive to store the data.

Here is an example of how you can implement this:

```dart
import 'package:flutter/material.dart';
import 'package:hive/hive.dart';
import 'package:hive_flutter/hive_flutter.dart';

part 'main.g.dart';

@HiveType(typeId: 1)
class Todo {
  @HiveField(0)
  String title;

  @HiveField(1)
  bool completed;

  Todo({required this.title, this.completed = false});
}

void main() async {
  await Hive.initFlutter();
  Hive.registerAdapter(TodoAdapter());
  await Hive.openBox<Todo>('todos');
  runApp(MyApp());
}

// ... more code for the app
```

## Resources

- [Hive package](https://pub.dev/packages/hive)
- [Hive documentation](https://docs.hivedb.dev/)
