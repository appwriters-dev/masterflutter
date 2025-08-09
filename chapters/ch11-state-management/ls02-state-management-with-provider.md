---
id: ls02-state-management-with-provider
title: State Management with Provider
description: In this lesson, we will learn about state management with Provider.
---

## What is Provider?

Provider is a wrapper around `InheritedWidget` that makes it easier to use and more reusable. It is the recommended way to manage state for apps of any scale.

To use Provider, you need to add the `provider` package to your `pubspec.yaml` file:

```yaml
dependencies:
  provider: ^6.0.0
```

## Projects

### 1. Counter App with Provider

Re-create the counter app from the previous lesson, but this time use Provider to manage the state.

Here is an example of how you can implement this:

```dart
import 'package:flutter/material.dart';
import 'package:provider/provider.dart';

class Counter with ChangeNotifier {
  int _count = 0;

  int get count => _count;

  void increment() {
    _count++;
    notifyListeners();
  }
}

class CounterApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return ChangeNotifierProvider(
      create: (context) => Counter(),
      child: MaterialApp(
        home: Scaffold(
          appBar: AppBar(
            title: Text('Counter App with Provider'),
          ),
          body: Center(
            child: CounterDisplay(),
          ),
          floatingActionButton: CounterButton(),
        ),
      ),
    );
  }
}

class CounterDisplay extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Consumer<Counter>(
      builder: (context, counter, child) {
        return Text(
          '${counter.count}',
          style: Theme.of(context).textTheme.headline4,
        );
      },
    );
  }
}

class CounterButton extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return FloatingActionButton(
      onPressed: () {
        Provider.of<Counter>(context, listen: false).increment();
      },
      child: Icon(Icons.add),
    );
  }
}

void main() {
  runApp(CounterApp());
}
```

## Resources

- [Provider package](https://pub.dev/packages/provider)
- [Simple app state management](https://flutter.dev/docs/development/data-and-backend/state-mgmt/simple)
- [Provider, the easy way](https://www.youtube.com/watch?v=d_m5csmrf7I)
