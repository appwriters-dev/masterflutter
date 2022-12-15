---
id: ls04-scrolling-layout
title: Scrolling Layout
---

An application most of the time shows a lot of data that doesn't fit in a single screen. Especially for mobile applications where screen real state is very low. How do we deal with that? With scrolling area. In this lesson, we will practice displaying a lot of data using a scrolling layout. Two key widgets to remember for this lesson is `SingleChildScrollView` and `ListView`.

## Projects

### 1. List of Names

Display a list of 100 names in a scrolling area. The list should be displayed in a `ListView` widget. Each item in the list should be a `Text` widget with a name. The names can be generated using the [faker](https://pub.dev/packages/faker) package.

### 2. List of Images

Display a list of 10 images in a scrolling area. The list should be displayed in a `ListView` widget. Each item in the list should be an `Image` widget with a random image. The images can be generated using the [faker](https://pub.dev/packages/faker) package.

## Resources

- [SingleChildScrollView](https://api.flutter.dev/flutter/widgets/SingleChildScrollView-class.html)
- [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html)
- [Faker](https://pub.dev/packages/faker)
