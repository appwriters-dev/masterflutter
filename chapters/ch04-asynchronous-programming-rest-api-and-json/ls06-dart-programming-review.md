---
id: ls06-dart-programming-review
title: Dart Programming Review
---

Wow, you have done it. You have learned the basics of Dart that are essential to learn Flutter. In the preceeding chapters, we have covered the following topics:

1. Basics of Dart (variables, data types, operators, control flow, collections, null safety, and functions)
2. Object Oriented Programming (classes, objects, constructors, inheritance, and interfaces)
3. Dependency Management (pubspec.yaml, packages, and pub.dev)
4. Asynchronous Programming (async, await, and futures)

## Questions

1. What is the difference between synchronous and asynchronous programming?
2. What is the difference between a class and an object?
3. What is sound null safety in Dart? What are the benefits of sound null safety?
4. What does `dev_dependencies` mean in `pubspec.yaml`?
5. What is the `pub` CLI command to install a package?

## Projects

### 1. Areas of Shapes

Build a CLI app that calculates the area of a different shapes. Display the menu as follows:

```bash
1. Circle
2. Rectangle
3. Square
4. Triangle
5. Exit
```
Based on user selection, ask for the required input and display the area of the shape. For example, if the user selects 1, ask for the radius and display the area of the circle. If the user selects 5, exit the program.

### 2. Quote of the Day

Build a CLI program when executed shows a random quotes of the day every time. Use the [Quotes API](https://quotes.rest/) to fetch the quotes. Parse the JSON response into Dart object and display the quote.

### 3. CLI Scraper

Build a CLI program that scrapes the [Quotes API](https://quotes.rest/) and saves the quotes in a file. The file should be in JSON format. The program should take the number of quotes to scrape as an argument. For example, if the user runs the program as follows:

```bash
dart scraper.dart 10
```

The program should scrape 10 quotes and save them in a file. If the user does not provide the number of quotes to scrape, the program should scrape 10 quotes by default.

### 4. CSV to JSON Converter

Build a CLI program that converts a CSV file to JSON. The program should take the CSV file path as an argument. For example, if the user runs the program as follows:

```bash
dart converter.dart users.csv
```

The program should convert the CSV file to JSON and save it in a file. If the user does not provide the CSV file path, the program should ask for the CSV file path.

> **Note:** Make sure to add a nice Readme file to all your project with description, screenshots, and instructions to run the program. Publish each project once you complete to GitHub and share in your social networks.