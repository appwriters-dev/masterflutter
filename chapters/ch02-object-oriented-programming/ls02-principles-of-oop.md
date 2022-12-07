---
id: ls02-principles-of-oop
title: Principles of OOP
---

## Encapsulation

Encapsulation is the process of hiding the implementation details of a class from the outside world. The only way to interact with an object is through its public interface. This means that the object's internal state is hidden from the outside world. The object's internal state can only be changed by calling public methods. This is a very powerful concept because it allows us to change the implementation of a class without affecting the code that uses it.

## Abstraction

Abstraction is the process of hiding the implementation details of a class from the outside world. The only way to interact with an object is through its public interface. This means that the object's internal state is hidden from the outside world. The object's internal state can only be changed by calling public methods. This is a very powerful concept because it allows us to change the implementation of a class without affecting the code that uses it.

## Inheritance

Inheritance is the process of creating a new class from an existing class. The new class is called a subclass, and the existing class is called a superclass. The subclass inherits all the public and protected methods from the superclass. In addition, it can have its own methods in addition to the superclass's methods. Inheritance is a powerful concept because it allows us to create a new class that is based on an existing class, thus reducing the amount of code that we need to write.

## Projects

### 1. A Game

Create a simple game that uses classes to represent different game entities, such as the player, enemies, and items.

### 2. Abstract Class

 - Create an abstract class called `ArticleDataSource` with method `getArticle(String id)`, and `deleteArticle(String id)`.
 - Create a class called `ArticleLocalDataSource` and implement the `ArticleDataSource`
 - Implement each method and print operation with the provided id. For example, calling `getArticle('dart-today-and-tomorrow')` should print `Get dart-today-and-tomorrow`
 - Add a factory constructor to `ArticleLocalDataSource` and return the object of `ArticleLocalDataSource`.
 - Instantiate `ArticleLocalDataSource` using the factory constructor and call each methods on the object.

### 3. Color Points

The class "Point" is defined as follows:

```dart
class Point {

  int _x, _y;

  Point(this._x, this._y);

  void move(int mx, int my) {

    _x += mx;

    _y += my;

  }



  void display() {

    print("x = $_x   y = $_y");

  }

}
```

- Define a new class `PointCol` derived from `Point` to manipulate colored points.
- Its constructor initializes the color of the object with a given integer (the color reference).
- Add a method "printColor" that print the color.
- Create a small test program (main).

### 4. Create a class "Client" that have 2 private attributes

- Name (can't be changed).
- PurchasesAmount (double) have 2 methods (get, add).

- Create a constructor that initialize the name.
- Create a class "LoyalClient" that have 1 private attribute :
- PurchasesAmount (double) have 1 methods (get).
- Create a method "discount" that assign to PurchasesAmount (subclass) the value of PurchasesAmount (superclass) after reduction of 10%.
- Create a small test program (main) .

Note : Use different names for the get methods.

## Resources

- [Principles of OOP](https://www.freecodecamp.org/news/object-oriented-programming-concepts-21bb035f7260/)
- [OOP in 8 minutes](https://www.youtube.com/watch?v=pTB0EiLXUC8)
- [Inheritance](https://www.darttutorial.org/dart-tutorial/dart-inheritance/)
- [Inheritance](https://dart-tutorial.com/object-oriented-programming/inheritance-in-dart/)
- [Inheritance of Constructor](https://dart-tutorial.com/object-oriented-programming/inheritance-of-constructor-in-dart/)
- [Encapulation in Dart](https://dart-tutorial.com/object-oriented-programming/encapsulation-in-dart/)