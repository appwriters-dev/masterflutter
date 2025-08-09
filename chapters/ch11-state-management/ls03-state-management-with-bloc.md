---
id: ls03-state-management-with-bloc
title: State Management with BLoC
description: In this lesson, we will learn about state management with BLoC.
---

## What is BLoC?

BLoC (Business Logic Component) is a state management system for Flutter that helps to separate business logic from the UI. It is based on the concept of streams and reactive programming.

To use BLoC, you need to add the `flutter_bloc` package to your `pubspec.yaml` file:

```yaml
dependencies:
  flutter_bloc: ^8.0.0
```

## Projects

### 1. Counter App with BLoC

Re-create the counter app from the previous lessons, but this time use BLoC to manage the state.

Here is an example of how you can implement this:

```dart
import 'package:flutter/material.dart';
import 'package:flutter_bloc/flutter_bloc.dart';

abstract class CounterEvent {}

class IncrementEvent extends CounterEvent {}

class CounterBloc extends Bloc<CounterEvent, int> {
  CounterBloc() : super(0) {
    on<IncrementEvent>((event, emit) => emit(state + 1));
  }
}

class CounterApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return BlocProvider(
      create: (context) => CounterBloc(),
      child: MaterialApp(
        home: Scaffold(
          appBar: AppBar(
            title: Text('Counter App with BLoC'),
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
    return BlocBuilder<CounterBloc, int>(
      builder: (context, count) {
        return Text(
          '$count',
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
        context.read<CounterBloc>().add(IncrementEvent());
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

- [Bloc Library](https://bloclibrary.dev/)
- [Flutter BLoC package](https://pub.dev/packages/flutter_bloc)
- [Getting Started with BLoC](https://www.youtube.com/watch?v=LeLrsnHeCZY)
