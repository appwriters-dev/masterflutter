---
id: ls01-basic-interactivity
title: Basic Interactivity
---

Up until now you have been using the Stateless Widgets, that's fine until you are building static layouts. However to build dynamic layouts and add interactivity to your app, you need to use Stateful Widgets.

## Projects

### 1. The Famous Counter App

Create a new Flutter project. It by default comes with a stateful widget. Explore how the `+` button is working incrementing the counter and how the state rebuilds to display the increased counter. Important to note that the `setState()` method is called to rebuild the UI. Also note `setState()` can only be used in a stateful widget.

### 2. Dice App

Create a dice App that displays a random dice number (between 1-6) when the `Roll` button is clicked. The number should be displayed in the center of the screen in large font size. The `Roll` button should be displayed at the bottom of the screen. Use dart's [Random](https://api.dart.dev/stable/2.10.4/dart-math/Random-class.html) class to generate a random number.

### 2. Quiz App

Create a new Flutter project, clear `main.dart` and paste the following code. Complete the following code to build the UI as shown below. Then add the functionality to change the background color of the button when clicked as described below.

**Starter Code**

```dart

void main() => runApp(QuizApp());

class QuizApp extends StatelessWidget {
    @override
    Widget build(BuildContext context) {
        return MaterialApp(
        home: Scaffold(
            backgroundColor: Colors.grey.shade900,
            body: SafeArea(
            child: Padding(
                padding: EdgeInsets.symmetric(horizontal: 10.0),
                child: Quiz(),
            ),
            ),
        ),
        );
    }
}

class Quiz extends StatefulWidget {
  @override
  _QuizState createState() => _QuizState();
}

class _QuizState extends State<Quiz> {
  int questionNumber = 0;
  List<Icon> scoreKeeper;

    @override
    Widget build(BuildContext context) {
      Map<String, dynamic> question = {
        'question': 'Flutter stable version was launched in November 2018',
        'options': ['Yes', 'No'],
        'answer': 'No',
      };

      return Scaffold(); // complete the UI
    }
}
```

When one of the button is clicked, change the clicked buttons background color to green if the answer was correct, red otherwise.

## Resources

- [Stateful vs Stateless Widgets](https://medium.com/flutter-community/flutter-stateful-vs-stateless-widgets-7f8a5e3d7b5b)
- [Stateful Widgets](https://flutter.dev/docs/development/ui/interactive#stateful-widgets)
- [setState()](https://api.flutter.dev/flutter/widgets/State/setState.html)
- [initState()](https://api.flutter.dev/flutter/widgets/State/initState.html)
- [StatefulWidget](https://api.flutter.dev/flutter/widgets/StatefulWidget-class.html)
- [ElevatedButton](https://api.flutter.dev/flutter/material/ElevatedButton-class.html)
- [ElevatedButton.styleFrom](https://api.flutter.dev/flutter/material/ElevatedButton/styleFrom.html)