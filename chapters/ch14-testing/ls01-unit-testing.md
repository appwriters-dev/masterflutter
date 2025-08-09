---
id: ls01-unit-testing
title: Unit Testing
description: In this lesson, we will learn how to write unit tests in Flutter.
---

## What is Unit Testing?

A unit test tests a single function, method, or class. The goal of a unit test is to verify the correctness of a unit of logic under a variety of conditions.

To write unit tests in Flutter, you can use the `test` package.

```yaml
dev_dependencies:
  test: ^1.16.0
```

## Projects

### 1. Simple Unit Test

Create a simple function that adds two numbers, and then write a unit test to verify that it works correctly.

Here is an example of how you can do this:

**lib/main.dart**
```dart
int add(int a, int b) {
  return a + b;
}
```

**test/widget_test.dart**
```dart
import 'package:flutter_test/flutter_test.dart';
import 'package:my_app/main.dart';

void main() {
  test('adds two numbers', () {
    expect(add(1, 2), 3);
  });
}
```

## Resources

- [An introduction to unit testing](https://flutter.dev/docs/cookbook/testing/unit/introduction)
- [test package](https://pub.dev/packages/test)
