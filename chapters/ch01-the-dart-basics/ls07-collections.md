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

     Write a program for the list, which have Value1 , Value2 and Value3 and print the values from that list.

### 3. Set
     
    Understand the Types of set from the given resource and write a program by using add and addAll functions and add values and print from there.

### 4. Map

    The Map object is a straightforward key/value pair. A map's keys and values can be of any type. A map is a living collection. In other words, Maps can expand and contract at runtime.There are two ways to declare maps.
         - Making Use of Map Literals
         - Making Use of a Map Constructor

## Example code by using Map
    
    Run this code on your local machine and try to understand how it works on Map.
    
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