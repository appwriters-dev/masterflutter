---
id: ls03-themes
title: Themes
---

Theming allows you to change the look and feel of your application. It is a useful feature that allows you to change the appearance of your application without changing the code. You can customize your application's colors, fonts, and other visual elements.

## Projects

### 1. Understanding Theme

Create a new Flutter project. Update the theme so that scaffold background color is `white`, `AppBar` background color is `lime`. Update the existing `Text` widget to use the `headline1` style (check `Theme.of(context).textTheme`).

### 2. Text Theme

Create a new Flutter project. Update the `AppBar` theme so that the background color is `indigo`. Also update AppBar title text style so that font size is `20` and weight is `bold`.  Update the text theme of the application so that body text size is `16` and `headline1` to `headline6` sizes are `28, 26, 24, 22, 20, 18` respectively.

Finally, create a simple home page with AppBar and multiple text widget in body that uses style from headline 1 to 6 and also normal body text.


## Resources

- [MaterialApp.theme](https://api.flutter.dev/flutter/material/MaterialApp/theme.html)
- [ThemeData](https://api.flutter.dev/flutter/material/ThemeData-class.html)
- [MaterialApp.darkTheme](https://api.flutter.dev/flutter/material/MaterialApp/darkTheme.html)
- [ThemeData.dark](https://api.flutter.dev/flutter/material/ThemeData/dark.html)
- [ThemeData.light](https://api.flutter.dev/flutter/material/ThemeData/light.html)
