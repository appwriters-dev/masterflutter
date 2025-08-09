---
id: ls02-widget-testing
title: Widget Testing
description: In this lesson, we will learn how to write widget tests in Flutter.
---

## What is Widget Testing?

A widget test (also known as a component test) tests a single widget. The goal of a widget test is to verify that the widget’s UI looks and interacts as expected.

To write widget tests in Flutter, you can use the `flutter_test` package.

```yaml
dev_dependencies:
  flutter_test:
    sdk: flutter
```

## Projects

### 1. Simple Widget Test

Create a simple widget that displays a message, and then write a widget test to verify that the message is displayed correctly.

Here is an example of how you can do this:

**lib/main.dart**
```dart
import 'package:flutter/material.dart';

class MyWidget extends StatelessWidget {
  final String title;
  final String message;

  const MyWidget({
    Key? key,
    required this.title,
    required this.message,
  }) : super(key: key);

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'MyWidget',
      home: Scaffold(
        appBar: AppBar(
          title: Text(title),
        ),
        body: Center(
          child: Text(message),
        ),
      ),
    );
  }
}
```

**test/widget_test.dart**
```dart
import 'package:flutter_test/flutter_test.dart';
import 'package:my_app/main.dart';

void main() {
  testWidgets('MyWidget has a title and message', (WidgetTester tester) async {
    await tester.pumpWidget(MyWidget(title: 'T', message: 'M'));
    final titleFinder = find.text('T');
    final messageFinder = find.text('M');
    expect(titleFinder, findsOneWidget);
    expect(messageFinder, findsOneWidget);
  });
}
```

## Resources

- [An introduction to widget testing](https://flutter.dev/docs/cookbook/testing/widget/introduction)
- [flutter_test package](https://api.flutter.dev/flutter/flutter_test/flutter_test-library.html)
