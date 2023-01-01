---
id: ls04-scrolling-layout
title: Scrolling Layout
---

Most applications display a large amount of data that does not fit on a single screen. Especially for mobile applications with low screen real state. What are we going to do about it? With a scrollable area. We will practice displaying a large amount of data using a scrolling layout in this lesson. 'SingleChildScrollView' and 'ListView' are two important widgets to remember for this lesson.

## Projects

### 1. List of Names

Display a list of 100 names in a scrolling area. The list should be displayed in a `ListView` widget. Each item in the list should be a `Text` widget with a name. The names can be generated using the [faker](https://pub.dev/packages/faker) package.

> Note: Make sure to explore different properties of `ListView` widget. For example, you can set the `scrollDirection` property to `Axis.horizontal` to display the list horizontally.

### 2. List of Images

Display a list of 10 images in a scrolling area. The list should be displayed in a `ListView` widget. Each item in the list should be an `Image` widget with a random image. The images can be generated using the [faker](https://pub.dev/packages/faker) package.

By using `SingleChildScrollView` you can create a full page design that is scrollable if the view part is still in the app. Also, try using `SingleChildScrollView` by scrolling horizontally inside the row.

### 3. Products List

Imagine you are building a list of products for an e-commerce application. Each product has a name, price, and an image. Display a list of 10 products in a scrolling area. The list should be displayed in a `ListView` widget. Each item in the list should be a `Container` widget with a product name, price, and an image.

> Note: For images use [Pixabay](https://pixabay.com/) or [Pexels](https://www.pexels.com/).

## Resources

- [SingleChildScrollView](https://api.flutter.dev/flutter/widgets/SingleChildScrollView-class.html)
- [ListView](https://api.flutter.dev/flutter/widgets/ListView-class.html)
- [Faker](https://pub.dev/packages/faker)
- [GridView](https://api.flutter.dev/flutter/widgets/GridView-class.html)
- [PageView](https://api.flutter.dev/flutter/widgets/PageView-class.html)
- [CustomScrollView](https://api.flutter.dev/flutter/widgets/CustomScrollView-class.html)
