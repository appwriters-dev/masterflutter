---
id: ls01-basic-material-layout
title: Basic Material Layout
---

In this lesson we will learn about various widgets that are used to create a basic layout following the Material Design guidelines. We will be using the following widgets:

1. Material App
2. Scaffold, 
3. AppBar
4. FloatingActionButton
5. BottomNavigationBar

## Projects

### 1. Flutter Create

Create a new Flutter project. Open the project in VS Code. Now open the `main.dart` file and investigate the code. You will see that the code is already written for you. This basic app already uses `MaterialApp`, `Scaffold`, `AppBar`, and `FloatingActionButton` widgets. Investigate how they are used. You can also run the app to see how it looks. You can try changing the different properties assigned to the widgets to see how it affects the app.

### 2. Build The Following Layout

Build following layout using the Material design widgets.

![Simple material UI](/images/ch06-ls01-pr02.png)

> Hint: Use `Container` with a linear gradient in `decoration` for the background effect. Other helpful widget will be `Card`, and `ListTile`

### 3. People App

Create a Flutter application that displays a list of people from the data given below.

```dart
List people = [
  {
    "name": "Jessica Smith",
    "age": 27,
    "address": "123 Main Street, Nepal",
    "email": "jessica.smith@example.com"
  },
  {
    "name": "Michael Williams",
    "age": 35,
    "address": "456 Park Avenue, Nepal",
    "email": "michael.williams@example.com"
  },
  {
    "name": "Sarah Johnson",
    "age": 29,
    "address": "789 Maple Street, Nepal",
    "email": "sarah.johnson@example.com"
  },
  {
    "name": "Jason Thompson",
    "age": 41,
    "address": "321 Oak Street, Nepal",
    "email": "jason.thompson@example.com"
  },
  {
    "name": "Amanda Davis",
    "age": 22,
    "address": "159 Pine Street, Nepal",
    "email": "amanda.davis@example.com"
  }
];
```

The app should have the following features:

1. The app should have a `Scaffold` widget as the root widget.
2. The app should have an `AppBar` widget at the top of the screen.
3. The app should have a `FloatingActionButton` widget at the bottom right of the screen.
4. The app should have a `BottomNavigationBar` widget at the bottom of the screen.
5. The app should have a `ListView` widget that displays the list of people.
6. The app should have a `Card` widget that displays the details of a person.

### 4. Material Widgets

Write an article covering any two of the material widgets that we have learned about in this lesson. The article should include the following:

1. A brief introduction to the widget.
2. Code snippets showing how to use the widget.
3. Screenshot of the app that uses the widget.

Publish the article on medium or dev.to and share the link in your social media.

## Resources

1. [Material Design](https://material.io/design/)
2. [Material App](https://api.flutter.dev/flutter/material/MaterialApp-class.html)
3. [Scaffold](https://api.flutter.dev/flutter/material/Scaffold-class.html)
4. [AppBar](https://api.flutter.dev/flutter/material/AppBar-class.html)
5. [FloatingActionButton](https://api.flutter.dev/flutter/material/FloatingActionButton-class.html)
6. [BottomNavigationBar](https://api.flutter.dev/flutter/material/BottomNavigationBar-class.html)
7. [ListTile](https://api.flutter.dev/flutter/material/ListTile-class.html)
8. [Card](https://api.flutter.dev/flutter/material/Card-class.html)
9. [LinearGradient](https://api.flutter.dev/flutter/painting/LinearGradient-class.html)