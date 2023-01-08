---
id: ls01-navigation
title: Navigation
---

## Learning Objectives

- Use `Navigator` to navigate between pages
- Use named routes

## Projects

### 1. Second Page

Create a new Flutter project. Add a new widget in `lib/second.dart` that has Scaffold and the body shows a text `This is the second page` in the center. The FloatingActionButton of the default page should navigate to the second page.

> Note: You can do this easily using `Navigator.push`

### 2. Named Pages

Modify the previous project to use named routes. Use `MaterialApp`'s `routes` property to define the routes. The default page should navigate to the second page using the name `second`.

Just like with assets, it's always a good practice to keep the route name constants as a class instead of using string everywhere.

```dart
class RouteNames {
    static const String second = 'second';
    static ocnst String home = 'home';
}
```

## Resources

- [Navigation and Routing](https://flutter.dev/docs/development/ui/navigation)
- [Navigator](https://api.flutter.dev/flutter/widgets/Navigator-class.html)
- [MaterialPageRoute](https://api.flutter.dev/flutter/material/MaterialPageRoute-class.html)
- [MaterialApp.routes](https://api.flutter.dev/flutter/material/MaterialApp/routes.html)