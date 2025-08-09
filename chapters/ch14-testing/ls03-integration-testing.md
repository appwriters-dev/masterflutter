---
id: ls03-integration-testing
title: Integration Testing
description: In this lesson, we will learn how to write integration tests in Flutter.
---

## What is Integration Testing?

An integration test tests a complete app or a large part of an app. The goal of an integration test is to verify that all the widgets and services work together as expected.

To write integration tests in Flutter, you can use the `integration_test` package.

```yaml
dev_dependencies:
  integration_test:
    sdk: flutter
```

## Projects

### 1. Simple Integration Test

Create a simple app with a button that increments a counter, and then write an integration test to verify that the counter is incremented correctly when the button is tapped.

Here is an example of how you can do this:

**lib/main.dart**
```dart
import 'package:flutter/material.dart';

void main() => runApp(MyApp());

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Counter App',
      home: MyHomePage(title: 'Counter App'),
    );
  }
}

class MyHomePage extends StatefulWidget {
  MyHomePage({Key? key, required this.title}) : super(key: key);
  final String title;

  @override
  _MyHomePageState createState() => _MyHomePageState();
}

class _MyHomePageState extends State<MyHomePage> {
  int _counter = 0;

  void _incrementCounter() {
    setState(() {
      _counter++;
    });
  }

  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text(widget.title),
      ),
      body: Center(
        child: Text(
          '$_counter',
          style: Theme.of(context).textTheme.headline4,
        ),
      ),
      floatingActionButton: FloatingActionButton(
        onPressed: _incrementCounter,
        tooltip: 'Increment',
        child: Icon(Icons.add),
      ),
    );
  }
}
```

**integration_test/app_test.dart**
```dart
import 'package:flutter_test/flutter_test.dart';
import 'package:integration_test/integration_test.dart';
import 'package:my_app/main.dart' as app;

void main() {
  IntegrationTestWidgetsFlutterBinding.ensureInitialized();

  testWidgets('tap on the floating action button, verify counter',
      (WidgetTester tester) async {
    app.main();
    await tester.pumpAndSettle();

    // Verify the counter starts at 0.
    expect(find.text('0'), findsOneWidget);

    // Finds the floating action button to tap on.
    final Finder fab = find.byTooltip('Increment');

    // Emulate a tap on the floating action button.
    await tester.tap(fab);

    // Trigger a frame.
    await tester.pumpAndSettle();

    // Verify the counter increments by 1.
    expect(find.text('1'), findsOneWidget);
  });
}
```

## Resources

- [An introduction to integration testing](https://flutter.dev/docs/testing/integration-testing)
- [integration_test package](https://pub.dev/packages/integration_test)
