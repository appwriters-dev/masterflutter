---
id: ls07-collections
title: Collections
---

Recommended Time: 2 days

Collections are derived data structures.

Data structures are central to software development and, by extension, computer science. They are a
significant foundation upon which systems of varying complexity are built. With the popularity of
the Flutter framework driving the rapid growth of Dart, it is becoming increasingly important to
understand the data structures available in this language and how to use them.

## Projects

### 1. Enum
    
Write a enum Season which can have values as different seasons. And write a program that prints your favorite season using the enum.

### 2. List

Create a quiz app that allows users to answer multiple-choice questions. Use a combination of Map and List to store the questions and options for each question, and allow the user to select one of the options.

### 3. Unique Random Number
     
Create a simple random number generator. Use a Set to store the numbers that have been generated, and make sure that each number is unique.

### 4. Shopping List

Create a shopping list app that allows users to add and remove items from a list. Use a Set to store the items in the list and ensure that each item only appears once in the list.

### 5. Understand Map Usage
    
Run this code on your local machine and try to understand how it works on Map.

```dart
enum transmission { manual, automatic }
void main() {
    var car = {
        "model": "Y8",
        "Horsepower": 456,
        "Energy": "Paterol",
        "transmission": transmission.automatic
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
    car.updateAll((key, value) => "unkown");
    print(car);
    car.clear();
    print(car);
}

    Try all the methods avaiable on the Map and their attributes too for the practice purpose.

## Resources

- [data structures in Dart](https://medium.com/@daria.orlova/data-structures-with-dart-set-a034bc7b7d4a)