---
id: ls04-scrolling-layout
title: Scrolling Layout
---

Most applications display a large amount of data that does not fit on a single screen. Especially for mobile applications with low screen real state. What are we going to do about it? With a scrollable area. We will practice displaying a large amount of data using a scrolling layout in this lesson. 'SingleChildScrollView' and 'ListView' are two important widgets to remember for this lesson.

## Projects

### 1. List of Names

Display a list of 100 names in a scrolling area. The list should be displayed in a `ListView` widget. Each item in the list should be a `Text` widget with a name. The names can be generated using the [faker](https://pub.dev/packages/faker) package.

### 2. List of Images

Display a list of 10 images in a scrolling area. The list should be displayed in a `ListView` widget. Each item in the list should be an `Image` widget with a random image. The images can be generated using the [faker](https://pub.dev/packages/faker) package.

### 3. GridView 

Create a two-column `GridView`. To separate the children, use the crossAxisSpacing and mainAxisSpacing properties.

### 4. PageView 

By wrapping `PageViw` widget , Creates a page with centered Text in each of the three pages which scroll horizontally.

### 5. SingleChildScrollView

By using `SingleChildScrollView` you can create a full page design that is scrollable if the view part is still in the app. Also, try using `SingleChildScrollView` by scrolling horizontally inside the row.

### 6. CustomScrollView

By using `CustomScrollView` , Make a scroll view with an expanding app bar, a list, and a grid by combining three slivers: SliverAppBar, SliverList, and SliverGrid.

## Resources

- [SingleChildScrollView](https://api.flutter.dev/flutter/widgets/SingleChildScrollView-class.html)
- [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html)
- [Faker](https://pub.dev/packages/faker)
- [GridView](https://api.flutter.dev/flutter/widgets/GridView-class.html)
- [PageView](https://api.flutter.dev/flutter/widgets/PageView-class.html)
- [CustomScrollView](https://api.flutter.dev/flutter/widgets/CustomScrollView-class.html)
