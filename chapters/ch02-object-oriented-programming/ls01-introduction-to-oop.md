---
id: ls01-introduction-to-oop
title: Introduction to OOP
---

## What is OOP?

Object-oriented programming (OOP) is a programming paradigm based on the concept of "objects", which can contain data, in the form of fields, often known as attributes; and code, in the form of procedures, often known as methods.

A class is a blueprint for the object. We can think of class as an sketch of a parrot with labels. It contains all the details about the name, colors, size etc. Based on these descriptions, we can study about the parrot. Here, a parrot is an object. An object (instance) is an instantiation of a class. When a class is defined, no memory or storage is allocated but when it is instantiated (i.e. an object is created) memory is allocated. The process of creating this object is called instantiation. The newly created object is called an instance of the class. The instance inherits all the variables and methods from the class but it also has its own unique set of variables and methods. In other words, each object contains an independent copy of the instance variables defined in the class.

## Resources

- [What is Object-oriented programming](https://www.educative.io/blog/object-oriented-programming)
- [OOP Primer](https://www.codeguru.com/visual-basic/an-oop-primer/)
- [OOP Concepts a Primer](https://www.cs.princeton.edu/courses/archive/spr96/cs333/java/tutorial/java/objects/index.html)
- [Class vs Object](https://www.youtube.com/watch?v=BM9tPve8T1o)
- [OOP in 8 minutes](https://www.youtube.com/watch?v=pTB0EiLXUC8)
- [Class in Dart](https://dart-tutorial.com/object-oriented-programming/class-in-dart/)
- [Objects in Dart](https://dart-tutorial.com/object-oriented-programming/object-in-dart/)
- [Class and Objects](https://dart-tutorial.com/object-oriented-programming/class-and-objects-in-dart/)
- [Constructor in Dart](https://dart-tutorial.com/object-oriented-programming/constructor-in-dart/)
- [Default constructor](https://dart-tutorial.com/object-oriented-programming/default-constructor-in-dart/)

## Projects

Projects are a great way to learn. Here are some projects that you can try to get a better understanding of OOP.

### 1. Person

Create a simple program that defines a Person class with properties for a person's name and age, and then creates a few instances of the Person class. This project will help you understand the basics of defining classes and creating objects in Dart.

### 2.  Calculator

Define a calculator class that has

- methods `add`, `subtract`, `multiply`, `divide` and `setInitial` all accept one `double` parameter
- has private nullable property `result` of type double
- `setInitial` will set the initial `result`
- all methods perform the desired calculation to the result and store the result
- Create a test program with main method that initializes the calculator and performs operations

### 2.  Coordinate

Create a class called `Point` allowing to manipulate a point of a plane (x,y).

You will provide:

- A constructor receiving as arguments the coordinates (double) of a point.
- A member function "move" performing a translation defined by its two arguments (double).
- A member function "display" simply displaying the coordinates of the point.

The coordinates of the point should be private data members.

Write separate files:
- A source file constituting the declaration of the class.
- A small test program (main) declaring a point, displaying it, moving it around and showing it again.

### 3.  Vector3D

The class "vector3D" is defined as follows:

```dart
class Vector3D {
    double _x, _y, _z;

    Vector3D(this._x, this._y, this._z);
}
```

- Add new named constructor `same` that have only one argument and initialize the three variables with it.
- Add a member function "coincide" that check if two vectors have the same components.
- A small test program (main)

### 4. Bank Client

Create a class called BankClient that have 3 private attributes : - Id which is generated automatically and represents the order of the client in the bank Data Base (starting from 1 and can't be changed). - Name (can't be changed). - Balance have 3 methods (`getBalance`, `addToBalance`, and `subtractIfPossible`).

- Create a constructor that use "Initializer list" to initialize the name.
- Create a static method that print the number of clients and the bank balance.
- Create a small test program (main) .

Note : The balance is initialized at 0 and can't be negative.
