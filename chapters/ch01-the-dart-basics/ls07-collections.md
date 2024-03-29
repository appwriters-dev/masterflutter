---
id: ls07-collections
title: Collections
description: Dart is a programming language that provides several built-in collections for storing and managing groups of objects. These collections include lists, sets, and maps, which are useful for storing and organizing data in different ways.
---

Recommended Time: 2 days

Dart is a programming language that provides several built-in collections, which are data structures that store and manage collections of objects. These collections include lists, sets, and maps.

A list is an ordered collection of objects, where each object has a specific index. Lists are useful for storing collections of data that need to be accessed by their index, such as the elements of an array.

A set is an unordered collection of unique objects. Sets are useful for storing collections of data that do not have a specific order, such as the unique values in a list.

A map is a collection of key-value pairs, where each key is associated with a specific value. Maps are useful for storing collections of data that need to be accessed by their keys, such as a dictionary or lookup table.

Dart collections are versatile and powerful, and can be used in a variety of applications. They support common operations such as adding, removing, and searching for elements, as well as more advanced operations such as sorting and filtering.

In summary, Dart is a programming language that provides several built-in collections for storing and managing groups of objects. These collections include lists, sets, and maps, which are useful for storing and organizing data in different ways. Lists are ordered collections of objects, sets are unordered collections of unique objects, and maps are collections of key-value pairs. Dart collections support common operations such as adding, removing, and searching for elements, as well as more advanced operations such as sorting and filtering.

## Projects

### 1. Quiz

Create a quiz app that allows users to answer multiple-choice questions. Use a combination of Map and List to store the questions and options for each question, and allow the user to select one of the options.

### 2. Unique Random Number

Create a simple random number generator. Use a Set to store the numbers that have been generated, and make sure that each number is unique.

### 3. Shopping List

Create a shopping list app that allows users to add and remove items from a list. Use a Set to store the items in the list and ensure that each item only appears once in the list.

### 4. Understand Map Usage

Run this code on your local machine and try to understand how it works on Map.

```dart
void main() {
    var car = {
        "model": "Y8",
        "Horsepower": 456,
        "Energy": "Patrol",
    };
    print(car.length);
    print(car.keys);
    print(car.values);
    car.addAll({"airbags": true});
    print(car);
    car["model"] = "Audi R8";
    print(car);
    car.update("Horsepower", (value) => 650);
    print(car);
    car.remove("Energy");
    print(car);
    car.updateAll((key, value) => "unknown");
    print(car);
    car.clear();
    print(car);
}
```

Try all the methods available on the Map and their attributes too for the practice purpose.

## Resources

- [Collections](https://dart.dev/guides/libraries/library-tour#collections)
- [Collections](https://www.geeksforgeeks.org/dart-collections/)
- [List](https://dart-tutorial.com/collections/list-in-dart/)
- [List](https://api.dart.dev/stable/2.18.5/dart-core/List-class.html)
- [Set](https://dart-tutorial.com/collections/set-in-dart/)
- [Set](https://api.dart.dev/stable/2.18.5/dart-core/Set-class.html)
- [Map](https://dart-tutorial.com/collections/map-in-dart/)
- [Map](https://api.dart.dev/stable/2.18.5/dart-core/Map-class.html)
