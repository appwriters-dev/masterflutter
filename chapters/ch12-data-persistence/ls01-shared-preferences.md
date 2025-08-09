---
id: ls01-shared-preferences
title: Shared Preferences
description: In this lesson, we will learn how to use shared preferences to store simple data.
---

## What are Shared Preferences?

Shared preferences are a way to store simple data in a key-value format. It is a good way to store simple data like user settings, or a flag to indicate if the user has seen the intro screen.

To use shared preferences, you need to add the `shared_preferences` package to your `pubspec.yaml` file:

```yaml
dependencies:
  shared_preferences: ^2.0.0
```

## Projects

### 1. Simple Counter with Shared Preferences

Create a simple counter app that saves the count to shared preferences. When the app is restarted, the count should be loaded from shared preferences.

Here is an example of how you can implement this:

```dart
import 'package:flutter/material.dart';
import 'package:shared_preferences/shared_preferences.dart';

class CounterApp extends StatefulWidget {
  @override
  _CounterAppState createState() => _CounterAppState();
}

class _CounterAppState extends State<CounterApp> {
  int _count = 0;
  late SharedPreferences _prefs;

  @override
  void initState() {
    super.initState();
    _loadCounter();
  }

  void _loadCounter() async {
    _prefs = await SharedPreferences.getInstance();
    setState(() {
      _count = _prefs.getInt('counter') ?? 0;
    });
  }

  void _increment() {
    setState(() {
      _count++;
    });
    _prefs.setInt('counter', _count);
  }

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      home: Scaffold(
        appBar: AppBar(
          title: Text('Counter App with Shared Preferences'),
        ),
        body: Center(
          child: Text(
            '$_count',
            style: Theme.of(context).textTheme.headline4,
          ),
        ),
        floatingActionButton: FloatingActionButton(
          onPressed: _increment,
          child: Icon(Icons.add),
        ),
      ),
    );
  }
}

void main() {
  runApp(CounterApp());
}
```

## Resources

- [Shared Preferences package](https://pub.dev/packages/shared_preferences)
- [Persist data with shared preferences](https://flutter.dev/docs/cookbook/persistence/key-value)
