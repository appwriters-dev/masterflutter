---
id: ls01-state-management-with-inherited-widget
title: State Management with InheritedWidget
description: In this lesson, we will learn about state management with InheritedWidget.
---

## What is State Management?

In a Flutter app, "state" is whatever data you need in order to rebuild your UI at any moment. When the state of your app changes (for example, the user flips a switch in the settings screen), you change the state, and that tells Flutter to redraw the UI.

## What is InheritedWidget?

The `InheritedWidget` is a special widget that can be used to pass data down the widget tree. It's a way to share data between widgets without having to pass it down through constructors.

## Projects

### 1. Counter App with InheritedWidget

Create a simple counter app that uses an `InheritedWidget` to share the counter state. The app should have a button to increment the counter and a text widget to display the current count.

Here is an example of how you can implement this:

```dart
import 'package:flutter/material.dart';

class CounterState extends InheritedWidget {
  final int count;
  final VoidCallback onIncrement;

  CounterState({
    required this.count,
    required this.onIncrement,
    required Widget child,
  }) : super(child: child);

  static CounterState of(BuildContext context) {
    return context.dependOnInheritedWidgetOfExactType<CounterState>()!;
  }

  @override
  bool updateShouldNotify(CounterState oldWidget) {
    return count != oldWidget.count;
  }
}

class CounterApp extends StatefulWidget {
  @override
  _CounterAppState createState() => _CounterAppState();
}

class _CounterAppState extends State<CounterApp> {
  int _count = 0;

  void _increment() {
    setState(() {
      _count++;
    });
  }

  @override
  Widget build(BuildContext context) {
    return CounterState(
      count: _count,
      onIncrement: _increment,
      child: MaterialApp(
        home: Scaffold(
          appBar: AppBar(
            title: Text('Counter App'),
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
    final state = CounterState.of(context);
    return Text(
      '${state.count}',
      style: Theme.of(context).textTheme.headline4,
    );
  }
}

class CounterButton extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    final state = CounterState.of(context);
    return FloatingActionButton(
      onPressed: state.onIncrement,
      child: Icon(Icons.add),
    );
  }
}

void main() {
  runApp(CounterApp());
}
```

## Resources

- [InheritedWidget](https://api.flutter.dev/flutter/widgets/InheritedWidget-class.html)
- [Managing state using inherited widgets](https://flutter.dev/docs/development/data-and-backend/state-mgmt/simple#managing-state-using-inheritedwidgets)
